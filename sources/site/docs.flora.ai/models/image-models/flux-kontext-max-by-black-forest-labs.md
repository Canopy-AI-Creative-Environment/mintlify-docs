# Source: https://docs.flora.ai/models/image-models/flux-kontext-max-by-black-forest-labs

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/flux-kontext-max-by-black-forest-labs.md).

### 

**Overview**

High performing text-to-image model with multi-image support and flexible aspect ratios.

---

### 

**Quick facts**

- **Modes:** Text → Image · Image → Image · Images → Image
 
- **Default output / size:** 1024×1024 (1:1)
 
- **Aspect ratios:** 21:9, 16:9, 4:3, 3:2, 1:1, 2:3, 3:4, 9:16, 9:21
 

---

### 

**What it's great for**

- High-quality text-to-image generation with excellent prompt adherence
 
- Multi-image blending and composition tasks
 
- Image editing with reference images
 
- Creative workflows requiring diverse aspect ratios
 

---

### 

Parameters

Control

Type

Default

Notes

`Prompt`

Text

—

Natural-language instruction (required)

`Aspect Ratio`

Dropdown

1:1

21:9, 16:9, 4:3, 3:2, 1:1, 2:3, 3:4, 9:16, 9:21 (auto for image inputs)

`Seed`

Number

Random

Optional for repeatable results

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Text → Image

~8s

Prompt

Generate images from text

Image → Image

~8s

Prompt, Image

Edit or transform images

Images → Image

~8s

Prompt, Images

Blend up to 5 images

---

### 

**Output options**

Option

Values / notes

Aspect ratio

21:9, 16:9, 4:3, 3:2, 1:1, 2:3, 3:4, 9:16, 9:21

---

### 

**Prompt tips**

- Use specific style descriptors for better results
 
- Seed values enable reproducible outputs
 
- For multi-image blending, describe the desired composition clearly
 

---

### 

**Safety**

Text moderation is applied according to platform rules — avoid disallowed content.

---

[PreviousTopaz](https://docs.flora.ai/models/image-models/topaz) [NextFlux Pro (by Black Forest Labs)](https://docs.flora.ai/models/image-models/flux-pro-by-black-forest-labs)

Last updated 1 month ago

Was this helpful?