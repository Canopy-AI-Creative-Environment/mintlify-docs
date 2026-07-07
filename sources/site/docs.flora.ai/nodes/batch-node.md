# Source: https://docs.flora.ai/nodes/batch-node

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/batch-node.md).

The Batch Node allows you to aggregate multiple images, videos, or text items and process them all through one or more downstream generation nodes. Instead of manually running the same operation multiple times, the Batch Node automates bulk processing—saving time and ensuring consistency across all your outputs.

## 

Overview

The Batch Node is designed for workflows where you need to apply the same transformation to multiple inputs:

- **Upscale a collection of images** using the same enhancement model
 
- **Generate variations** from multiple reference images
 
- **Apply consistent styling** across a set of base images
 
- **Process multiple text prompts** through the same generation pipeline
 

Think of it as a "for each" loop for your creative workflow—define the operation once, and the Batch Node applies it to every item in the collection.

---

## 

Getting Started

### 

Adding a Batch Node

1

**Add the Node**

From the node menu, select **Batch** to add it to your canvas.

2

**Add Items to the Batch**

Populate your batch with items using any of these methods:

- **Connect upstream nodes** - Link image, video, or text nodes to the batch input
 
- **Upload files** - Click the Upload button or drag-and-drop files onto the node
 
- **Drag from asset library** - Pull items from your workspace history or assets
 

3

**Connect a Generation Node**

Link the Batch Node output to a generation node (Image, Video, or Text). This defines what operation will be applied to each item.

4

**Run the Generation**

Execute the downstream node. The batch automatically processes all items in parallel, creating separate outputs for each input.

---

## 

Adding Items to a Batch

### 

Connecting Upstream Nodes

The most common way to populate a batch is by connecting other nodes:

1. Create your source nodes (image generators, uploads, etc.)
 
2. Connect each source to the Batch Node's input handle
 
3. When source nodes produce output, those outputs appear as items in your batch
 

Multiple nodes can feed into the same batch, allowing you to collect outputs from various sources.

### 

Uploading Files

Click the **Upload** button in the Batch Node to select files from your computer, or simply drag-and-drop files directly onto the node.

**Supported file types:**

Modality

Formats

Images

PNG, JPG, JPEG, WEBP, SVG

Videos

MP4, WEBM, MOV

Text

CSV

### 

Uploading a CSV

You can upload a `.csv` file to quickly populate a text batch. FLORA reads the first column of each row and creates one batch item per row. All rows are included (there is no header skip), so remove any header row you don't want processed.

Drag-and-drop a CSV onto the node, or click **Upload** and select a `.csv` file. You'll see a toast confirming how many rows were added. If the batch already has items, the new rows are appended up to the 100-item limit.

### 

Dragging from Assets

Drag items from the workspace sidebar directly onto the Batch Node:

- **History** - Previously generated images or videos
 
- **Assets** - Saved items in your workspace
 
- **Unsplash** - Stock photos from the Unsplash integration
 

### 

Splitting Text Inputs

When text nodes are connected to a batch, a **text split toolbar** appears above the node. This lets you split each connected text node's content into separate batch items using a delimiter.

The toolbar offers three modes via the **Input split** dropdown:

- **None** (default) — Each connected text node is one batch item
 
- **By line** — Splits on newlines, so each line becomes its own batch item
 
- **Custom** — Splits on any string you type (e.g. `;`, `|`, `//`)
 

For example, if a text node contains `"cat\ndog\nbird"` and you select **By line**, the batch will contain three items: "cat", "dog", and "bird". Empty and whitespace-only segments are automatically filtered out.

Text splitting and CSV upload work together — CSV-uploaded items are preserved when you change the split mode, and vice versa.

---

## 

Modality Locking

The Batch Node locks to a single content type (modality) once you add your first item:

- Add an image → the batch becomes an **image batch**
 
- Add a video → the batch becomes a **video batch**
 
- Connect a text node → the batch becomes a **text batch**
 

You cannot mix different content types in the same batch. All items must be the same modality (all images, all videos, or all text).

If you remove all items from a batch, the modality lock is released, allowing you to start fresh with a different content type.

---

## 

The Batch Interface

### 

Header

Displays the batch icon, the current modality (if set), and the total item count.

### 

Item List

Shows all items currently in the batch with:

- **Thumbnail** for images and videos
 
- **Text preview** (first 100 characters) for text items
 
- **Source label** indicating where the item came from
 
- **Delete option** to remove individual items
 

### 

Footer

- **Upload button** to add more items
 
- **Add Generation Node** button to quickly connect a downstream processing node
 

---

## 

Processing a Batch

### 

How Batch Execution Works

When you run a generation node connected to a batch:

1. **Usage validation** - FLORA checks you have sufficient budget for all items
 
2. **Task creation** - A separate generation task is created for each batch item
 
3. **Parallel processing** - All items are processed simultaneously
 
4. **Output creation** - Each item produces its own output in the generation history
 

### 

Cost Calculation

Batch processing costs are calculated as:

AskCopy

```
Total Cost = Generation Cost per Item × Number of Items
```

For example, if upscaling costs $0.05 per image and your batch contains 10 images, the total cost is $0.50.

FLORA validates your usage budget before starting. If you don't have enough budget for all items, the batch won't start.

### 

Generation Limits

- **Maximum items per batch execution**: 100 items
 
- If your batch contains more than 100 items, you'll need to run the generation multiple times
 

---

## 

Connecting to Generation Nodes

### 

Quick Connect

Click the **arrow button** in the Batch Node footer to open a node selection modal. Choose a generation node type to automatically create and connect it.

### 

Manual Connection

Drag from the Batch Node's output handle to any compatible downstream node:

- **Image Node** - For image-to-image transformations, upscaling, style transfer
 
- **Video Node** - For image-to-video generation
 
- **Text Node** - For image-to-text or text processing
 
- **Technique Node** - For running a full multi-step technique pipeline on each batch item
 

### 

How Connections Work

When a batch is connected to a downstream node:

- **Image batches** replace the image input for each generation
 
- **Video batches** replace the video input for each generation
 
- **Text batches** inject text content into the prompt parameter
 

The downstream node's settings (model, parameters, prompt) apply identically to every item in the batch.

### 

Multiple Downstream Nodes

A single Batch Node can connect to multiple generation nodes downstream. Each downstream node independently processes every item in the batch, so one collection of inputs can feed into several different operations at once.

---

## 

Combining Two Batches (Batch × Batch)

You can connect **two** Batch Nodes to the same downstream generation node to produce results for every pairing — each output combines one item from Batch A with one item from Batch B. This is ideal for exploring style × subject grids, prompt × reference comparisons, or any "every-of-these against every-of-those" workflow.

When a generation node has exactly two Batch Nodes connected, a **Zip / Cross** toggle appears on the node:

- **Cross** (default) — Cartesian product. If Batch A has N items and Batch B has M items, the node generates N × M outputs, one for every possible pair.
 
- **Zip** — Positional pairing. Pairs items by index, producing `min(N, M)` outputs. The toggle is only enabled when both batches have matching item counts; when sizes differ, the node stays in Cross mode automatically.
 

Switching modes updates the generate button's item count and credit cost in real time. Your choice persists with the node.

The Zip / Cross toggle supports all four block types — Image, Video, Text, and Audio. Connecting three or more Batch Nodes to a single generation node is not supported.

### 

Tracking Which Output Came From Which Pair

Every result is tagged with its source pair (one item from each parent batch), so you can navigate between inputs and outputs:

- **Input → Output** — Click an item in either parent batch to scroll the result carousel to the generation that used that item.
 
- **Output → Input** — Selecting a result highlights the matching item in both parent batches.
 

This two-way sync works the same in Zip and Cross mode, and stays correct even if you later reorder items in either parent batch.

### 

Matrix View (Fullscreen)

When a generation node is in **Cross** mode, the fullscreen view (double-click any result) adds a new **Matrix** layout option alongside Single and Masonry.

The Matrix is a grid where rows correspond to Batch A items and columns to Batch B items. Every cell shows the generation produced by that (row, column) pair, and sticky row and column headers display each parent batch's thumbnails so you can always see the inputs.

In the Matrix view you can:

- **Hover a cell** to reveal the two source thumbnails and a download button
 
- **Click a completed cell** to open that result in the Single view, with its metadata panel, prompt drawer, and keyboard navigation
 
- **Download a cell** directly — same formats and filename scheme as the rest of fullscreen
 

Pending cells show a spinner in place; failed cells show an error icon with a tooltip describing the failure.

The Matrix option appears only in Cross mode when both parent batches have thumbnailable items. Zip-mode and single-batch results continue to use the Masonry and Single layouts.

### 

Chaining Beyond Two Batches

You are not limited to mixing two live batches at the same node. A Cross (or Zip) arm can also be the **history of a previous batch generation** — so you can feed a batch result into another block, then combine that block's history with a third batch to explore a new dimension. The Matrix view supports these combinations too: row or column headers draw from the history arm when that input is a prior generation rather than a live batch.

---

## 

Workflow Examples

### 

Example 1: Batch Upscaling

AskCopy

```
[Image 1] ─┐
[Image 2] ─┼─→ [Batch Node] ─→ [Image Node: Upscale] → 3 upscaled outputs
[Image 3] ─┘     (3 items)       (Magnific 2x)
```

All three images are upscaled using the same model and settings.

### 

Example 2: Style Transfer Across Multiple Images

AskCopy

```
[Photo 1] ─┐
[Photo 2] ─┼─→ [Batch Node] ─→ [Image Node] → 4 stylized outputs
[Photo 3] ─┤     (4 items)     "anime style"
[Photo 4] ─┘
```

Apply the same "anime style" prompt to all four photos.

### 

Example 3: Generate Videos from Multiple Images

AskCopy

```
[Product Shot 1] ─┐
[Product Shot 2] ─┼─→ [Batch Node] ─→ [Video Node] → 3 product videos
[Product Shot 3] ─┘     (3 items)     "slow zoom"
```

Create video animations from multiple product images.

### 

Example 4: Style × Subject Grid (Batch × Batch, Cross Mode)

AskCopy

```
[Photo 1] ─┐
[Photo 2] ─┼─→ [Batch A: 3 subjects] ─┐
[Photo 3] ─┘                          │
                                      ├─→ [Image Node, Cross] → 3 × 3 = 9 outputs
[Anime]   ─┐                          │        (open fullscreen → Matrix)
[Pixar]   ─┼─→ [Batch B: 3 styles] ──┘
[Watercolor] ─┘
```

Generate every combination of 3 photos across 3 styles, then compare them side-by-side in the Matrix view.

### 

Example 5: Batch Technique Processing

Run an entire multi-step technique pipeline on each item in the batch. Each product image is processed through the full technique workflow independently, producing complete outputs for every item.

---

## 

Managing Batch Items

### 

Removing Items

Hover over an item in the batch list and click the delete button to remove it. Removing an item also disconnects it from any source node.

### 

Clearing the Batch

Remove all items to reset the batch completely, including its modality lock.

### 

Item Sources

Each item displays its source:

- **Node name** - For items from connected nodes
 
- **"Uploaded file"** - For manually uploaded items
 

---

## 

Tips for Effective Batch Processing

- **Consistent quality** - Ensure all source images have similar quality and dimensions for best results
 
- **Test first** - Run a single item through your generation node before processing the full batch
 
- **Check your budget** - Verify you have enough usage budget before starting large batches
 
- **Monitor progress** - Each item generates independently, so you can see results as they complete
 
- **Organize sources** - Name your source nodes clearly to track which outputs came from which inputs
 

---

## 

Limitations

Limitation

Details

Single modality only

Cannot mix images, videos, and text in one batch

CSV first column only

CSV upload reads only the first column per row

100 items per execution

Larger batches require multiple runs

Same settings for all

Cannot customize parameters per item

Two batches max per node

A single generation node accepts at most two Batch Nodes (Cross / Zip) — connecting a third disables batch × batch

Zip requires equal sizes

Zip mode is only enabled when both parent batches have the same item count; otherwise the node stays in Cross mode

---

## 

Using Batch Nodes Inside Techniques

Batch nodes can be included inside Techniques, enabling fan-out processing as part of a reusable workflow. When a Technique contains a Batch node:

- The batch fan-out executes as an internal step during the technique run
 
- Collection outputs are surfaced on the technique node's output slots
 
- Users can view each item in the collection from the sidebar, detail view, or App Mode
 

This lets technique authors build workflows that process multiple items — for example, a technique that takes one product photo and generates a batch of ad variations from it.

Chaining multiple batch nodes inside a technique in a way that creates explosive fan-out (e.g., batch → batch) is blocked at publish time to prevent runaway costs.

---

## 

Common Use Cases

- **Product photography** - Apply consistent editing to an entire product line
 
- **Social media content** - Generate multiple variations for A/B testing
 
- **Asset preparation** - Upscale or enhance a collection of images at once
 
- **Video creation** - Turn a series of images into individual video clips
 
- **Style exploration** - Apply different models to the same set of inputs (using multiple batches)
 
- **Style × subject grids** - Use Batch × Batch in Cross mode to explore every combination of a prompt set against a reference set, then review results in the Matrix view
 
- **A/B pairing** - Use Zip mode to pair two parallel lists (e.g. prompts with matching reference images) at the same index
 

[PreviousAction Node](https://docs.flora.ai/nodes/action-node) [NextExport Node](https://docs.flora.ai/nodes/export-node)

Last updated 1 month ago

Was this helpful?