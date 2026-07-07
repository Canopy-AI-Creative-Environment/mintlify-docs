# Source: https://docs.flora.ai/models/image-models/flux-redux-by-black-forest-labs

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/flux-redux-by-black-forest-labs.md).

### 

**Overview**

Image variation model for slight modifications of input images.

---

### 

**Quick facts**

- **Modes:** Image → Image
 
- **Default output / size:** Auto (preserves input aspect)
 
- **Aspect ratios:** Auto + multiple resolution options
 

---

### 

**What it's great for**

- Creating subtle variations of existing images
 
- Iterative refinement workflows
 
- Maintaining overall composition while varying details
 
- Quick image alternatives
 

---

### 

Parameters

Control

Type

Default

Notes

`Reference Image`

Upload

—

Input image to vary (required)

`Quality`

Slider

100

0-100

`Size`

Select

Auto

Auto, 16:9, 4:3, 1:1, 3:4, 9:16

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Image → Image

~28s

Image

Image variation

---

### 

**Output options**

Option

Values / notes

Aspect ratio

Auto (preserves input) + multiple aspect ratio options

---

### 

**Prompt tips**

- No prompt required—model creates variations automatically
 
- Lower guidance scale produces more variation
 
- Higher guidance scale stays closer to input
 
- Useful for generating alternatives quickly
 

---

### 

**Safety**

Moderation may be applied according to platform rules — avoid disallowed content.

---

[PreviousFlux Pro (by Black Forest Labs)](https://docs.flora.ai/models/image-models/flux-pro-by-black-forest-labs) [NextIdeogram 3.0](https://docs.flora.ai/models/image-models/ideogram-3.0)

Last updated 1 month ago

Was this helpful?