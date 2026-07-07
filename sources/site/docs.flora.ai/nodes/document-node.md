# Source: https://docs.flora.ai/nodes/document-node

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/document-node.md).

The Document Node brings PDFs onto your FLORA canvas as a first-class citizen. Drop in a research paper, a brand book, a script, or a slide deck — every page becomes browsable and ready to feed the rest of your workflow.

## 

Capabilities

- **Drop a PDF, get a node.** Drag any PDF onto the canvas (or pick one from the Add menu → Upload). FLORA renders the first page instantly via an in-browser preview while the document uploads in the background.
 
- **Page-by-page navigation.** Multi-page PDFs gain a thumbnail carousel below the node. Click any page to jump to it, or use the arrow keys when the node is selected.
 
- **Full-screen reader.** Open the document in a focused viewer to read full pages, select text, and right-click any selection to spawn it as a new text node.
 
- **Document and image outputs.** Connect a document node to a text node to pass the full document as context, or to an image node to use the currently-open page as visual input.
 
- **Drag-out pages.** Drag any page thumbnail from the carousel onto the canvas to extract it as a new single-page document node — useful for isolating one figure or one slide and wiring it independently.
 
- **Sharing and library.** Document nodes participate in share links, view-only sessions, and the Asset Library just like any other media node.
 

## 

Connections

- **Text nodes** — the full document is passed as context to the downstream model.
 
- **Image nodes** — the currently-open page is used as visual input. Navigate pages on the document node to change which page is sent downstream.
 
- **Batch nodes** — process every page in parallel through whatever pipeline you wire downstream.
 

Even more connectivity is coming soon! If you have thoughts, comments, or suggestions, please let us know.

## 

See also

- [PDF to Text](https://docs.flora.ai/nodes/document-node/pdf-to-text) — wiring documents into text workflows.
 
- [PDF to Image](https://docs.flora.ai/nodes/document-node/pdf-to-image) — using the current page as image input.
 

[PreviousText to Audio](https://docs.flora.ai/nodes/audio-node/text-to-video) [NextPDF to Text](https://docs.flora.ai/nodes/document-node/pdf-to-text)

Last updated 1 month ago

Was this helpful?