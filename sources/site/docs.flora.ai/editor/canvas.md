# Source: https://docs.flora.ai/editor/canvas

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/editor/canvas.md).

## 

Summary

FLORA's canvas is your creative garden. You can spawn nodes, connect nodes, edit parameters, and create your own personalized workflows.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FdksYM1KwDgks4JSR005L%252FEditor.png%3Falt%3Dmedia%26token%3Dc679da60-b304-4637-9957-0a5c9cd4be11&width=768&dpr=3&quality=100&sign=55b9eeb1&sv=2)

## 

Getting Started

There are many ways to start populating the canvas with your creative thoughts.

Simply **Double-Click** to spawn a node or click on any of the selected workflows to start.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FcQDOx8l4w0iS3zEtiXhK%252FEditor.gif%3Falt%3Dmedia%26token%3D302dd9da-12c1-493b-9c3f-f9de90b910be&width=768&dpr=3&quality=100&sign=3318cc86&sv=2)

## 

Connecting Nodes

FLORA brings over 50+ text, image, and video models to one canvas, saving you time and effort in context- and tool-switching. With this approach, you can connect nodes of different modalities, using our open-ended canvas to ideate, explore different creative directions, compare models and prompts, and more.

To connect a node, simply drag the '+' handle from a node that's on the canvas.

Here are **just a couple** of example use cases of connecting nodes:

- **Text node to image node:** Connect the output of a text node to the input of an image node.
 
- **Image node to video node:** Connect one or multiple image nodes to a video node as a reference frame (depending on the model, can be first frame, last frame, or both).
 

As AI model capabilities advance, the number of possibilities around combining text / image / video nodes expands.

## 

Color Tagging

You can assign color tags to nodes to visually organize your canvas. Color tags appear as colored highlights on nodes, making it easy to group related content by theme, status, or any system that works for your workflow.

### 

Tagging individual nodes

Select a node and use the **color tag** option in the node toolbar to assign a color.

### 

Tagging multiple nodes at once

Select multiple nodes on your canvas (drag-select or Shift+click), and the **multi-selection toolbar** will appear with a color tag picker. Choose a color to apply it to all selected nodes simultaneously — useful for quickly categorizing batches of nodes.

## 

Bulk Parameter Editing

When you select **two or more blocks of the same type and mode** on the canvas (e.g., two image generation blocks both using the same modality), a **Bulk Parameters Panel** appears in the right sidebar. This lets you edit shared parameters across all selected blocks at once — no need to update each block individually.

- **Shared parameters only** — The panel shows only the parameters that exist on every selected block. Parameters unique to a single block are not shown.
 
- **Mixed values** — When selected blocks have different values for a parameter, the field shows a "Mixed" indicator. Editing the field applies the new value to all selected blocks.
 
- **Model selector** — If the selected blocks share compatible models, you can switch models for all of them at once from the bulk panel.
 

This is especially useful when you want to apply consistent settings (seed, guidance, aspect ratio, etc.) across multiple blocks in a comparison or batch workflow.

### 

Reordering Connected Inputs

When a node has multiple connected inputs — such as several images wired into a generation node, or multiple text inputs on an Action node — you can **drag to reorder** them. Grab any connected input and drag it up or down to change the order in which inputs are processed.

### 

Wiring In-Progress Nodes

You can connect nodes that are still processing (such as a Document node that hasn't finished extracting text yet) to downstream nodes. FLORA validates readiness at generation time, not at connection time — so you can build your workflow while earlier steps are still running.

[PreviousEditor](https://docs.flora.ai/editor/editor) [NextToolbar](https://docs.flora.ai/editor/toolbar)

Last updated 1 month ago

Was this helpful?