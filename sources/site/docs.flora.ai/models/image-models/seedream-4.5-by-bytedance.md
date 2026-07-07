# Source: https://docs.flora.ai/models/image-models/seedream-4.5-by-bytedance

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/seedream-4.5-by-bytedance.md).

### 

**Overview**

A new-generation image creation model with enhanced quality and multi-image blending capabilities.

---

### 

**Quick facts**

- **Modes:** Text → Image · Image → Image (editing) · Images → Image (multi-image blend)
 
- **Outputs / sizes:** 1024×1024 (1:1), 1280×720 (16:9), 720×1280 (9:16) — higher when selecting 2K/4K
 
- **Aspect ratios:** 21:9, 16:9, 4:3, 3:2, 1:1, 2:3, 3:4, 9:16, 9:21
 

---

### 

**What it's great for**

- High-quality photoreal images with improved generation fidelity.
 
- Multi-image blending and composition (up to 10 input images).
 
- Image editing, inpainting, and style transfer tasks.
 
- High-resolution 4K asset creation.
 

---

### 

**Parameters (editor-ready)**

Name

Type

Default

Notes

`Prompt`

Text

—

Required

`Reference Image`

Upload

Optional

Used for edits and variations (up to 10 images for multi-image mode)

`Aspect Ratio`

Select

Square (1:1)

Square (1:1), Landscape (16:9), Landscape (4:3), Landscape (3:2), Portrait (2:3), Portrait (3:4), Portrait (9:16), Ultra-wide (21:9), Tall (9:21)

`Resolution`

Select

2K

2K, 4K

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Text → Image

~25 seconds

Prompt

High-resolution generation

Image → Image

~25 seconds

Reference Image, Prompt

Inpainting & edits

Images → Image

~25 seconds

Multiple Images, Prompt

Multi-image blending & composition

---

### 

**Output options**

Option

Values / notes

Aspect ratio

Square (1:1), Landscape (16:9), Portrait (9:16), and more

Resolution

2048×2048 (Square), 2048×1152 (Landscape), 1152×2048 (Portrait)

---

### 

**Prompt tips**

- Use photographic tokens for realism.
 
- Describe lighting, camera angles, and mood for cinematic results.
 
- For multi-image blending, describe how elements should combine in your prompt.
 

---

[PreviousSeedream 4.0 (by Bytedance)](https://docs.flora.ai/models/image-models/seedream-4.0-by-bytedance) [NextMagnific Upscaler & Enhancer](https://docs.flora.ai/models/image-models/magnific-upscaler-and-enhancer)

Last updated 1 month ago

Was this helpful?