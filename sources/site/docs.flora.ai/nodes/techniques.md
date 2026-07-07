# Source: https://docs.flora.ai/nodes/techniques

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/techniques.md).

Techniques are pre-built, multi-step AI workflows that you can add to your canvas and run with a single click. Each technique encapsulates a complex generation pipeline—combining multiple models and processing steps—into a simple node with defined inputs and outputs.

## 

Overview

Instead of manually building complex workflows from scratch, Techniques let you leverage proven creative pipelines built by FLORA and the community. Think of them as "recipes" for AI generation—you provide the ingredients (inputs), and the technique handles all the intermediate steps to produce the final result.

**What makes Techniques powerful:**

- **Multi-step workflows** - Chain multiple AI models together (e.g., analyze image → generate prompt → create video)
 
- **Action nodes** - Include deterministic processing steps (color grading, audio extraction, video effects) alongside AI generation
 
- **Batch processing** - Include Batch nodes inside techniques to fan out and process collections of items in a single run
 
- **Consistent results** - Same pipeline, same quality, every time
 
- **Time-saving** - Skip the setup and get straight to creating
 
- **Curated quality** - Each technique is tested and optimized for its specific use case
 

---

## 

The Techniques Library

### 

Browsing Techniques

Access the Techniques Library from the sidebar to explore all available techniques. The library features:

- **Featured carousel** - Highlighted techniques at the top
 
- **Category filters** - Browse by use case
 
- **Search** - Find techniques by name, description, or tags
 
- **Preview cards** - See sample outputs before adding to canvas
 

### 

Categories

Techniques are organized into the following categories:

Category

Description

Brand & Visual Design

Logo treatments, brand assets, visual identity

Product Visualization

Product shots, mockups, lifestyle imagery

Marketing & Ads

Ad creatives, social media content, campaigns

Video & Animation

Motion graphics, animated sequences, video ads

Fashion & Apparel Editorial

Lookbooks, fashion photography, styling

Content Packaging

Thumbnails, covers, promotional materials

Print Film/VFX

Film-quality effects, cinematic treatments

Space & Architecture

Interior design, architectural visualization

Fun & Inspiration

Creative experiments, artistic styles

### 

Technique Details

Click any technique card to view its detail page, which shows:

- **Description** - What the technique does and ideal use cases
 
- **Inputs required** - What you need to provide (images, videos, or text)
 
- **Outputs produced** - What you'll receive when the technique completes
 
- **Example presets** - Sample inputs and their corresponding outputs
 
- **Usage cost** - How much usage the technique consumes per run
 
- **Estimated time** - Approximate execution duration
 

---

## 

Adding Techniques to Your Canvas

### 

From the Add-Node Menu

The fastest way to add a technique is directly from the canvas add-node menu:

1. Open the add-node menu (click **+** on the toolbar or press **Shift+T** to jump straight to techniques)
 
2. Select **Technique** from the Media section to open the technique picker panel
 
3. Browse **Recent** and **Featured** techniques, or use the search bar to find a specific one
 
4. Hover over any technique to see a preview card with its thumbnail, description, and creator info
 
5. Click a technique or press its number key shortcut (**1-9**) to add it to your canvas at the cursor position
 

Use the **Back** button to return to the main add-node menu, or **View all** to open the full Techniques Library.

### 

From the Library

1

**Browse and Select**

Open the Techniques Library and find a technique that matches your needs. Click the technique card to view details.

2

**Add to Canvas**

Click the **Add to Canvas** button. A Technique Node node appears on your canvas with all input and output slots ready.

3

**Connect Inputs**

Provide the required inputs by connecting source nodes to each input slot on the technique node.

4

**Run the Technique**

Once all inputs are connected, click **Run** to execute the technique. The workflow processes automatically and creates output nodes when complete.

---

## 

The Technique Node

When you add a technique to your canvas, it appears as a Technique Node—a specialized node that represents the entire workflow.

### 

Node Structure

- **Header** - Displays the technique name, icon, and usage cost
 
- **Input slots** - Connection points for each required input (left side)
 
- **Output slots** - Connection points for each output (right side)
 
- **Run button** - Execute the technique when all inputs are ready
 

### 

Input Cards

Each input slot shows:

- **Input name** - What type of content is expected
 
- **Input type** - Image, video, or text indicator
 
- **Connection status** - Whether an input is connected or missing
 
- **Thumbnail** - Preview of the connected input (for images/videos)
 

---

## 

Providing Inputs

Techniques require specific inputs to run. There are several ways to provide each input:

### 

Connect Existing Nodes

Drag a connection from any compatible node output to the technique's input slot:

- **Image inputs** - Connect from Image nodes, uploads, or other image outputs
 
- **Video inputs** - Connect from Video nodes or video uploads
 
- **Text inputs** - Connect from Text nodes
 
- **Document inputs** - Connect from Document nodes (PDF to Text, PDF to Image)
 

### 

Quick Input Actions

Right-click an input slot or use the input menu to quickly add content:

Action

Description

Add Preset

Insert a sample input from the technique's examples

Generate

Run the technique and generate outputs

Upload

Upload a file directly to this input

### 

Using Presets

Each technique includes example presets—sample inputs that demonstrate the technique's capabilities. Adding a preset creates a static node with the sample content, letting you test the technique immediately.

---

## 

Running Techniques

### 

Execution Process

When you run a technique:

1. **Validation** - FLORA checks all required inputs are connected and valid
 
2. **Usage check** - Confirms you have sufficient budget for the run
 
3. **Processing** - The internal workflow executes step by step (including both AI generation steps and any deterministic action steps)
 
4. **Progress tracking** - The technique node shows real-time progress
 
5. **Output creation** - Result nodes appear connected to the technique's outputs
 

### 

Parameter Overrides

Some techniques allow you to customize specific outputs before running. When a technique author has enabled **user-editable parameters** on an output, you'll see a settings icon on that output slot. Click it to override the model or generation parameters (such as aspect ratio, quality, or style) for that output.

Overrides are validated server-side — only safe parameters can be changed (e.g., you cannot override cost-related knobs like quantity or seed). The technique's usage cost is automatically recalculated to reflect your chosen overrides.

### 

Usage Costs

Each technique has a usage cost displayed in the header. This cost covers all the internal generation steps—you pay once for the entire workflow, not per internal step. If you override parameters on any output, the cost is recalculated to reflect the actual models and settings used.

Usage is deducted when the technique starts. If a technique fails, the deduction is automatically refunded.

### 

Progress Indicator

While running, the technique node displays:

- **Progress bar** - Visual indicator of completion percentage
 
- **Current step** - Which internal node is currently processing
 
- **Estimated time remaining** - Approximate time until completion
 

---

## 

Working with Outputs

### 

Output Nodes

When a technique completes, it automatically creates output nodes on your canvas:

- **Image outputs** - Appear as result image nodes
 
- **Video outputs** - Appear as result video nodes
 
- **Text outputs** - Appear as result text nodes
 

These output nodes are connected to the technique node and can be used as inputs for other nodes in your workflow.

### 

Collection Outputs

Techniques that include Batch nodes produce **collection outputs** — multiple items from a single output slot. When a technique contains a fan-out step, the batch results are surfaced as a scrollable collection on the technique node's output. Each item in the collection can be viewed individually in the sidebar, detail view, or App Mode.

### 

Feedback

After a technique completes, you can provide feedback on the outputs using the thumbs up/down buttons. This helps improve technique quality over time.

### 

Chaining Techniques

Output nodes from one technique can be connected to inputs of another technique or any other node, enabling complex multi-technique workflows.

---

## 

Batch Processing with Techniques

Techniques can be run through a [Batch Node](https://docs.flora.ai/nodes/batch-node) to process multiple inputs through the same technique pipeline at once. This is useful when you want to apply the same creative workflow to a collection of images, videos, or other media.

### 

How It Works

1. Add a **Batch Node** to your canvas and populate it with your items
 
2. Connect the Batch Node's output to a **Technique Node's** input
 
3. Click **Run** on the technique — each batch item is processed through the full technique pipeline independently
 
4. Outputs are created for each batch item, with carousel navigation to browse results
 

### 

Use Cases

- **Product line processing** - Run a lifestyle photography technique across an entire product catalog
 
- **Campaign variations** - Generate branded ad creatives from multiple source images in one pass
 
- **Bulk video creation** - Convert a batch of product shots into animated videos using the same technique
 

---

## 

Detaching Techniques

Want to see how a technique works internally? You can "detach" a technique to expand it into its constituent nodes.

### 

How to Detach

1. Select the Technique Node
 
2. Click the **Detach** option in the toolbar or context menu
 
3. The technique expands into individual nodes on your canvas
 

### 

What Happens

- The technique node is replaced by all internal nodes
 
- Connections are preserved and mapped to the expanded nodes
 
- You can now see and modify each step of the workflow
 
- Action nodes appear as labeled "Action" blocks — the label is derived from the action's function name or schema
 

Detaching is one-way—you cannot re-collapse nodes back into a technique node. Consider duplicating the technique before detaching if you want to keep the original.

---

## 

Viewing a Technique's Workflow

You can preview a technique's internal workflow without detaching it by clicking **View workflow** in the Technique Node toolbar. This opens a read-only overlay that shows the full graph — generation nodes, action nodes, and their connections. Action nodes are displayed with a distinctive violet style so they're easy to spot.

---

## 

Tips for Using Techniques

- **Check the examples first** - Review technique presets to understand what inputs work best
 
- **Match input quality** - Higher quality inputs generally produce better outputs
 
- **Mind aspect ratios** - Some techniques work best with specific aspect ratios (noted in input descriptions)
 
- **Test with presets** - Try the built-in presets before using your own content
 
- **Watch usage costs** - Complex techniques with many steps may use more of your budget
 
- **Use technique outputs downstream** - Chain technique outputs into other nodes for extended workflows
 

---

## 

Technique vs. Manual Workflows

Aspect

Technique

Manual Workflow

Setup time

Instant—just add and connect inputs

Requires building from scratch

Consistency

Same pipeline every time

May vary between sessions

Customization

Author-defined parameter overrides

Full control over every parameter

Learning curve

Use immediately without expertise

Requires understanding each model

Usage cost

Single fixed cost

Varies based on nodes used

---

## 

Common Use Cases

- **Product photography** - Transform product shots into lifestyle imagery
 
- **Ad creation** - Generate multiple ad variations from a single product image
 
- **Video production** - Convert static images into animated video content
 
- **Brand assets** - Create consistent branded materials from reference images
 
- **Social content** - Produce platform-optimized content from source materials
 
- **Concept exploration** - Quickly test creative directions without manual setup
 

---

## 

App Mode

Techniques can also be run outside of the canvas using App Mode. This provides a streamlined, focused interface where you simply provide inputs and run the technique—no canvas setup required. App Mode is ideal for quick, repeated use of your favorite techniques without the overhead of managing a full project.

---

## 

Technique Builder

Technique Builder lets you package any multi-step workflow on your canvas into a reusable Technique — define inputs, define outputs, and publish. You can also edit published Techniques to update their workflow, inputs, outputs, or listing details.

For the full guide on creating, editing, and publishing your own Techniques, see [**Technique Builder**](https://docs.flora.ai/nodes/technique-builder).

[PreviousRouter Node](https://docs.flora.ai/nodes/router-node) [NextTechnique Builder](https://docs.flora.ai/nodes/technique-builder)

Last updated 1 month ago

Was this helpful?