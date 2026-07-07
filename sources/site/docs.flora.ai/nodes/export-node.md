# Source: https://docs.flora.ai/nodes/export-node

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/export-node.md).

The Export Node is your output destination on the canvas. It lets you download generated images, videos, and audio in multiple formats, or push them directly to Google Drive -- all without leaving FLORA.

## 

Overview

Every generation node on the canvas already has a download button in its toolbar, but the Export Node gives you a dedicated, persistent place to:

- **Download media** in your preferred format (PNG, JPG, MP4, MOV, GIF, and more)
 
- **Export to Google Drive** with a one-click connection to any folder in your Drive
 
- **Batch-export outputs** when multiple items are wired in
 

Think of it as the final stop in your workflow -- wire any node's output into the Export Node to save or sync it externally.

---

## 

Getting Started

### 

Adding an Export Node

1

**Open the Add Node Menu**

Press the **+** button or use the canvas shortcut to open the node menu. Under the **Utilities** section, click **Export**. You can also drag from any node's output handle onto empty canvas — the Export node appears in the quick-add picker.

2

**Place It on the Canvas**

The Export Node appears as a gold-bordered block with an upload icon. It starts empty with the prompt: "Wire any node into here to save its outputs."

3

**Connect an Upstream Node**

Drag a connection from any generation node (Image, Video, Audio, or Text) to the Export Node. When that node produces output, it becomes available for export.

---

## 

Downloading Media

Every generation node on the canvas includes a **Download** button in its hover toolbar. Clicking it opens a format dropdown so you can choose the output format before downloading.

### 

Image Formats

Format

Description

**PNG**

Lossless format, best for sharp graphics

**JPG**

Compressed format, smaller file size

**WEBP**

Modern web format, good quality-to-size ratio

**SVG**

Vector format (transcoded from raster via AI)

If the source image is already an SVG, SVG appears first in the format list.

### 

Video Formats

Format

Description

**Original**

Download in the original generated format

**MP4 (h264)**

Widely compatible, great for sharing

**MP4 (h265)**

Better compression, smaller files

**MOV (h264)**

Apple-compatible container with h264 encoding

**MOV (ProRes)**

Professional editing format, high quality

**GIF**

Animated image format, great for short loops

### 

Audio Formats

Audio nodes download in their original format. Supported formats include **MP3**, **M4A**, **WAV**, **AAC**, **OGG**, and **FLAC**. The download preserves whichever format the audio was generated or uploaded in.

### 

Keyboard Shortcuts

When the download dropdown is open, press a number key (**1**, **2**, **3**, etc.) to quickly select the corresponding format without clicking.

### 

Bulk Download

When a node has multiple items in its generation history, a **Download All** button appears in the toolbar. This bundles all history items into a single ZIP file.

---

## 

Exporting to Google Drive

The Export Node supports direct export to Google Drive. Once connected, your generated media is uploaded to a chosen Drive folder automatically.

### 

Connecting Google Drive

1

**Click "Connect to Google Drive"**

On a new Export Node, click the gold **Connect to Google Drive** button. This initiates an OAuth sign-in flow.

2

**Authorize FLORA**

A Google sign-in window opens. Grant FLORA permission to access your Google Drive.

3

**Pick a Destination Folder**

After authorization, a Google Drive folder picker opens. Browse your Drive with proper folder navigation — folders appear grouped before files and can be traversed into. You can choose any folder from **My Drive** or from **Shared Drives** (accessible via a dedicated tab). Click **Select** to confirm.

4

**Done**

The Export Node updates to show the connected folder name. The node icon switches to the Google Drive logo.

### 

Shared Drives

Google Shared Drives (formerly Team Drives) are fully supported for both import and export. When browsing for a destination folder, switch to the **Shared Drives** tab to see all shared drives your Google account has access to. You can navigate into nested folders within a shared drive and select any folder as your export destination.

### 

Managing the Destination

Once connected, hover over the Export Node to reveal the toolbar. Click the **folder dropdown** to:

- **Change folder** -- Open the folder picker again to select a different destination
 
- **Clear destination** -- Remove the Drive connection entirely
 

The dropdown also displays the connected Google account email for reference.

### 

How Drive Export Works

When media is exported to Google Drive:

1. FLORA streams the file directly from its CDN to your Drive folder
 
2. Multiple files are uploaded with bounded concurrency (up to 4 simultaneous uploads)
 
3. Each file is uploaded independently -- if one fails, the others still complete
 
4. A progress bar tracks real-time upload progress with byte-level accuracy
 
5. A toast notification shows progress and confirms when the export is complete, with a direct **Open in Drive** link
 

### 

Export Node Toolbar

Hover over a connected Export Node to access quick actions from the toolbar dropdown:

- **Open in Drive** -- Jump directly to the connected Drive folder
 
- **Disconnect** -- Remove the Drive connection
 

When exporting across batch runs, FLORA automatically deduplicates filenames to prevent overwriting previous exports in the same Drive folder.

---

## 

Importing from Google Drive

FLORA also supports importing files from Google Drive directly onto your canvas.

### 

How to Import

1

**Open the Integrations Panel**

Access the Google Drive tab from the integrations panel in the sidebar.

2

**Connect Your Account**

If you haven't already, connect your Google account via OAuth. The same account used for export can be reused for import.

3

**Browse and Select Files**

Click **Import** to open the Google Drive file picker. Browse or search your Drive, then select the files you want to bring onto your canvas.

4

**Files Appear on Canvas**

Selected files are imported and placed onto your canvas as source nodes, ready to be connected to generation nodes, techniques, or other workflow steps.

---

## 

Importing from Google Drive

In addition to exporting, FLORA supports importing files directly from Google Drive into your workspace.

### 

How to Import

1. Open the **Library** panel from the toolbar
 
2. Select the **Google Drive** tab
 
3. Browse or search your Drive for files to import
 
4. Select the files you want and click **Import**
 

Imported files go through FLORA's standard upload pipeline and appear as assets in your workspace, ready to use on the canvas.

### 

Managing Imported Files

Hover over any imported Drive asset to access management actions:

- **Rename** — Change the asset's display name in FLORA
 
- **Download** — Save a local copy of the file
 
- **Delete** — Remove the imported asset from your workspace
 

### 

Background Processing

Drive imports continue running in the background even after you close the Library panel. A toast notification confirms when each batch of imports is complete, so you can keep working on the canvas while files are being imported.

---

## 

How It Fits Into Workflows

The Export Node is a **terminal node** -- it has inputs but no outputs. It sits at the end of your workflow chain.

### 

Basic Workflow

AskCopy

```
[Text Prompt] --> [Image Node] --> [Export Node: Google Drive]
```

Generate an image and automatically push it to your Drive.

### 

Multi-Step Workflow

AskCopy

```
[Image Upload] --> [Image Node: Upscale] --> [Color Grade Action] --> [Export Node]
```

Upscale, color-grade, and export in one connected pipeline.

---

## 

Tips

- **Name your Export Nodes** -- Click the label at the top of the node to rename it. This helps when you have multiple export destinations in one project.
 
- **Test with one file first** -- Verify your Drive connection and folder selection work before running a large batch export.
 
- **Use the context menu** -- Right-click any node with output and select **Export to Drive** for a quick one-off export without placing an Export Node.
 

---

## 

Limitations

Limitation

Details

Google Drive only

Google Drive is the only supported external destination for both import and export

Terminal node

The Export Node has no outputs -- it cannot feed into other nodes

Not available in Techniques

Export Nodes cannot be used inside Technique workflows

Requires integration feature

Google Drive export requires the integrations feature to be enabled for your workspace

[PreviousBatch Node](https://docs.flora.ai/nodes/batch-node) [NextRouter Node](https://docs.flora.ai/nodes/router-node)

Last updated 1 month ago

Was this helpful?