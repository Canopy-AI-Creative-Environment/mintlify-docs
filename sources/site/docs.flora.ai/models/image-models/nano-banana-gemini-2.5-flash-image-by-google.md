# Source: https://docs.flora.ai/models/image-models/nano-banana-gemini-2.5-flash-image-by-google

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/nano-banana-gemini-2.5-flash-image-by-google.md).

## 

**Overview**

High-fidelity image generation and editing (photo-real & stylized) — fast, edit-first workflows.

---

### 

**Quick facts**

- **Modes:** Text → Image · Image → Image (editing) · Images → Image.
 
- **Default output / size:** 1024×1024 (Square)
 
- **Aspect ratios:** Square, Landscape, Portrait (determined by input image)
 

---

### 

**What it’s great for**

- Fast photo edits and stylized generation.
 
- Turning photos into collectible / toy-style renders.
 
- Multi-image fusion and targeted local edits.
 

---

### 

**Example outputs**

Hero portrait — edited photo to collectible render

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FMD7iIK9rzUd9jxc1bH0Z%252FFLORA-Untitled-7e0ce566.png%3Falt%3Dmedia%26token%3D84727e2c-cda3-41d1-aba8-74c9641422b7&width=768&dpr=3&quality=100&sign=bc52d615&sv=2)

Stylized figurine render

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FRUJjXAYnrmmvaOsGIDX3%252FFLORA-Untitled-e0c926b2.png%3Falt%3Dmedia%26token%3D6c42e0e2-5ffe-4c2f-ba45-8d72368b263e&width=768&dpr=3&quality=100&sign=b48f257a&sv=2)

Multi-image fusion composite

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FNKnTGIKRfdqqDZnQnQud%252FFLORA-Untitled-ef35b1a0.png%3Falt%3Dmedia%26token%3Dfd42ce3e-d4b8-4519-9647-93086ecd94e5&width=768&dpr=3&quality=100&sign=3e976e3a&sv=2)

#### 

**Copy-and-paste prompts**

AskCopy

```
Portrait photo retouched into collectible 3D figurine on acrylic base, studio lighting, crisp detail
```

AskCopy

```
Edit: remove background and add dramatic rim light, maintain subject skin tones, photoreal
```

AskCopy

```
Blend two product images into a single shelf display with natural shadows and reflections
```

---

### 

**Parameters**

Name

Type

Default

Notes

`Prompt`

Text

—

Natural-language description (required)

`Reference Image`

Image

—

Required for edits / multi-image fusion

`Aspect Ratio`

Inherited

Square

Determined by input reference image aspect ratio

---

### 

**Modes (summary)**

Mode

Estimated time

Required inputs

Typical use

Text → Image

20 seconds

Prompt

Generate images from text

Image → Image (edit)

30 seconds

Reference Image, Prompt

Local edits, background replacement

Images → Image

30 seconds

Reference Images, Prompt

Multi-image fusion / composites

---

### 

**Prompt tips**

- For edits prefix with “Edit:” and describe pixel-accurate changes.
 
- Use clear style tokens (e.g., “photoreal”, “3D figurine”, “studio lighting”).
 

---

[PreviousGPT-Image (by OpenAI)](https://docs.flora.ai/models/image-models/gpt-image-by-openai) [NextSeedream 4.0 (by Bytedance)](https://docs.flora.ai/models/image-models/seedream-4.0-by-bytedance)

Last updated 1 month ago

Was this helpful?