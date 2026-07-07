# Source: https://docs.flora.ai/models/image-models/gpt-image-by-openai

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/gpt-image-by-openai.md).

### 

**Overview**

Multimodal image generation and editing powered by API.

---

### 

**Quick facts**

- **Modes:** Text → Image · Image → Image (editing)
 
- **Default output / size:** 1024×1024 (auto)
 
- **Aspect ratios:** Auto, 3:2, 1:1, 2:3
 

---

### 

**What it’s great for**

- Photoreal and stylized image generation integrated with LLM workflows.
 
- Simple image edits and inpainting.
 

---

### 

**Example outputs**

Generated hero image — cinematic portrait

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FBwo3IgL8sgYgZUvmCVI5%252FFLORA-Model%2520Cards-017efa42.png%3Falt%3Dmedia%26token%3De6ec8a7f-e92d-4028-9fb7-802dac3402b6&width=768&dpr=3&quality=100&sign=231794a4&sv=2)

Photoreal render

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FKNn6oT2zJ1IpRvjSd6ey%252FFLORA-Model%2520Cards-b0d9eecd.png%3Falt%3Dmedia%26token%3D0c68a7ee-a2ee-4ef7-b427-dd393f5e90c5&width=768&dpr=3&quality=100&sign=fea2ba5a&sv=2)

Edited photo example — background swap

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fpxt5YEsreOjCk3hkUD2J%252Fimage.png%3Falt%3Dmedia%26token%3D50eac59a-3ce5-4fa8-8712-52529ead2feb&width=768&dpr=3&quality=100&sign=988886b5&sv=2)

#### 

**Copy-and-paste prompts**

AskCopy

```
Cinematic street portrait, 50mm lens feel, golden hour, shallow depth of field — 1:1
```

AskCopy

```
Edit: replace background with moody studio backdrop, natural skin tones preserved
```

AskCopy

```
Product pack shot on white, crisp shadows, 1200x1200
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

Required

`Aspect Ratio`

Select

Auto

Auto, 3:2, 1:1, 2:3

`Quality`

Select

High

Low, Medium, High

`Image`

Upload

—

Required for edits

---

### 

**Modes (summary)**

Mode

Estimated time

Required inputs

Typical use

Text → Image

45 seconds

Prompt

Image generation

Image → Image (edit)

1 minute

Image, Prompt

Inpainting & edits

---

### 

**Output options**

Option

Values / notes

Aspect ratio

Auto, 3:2, 1:1, 2:3

---

### 

**Prompt tips**

- Specify composition, lens feel, lighting, and desired ratio.
 
- Use “Edit:” to indicate local edits vs full generation.
 

[PreviousFlux Dev (by Black Forest Labs)](https://docs.flora.ai/models/image-models/flux-dev-by-black-forest-labs) [NextNano Banana (Gemini 2.5 Flash Image) (by Google)](https://docs.flora.ai/models/image-models/nano-banana-gemini-2.5-flash-image-by-google)

Last updated 1 month ago

Was this helpful?