# Source: https://docs.flora.ai/editor/image-editing

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/editor/image-editing.md).

## 

Overview

FLORA provides powerful image editing capabilities that allow you to modify and extend your generated images directly on the canvas. The Image Editor includes two main features:

- **Inpainting**: Paint over areas of an image to regenerate specific regions
 
- **Outpainting**: Expand the canvas beyond the original image boundaries
 

These tools work seamlessly with FLORA's AI generation pipeline, letting you iteratively refine your images without leaving the editor.

---

## 

Inpainting

Inpainting allows you to selectively regenerate portions of an image by painting a mask over the areas you want to change. This is useful for:

- Removing unwanted objects from an image
 
- Replacing specific elements with something new
 
- Fixing imperfections or artifacts
 
- Adding new objects to a scene
 

### 

How to Use Inpainting

1

**Select an Image Node**

Click on an image node that contains a generated or uploaded image.

2

**Activate the Inpaint Tool**

Click the **Inpaint** tool in the image editing toolbar. Your cursor will change to a brush indicator.

3

**Paint the Mask**

Click and drag on the image to paint over the areas you want to regenerate. The painted areas will be highlighted with a green crosshatch pattern.

**Brush Controls:**

- **Brush Size**: Adjust the brush size using the slider in the brush panel (5-100 pixels)
 
- **Undo Strokes**: Press `Ctrl/Cmd + Z` to undo individual brush strokes
 
- **Clear All**: Remove all painted strokes to start over
 

4

**Enter Your Prompt**

In the prompt input that appears below the image, describe what you want to generate in the painted area.

Example prompts:

- "A red sports car" (to replace a vehicle)
 
- "Blue sky with clouds" (to fix the background)
 
- "Remove the object" (to seamlessly blend the area)
 

5

**Generate**

Click the submit button to generate. A new image node will be created with your inpainted result, preserving your original image.

### 

How Inpainting Works

When you submit an inpainting request:

1. **Mask Generation**: Your brush strokes are converted into a mask image that tells the AI which areas to regenerate
 
2. **Composite Creation**: The original image and mask are combined and sent to the selected AI model
 
3. **Generation**: The model generates new content only within the masked regions while preserving the rest of the image
 
4. **Result**: A new image node appears with the inpainted result
 

Different AI models may require different mask formats. FLORA automatically handles this conversion based on the model you've selected.

### 

Tips for Better Inpainting Results

- **Paint generously**: Slightly extend your mask beyond the edges of what you want to change for smoother blending
 
- **Be descriptive**: Provide clear, detailed prompts about what should appear in the masked area
 
- **Consider context**: The AI uses the surrounding image as context, so your prompt should fit naturally with the scene
 
- **Iterate**: If the first result isn't perfect, try adjusting your mask or prompt and generate again
 

### 

Supported Models for Inpainting

Several AI models in FLORA support inpainting:

- **GPT Image 1.5** - Supports advanced mask-based inpainting
 
- **Nano Banana Pro** - Uses outline-based inpainting
 
- **Ideogram** - Creative inpainting capabilities
 

Model availability may vary. Check the model selector for currently available options.

---

## 

Outpainting

Outpainting (also known as canvas expansion) allows you to extend an image beyond its original boundaries. The AI will generate new content that seamlessly continues from the edges of your original image.

### 

How to Use Outpainting

1

**Select an Image Node**

Click on an image node containing the image you want to expand.

2

**Activate the Outpaint Tool**

Click the **Outpaint** tool in the image editing toolbar. Green resize handles will appear around the image.

3

**Expand the Canvas**

Drag the handles to expand the canvas in any direction:

- **Edge handles**: Drag the top, bottom, left, or right edges to expand in one direction
 
- **Corner handles**: Drag corners for diagonal expansion
 

4

**Enter Your Prompt**

In the prompt input that appears, describe what should fill the expanded area. If left empty, FLORA will use "Fill this expanded area" as the default prompt.

Example prompts:

- "Continue the beach scene with palm trees"
 
- "Extend the sky with sunset colors"
 
- "Add more of the forest landscape"
 

5

**Generate**

Click submit to generate. A new image node will appear with your expanded image.

### 

How Outpainting Works

When you submit an outpainting request:

1. **Composite Creation**: FLORA creates a new canvas at the expanded dimensions with your original image positioned in the appropriate location
 
2. **Generation**: The AI model fills in the expanded regions while maintaining visual continuity with your original image
 
3. **Result**: A new node displays the expanded image
 

### 

Tips for Better Outpainting Results

- **Expand gradually**: For very large expansions, consider doing multiple smaller expansions rather than one massive change
 
- **Provide context**: Your prompt should describe what naturally extends from the edges of your image
 
- **Watch the edges**: Pay attention to elements at the edges of your original image—the AI will try to continue them
 
- **Aspect ratio**: Consider your final desired aspect ratio when expanding; you can expand more in one direction than another
 

---

## 

Workflow Tips

### 

Combining Editing Tools

You can use inpainting and outpainting together for powerful workflows:

1. **Generate** an initial image
 
2. **Outpaint** to expand the canvas and add more scene
 
3. **Inpaint** specific areas to refine details or fix artifacts
 
4. **Repeat** as needed to achieve your desired result
 

### 

Preserving Your Work

- Each edit creates a new image node, so your original is always preserved
 
- You can compare results side-by-side on the canvas
 
- Delete nodes you don't need to keep your workspace organized
 

### 

Keyboard Shortcuts

Action

Shortcut

Undo brush stroke

`Ctrl/Cmd + Z`

Cancel generation

Click the cancel button during generation

[PreviousToolbar](https://docs.flora.ai/editor/toolbar) [NextTimeline Editor](https://docs.flora.ai/editor/timeline-editor)

Last updated 1 month ago

Was this helpful?