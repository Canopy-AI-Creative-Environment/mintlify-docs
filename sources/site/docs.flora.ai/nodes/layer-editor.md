# Source: https://docs.flora.ai/nodes/layer-editor

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/layer-editor.md).

The Layer Editor is a powerful compositing tool that lets you combine multiple images into a single layered composition. It provides a canvas-based editing environment similar to professional design tools, enabling precise control over positioning, sizing, and layering of visual elements.

## 

Overview

The Layer Editor transforms a node into a full-featured composition workspace where you can:

- **Combine multiple images** from different sources into one composition
 
- **Precisely position and transform** each layer independently
 
- **Control layer ordering** to create depth and visual hierarchy
 
- **Export the final composition** as a single unified image
 

This is ideal for creating collages, mood boards, social media graphics, or any project that requires combining multiple visual elements.

---

## 

Getting Started

### 

Adding a Layer Editor Node

1

**Add the Node**

From the node menu, select **Layer Editor** to add it to your canvas.

2

**Connect Source Images**

Connect image nodes, video frames, or other visual sources to the Layer Editor. Each connected source becomes a layer in your composition.

3

**Enter Edit Mode**

**Double-click** the Layer Editor node, or click **Layer Editor** in the node toolbar to activate the editing interface. The canvas becomes interactive, displaying all your layers and editing controls.

---

## 

Working with Layers

### 

The Layers Panel

The Layers Panel on the side of the editor displays all layers in your composition. Layers are listed from top to bottom, with the topmost layer in the list appearing in front of other layers on the canvas.

**Layer controls include:**

- **Visibility toggle** - Show or hide individual layers
 
- **Lock toggle** - Prevent accidental edits to a layer
 
- **Layer name** - Click to rename for better organization
 
- **Reorder** - Drag layers up or down to change their stacking order
 

### 

Selecting Layers

- **Single click** on a layer in the canvas or panel to select it
 
- **Ctrl/Cmd + Click** to toggle selection and select multiple layers
 
- **Click empty canvas space** to deselect all layers
 

---

## 

Transforming Layers

### 

Moving Layers

- **Drag** any selected layer to reposition it on the canvas
 
- **Arrow keys** nudge the layer by 1 pixel
 
- **Shift + Arrow keys** nudge by 10 pixels for faster movement
 

### 

Resizing Layers

Click a layer to reveal the transform handles:

- **Corner handles** - Resize while maintaining aspect ratio
 
- **Edge handles** - Resize in one direction only
 
- **Double-click** a layer to automatically fit it to the canvas frame
 

Hold **Shift** while resizing to toggle aspect ratio lock on or off.

### 

Rotating Layers

Hover near a corner handle to see the rotation cursor. Click and drag to rotate the layer freely.

### 

Flipping Layers

Use the transform actions panel to:

- **Flip Horizontal** - Mirror the layer left-to-right
 
- **Flip Vertical** - Mirror the layer top-to-bottom
 

---

## 

Layer Alignment

The alignment toolbar provides quick alignment options for selected layers:

Button

Action

Align Left

Align layer to the left edge of the canvas

Align Right

Align layer to the right edge of the canvas

Center H

Center layer horizontally on the canvas

Align Top

Align layer to the top edge of the canvas

Align Bottom

Align layer to the bottom edge of the canvas

Center V

Center layer vertically on the canvas

Center All

Center layer both horizontally and vertically

---

## 

Layer Ordering

Control which layers appear in front of others:

### 

Using the Context Menu

Right-click a layer to access ordering options:

- **Send to Top** - Move layer to the front of all others
 
- **Send to Bottom** - Move layer behind all others
 
- **Send Up** - Move layer one position forward
 
- **Send Down** - Move layer one position backward
 

### 

Keyboard Shortcuts

Action

Shortcut

Send Up

`Cmd/Ctrl + ]`

Send Down

`Cmd/Ctrl + [`

### 

Drag Reordering

In the Layers Panel, drag layers up or down to change their stacking order visually.

---

## 

Appearance Controls

### 

Opacity

Adjust layer transparency using the opacity slider in the Appearance Panel:

- **100%** - Fully opaque (default)
 
- **0%** - Fully transparent
 

Changes preview in real-time as you adjust the slider.

---

## 

Canvas Settings

### 

Frame Size

The Layer Editor uses a compositor frame that defines the output dimensions:

- **Default size**: 2048 × 2048 pixels
 
- **Maximum size**: 4096 × 4096 pixels
 
- **Minimum size**: 100 × 100 pixels
 

### 

Snap to Grid

Enable snap-to-grid for precise alignment. When enabled, layers snap to nearby edges and center points as you move them.

---

## 

Keyboard Shortcuts

Action

Shortcut

Delete selected layer

`Delete` or `Backspace`

Undo

`Cmd/Ctrl + Z`

Redo

`Cmd/Ctrl + Shift + Z`

Nudge 1px

Arrow keys

Nudge 10px

`Shift + Arrow keys`

Send layer up

`Cmd/Ctrl + ]`

Send layer down

`Cmd/Ctrl + [`

---

## 

Generating Output

When you're satisfied with your composition:

1. All visible layers are automatically composited together
 
2. The Layer Editor generates a preview image
 
3. Connect the Layer Editor output to other nodes for further processing
 

The compositor combines only **visible** layers. Toggle layer visibility to exclude layers from the final output without deleting them.

---

## 

Tips for Better Compositions

- **Lock finished layers** to prevent accidentally moving them while working on others
 
- **Name your layers** descriptively to stay organized in complex compositions
 
- **Use alignment tools** for professional, balanced layouts
 
- **Work with the snap-to-grid** feature enabled for precise positioning
 
- **Undo liberally** - the Layer Editor maintains a history of up to 50 changes
 

---

## 

Common Use Cases

- **Social media graphics** - Combine multiple product photos into polished layouts
 
- **Mood boards** - Arrange multiple reference images in one composition
 
- **Collages** - Create artistic arrangements of generated images
 
- **Presentations** - Layer diagrams and screenshots together
 
- **Before/after comparisons** - Position related images side by side
 

[PreviousPDF to Image](https://docs.flora.ai/nodes/document-node/pdf-to-image) [NextAction Node](https://docs.flora.ai/nodes/action-node)

Last updated 1 month ago

Was this helpful?