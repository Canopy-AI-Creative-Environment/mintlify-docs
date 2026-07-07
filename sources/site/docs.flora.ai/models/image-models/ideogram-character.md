# Source: https://docs.flora.ai/models/image-models/ideogram-character

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/ideogram-character.md).

### 

**Overview**

Character consistency and face swapping with reference images.

---

### 

**Quick facts**

- **Modes:** Image → Image · Images → Image
 
- **Default output / size:** 1024×1024 (Auto/1:1)
 
- **Aspect ratios:** Auto, 3:1, 16:10, 16:9, 3:2, 4:3, 1:1, 3:4, 2:3, 9:16, 10:16, 1:3
 

---

### 

**What it's great for**

- Maintaining character consistency across generations
 
- Face swapping with reference images
 
- Character-driven creative projects
 
- Consistent character appearances in different scenes
 

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

`Reference Image(s)`

Upload

—

1-2 images (1 for editing, 2 for face swap)

`Aspect Ratio`

Dropdown

Auto

Auto, 3:1, 16:10, 16:9, 3:2, 4:3, 1:1, 3:4, 2:3, 9:16, 10:16, 1:3

`Mode`

Dropdown

Auto

Auto, Fiction, Realistic

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

Image → Image

~18s

Prompt, Image

Character consistency

Images → Image

~18s

Prompt, 2 Images

Face swapping

---

### 

**Output options**

Option

Values / notes

Aspect ratio

Auto, 3:1, 16:10, 16:9, 3:2, 4:3, 1:1, 3:4, 2:3, 9:16, 10:16, 1:3

---

### 

**Prompt tips**

- Use reference images to maintain character consistency
 
- For face swapping, provide input image first, character reference second
 
- Style Type affects realism vs stylization
 

---

### 

**Safety**

Text moderation is applied according to platform rules — avoid disallowed content.

---

[PreviousIdeogram 3.0](https://docs.flora.ai/models/image-models/ideogram-3.0) [NextLuma Photon](https://docs.flora.ai/models/image-models/luma-photon)

Last updated 1 month ago

Was this helpful?