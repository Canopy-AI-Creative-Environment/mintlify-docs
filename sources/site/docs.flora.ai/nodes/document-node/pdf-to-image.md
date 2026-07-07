# Source: https://docs.flora.ai/nodes/document-node/pdf-to-image

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/document-node/pdf-to-image.md).

## 

Summary

Each page of a Document Node is rendered as an image. Connect a document node to an image node and the currently-open page is passed as visual input — navigate pages on the document node to change what gets sent downstream.

## 

How to use

### 

Connect downstream

1. Drop a PDF onto the canvas.
 
2. Use the page carousel (or arrow keys) to open the page you want to use.
 
3. Drag a connection from the document node to an Image Node
 
4. The downstream node receives the currently-open page as visual context. Switch pages on the document node to swap which page is sent.
 

### 

Drag a page out

1. Hover the page carousel under the document node.
 
2. Grab any thumbnail and drag it onto an empty area of the canvas.
 
3. FLORA extracts that page into a new single-page PDF and creates a new Document Node pointing to it — useful when you want to operate on one figure or one slide independently of the rest of the document.
 

## 

Example workflows

- **Reference-image generation** — Document Node (mood board PDF) → Image Node prompted with "Generate a frame that matches this composition."
 

Even more connectivity is coming soon! If you have thoughts, comments, or suggestions, please let us know.

[PreviousPDF to Text](https://docs.flora.ai/nodes/document-node/pdf-to-text) [NextLayer Editor](https://docs.flora.ai/nodes/layer-editor)

Last updated 1 month ago

Was this helpful?