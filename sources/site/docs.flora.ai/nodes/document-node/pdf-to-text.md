# Source: https://docs.flora.ai/nodes/document-node/pdf-to-text

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/document-node/pdf-to-text.md).

## 

Summary

There are two ways to get text from a document node into your workflow: wire it to a downstream text node to pass the full document as context, or open the fullscreen reader and select specific text to spawn it as a text node.

## 

How to use

### 

Connect downstream

1. Drop a PDF onto the canvas to create a Document Node.
 
2. Drag a connection from the document node to a Text Node.
 
3. The downstream node receives the full document as context.
 

### 

Extract selected text from fullscreen

1. Click the fullscreen button on the document node to open the focused viewer.
 
2. Select any text on the page.
 
3. Right-click the selection and choose **Create text node** — FLORA spawns a text node on the canvas containing exactly what you selected.
 

## 

Example workflows

- **Research summarizer** — Document Node → Text Node prompted with "Summarize the methodology of this paper in three sentences."
 
- **Brand-voice rewrite** — Document Node (style guide) → Text Node ("Rewrite this draft in the voice and tone described above.")
 
- **Pull a specific quote** — open fullscreen, select the passage, right-click → Create text node, then wire that text node wherever you need it.
 
- **Script breakdown** — Document Node (screenplay) → Batch Node → per-scene Text Node prompted with "Pull out every prop and wardrobe note in this scene."
 

Even more connectivity is coming soon! If you have thoughts, comments, or suggestions, please let us know.

[PreviousDocument Node](https://docs.flora.ai/nodes/document-node) [NextPDF to Image](https://docs.flora.ai/nodes/document-node/pdf-to-image)

Last updated 1 month ago

Was this helpful?