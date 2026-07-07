# Source: https://docs.flora.ai/models/image-models/seedream-4.0-by-bytedance

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/seedream-4.0-by-bytedance.md).

### 

**Overview**

Consistent, reasoning-driven text→image model with high-resolution outputs.

---

### 

**Quick facts**

- **Modes:** Text → Image · Image → Image (editing)
 
- **Outputs / sizes:** 1024×1024 (1:1), 1280×720 (16:9), 720×1280 (9:16) — higher when selecting 2K/4K
 
- **Aspect ratios:** 21:9, 16:9, 4:3, 3:2, 1:1, 2:3, 3:4, 9:16, 9:21
 

---

### 

**What it’s great for**

- High-detail photoreal images and editorial art.
 
- High-resolution asset prototyping.
 
- Image editing and inpainting tasks.
 

---

### 

**Example outputs**

Shadow study — experimental fashion film still

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FkCG5vaM733tIm5DtUCXs%252Fimage.png%3Falt%3Dmedia%26token%3D813ddd94-067a-4386-854b-5cbd771f38c6&width=768&dpr=3&quality=100&sign=bff368b3&sv=2)

Cinematic character moment

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FQ3EggAcqKPBEcooXoyhd%252Fimage.png%3Falt%3Dmedia%26token%3D49d170b3-5acb-4c43-8499-2eb1b1feb5a3&width=768&dpr=3&quality=100&sign=c74f60f9&sv=2)

Detailed environment concept

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Ft9Kq8RV4vFkznzI55yOv%252Fimage.png%3Falt%3Dmedia%26token%3Da43e284f-6480-4c08-815e-6965ed2473fd&width=768&dpr=3&quality=100&sign=56bd7879&sv=2)

#### 

**Copy-and-paste prompts**

AskCopy

```
Experimental fashion film still of a blurred shadow silhouette of a figure with long hair reaching out a hand. The body is partially obscured by tree leaf shadows cast on a white wall, captured in soft diffusion. An interior bedroom wall is bathed in hard daylight, with high-contrast backlight forming abstract silhouettes. Shot on 16mm film with a wide lens, extreme close-up low angle composition, desaturated color palette with subtle grain. The mood is hypnotic, dreamlike, and intimate, evoking trance-like disorientation and fragile presence.
```

AskCopy

```
Cool desaturated digital cinematography, a middle-aged Japanese man in a grey t-shirt brushes his teeth at a stainless steel sink. A towel hangs behind him, toothbrush in mouth, framed in a narrow Tokyo apartment bathroom. Artificial fluorescent side light casts cyan tones across metal surfaces, mixing with warm glow from a frosted glass window. Shot on Sony VENICE 2 with Canon K35 wide lens, medium wide clean single, centered composition, naturalistic production design with water heater and simple domestic objects. The mood is intimate and contemplative, evoking solitude and the quiet poetry of daily ritual.
```

AskCopy

```
Cinematic landscape film still of furrowed rows of young green crops, vast open field stretching to the horizon. Golden-hour sunset on the right edge throws long shadows and warm amber flare across desaturated earth tones and cool greens. Wide lens, very low ground-level angle with strong leading lines converging toward the sun, deep depth of field. Subtle 16mm grain, gentle halation around the sun, soft vignette. Sky in pastel lavender and peach, horizon thin and distant, mood contemplative, tender, and quietly transcendent, evoking rest after labor and a meditative union with the landscape.
```

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

Used for edits and variations

`Size`

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

---

### 

**Output options**

Option

Values / notes

Aspect ratio

Square (1:1), Landscape (16:9), Portrait (9:16)

Resolution

2048×2048 (Square), 2048×1152 (Landscape), 1152×2048 (Portrait)

---

### 

**Prompt tips**

- Use photographic tokens for realism.
 

---

[PreviousNano Banana (Gemini 2.5 Flash Image) (by Google)](https://docs.flora.ai/models/image-models/nano-banana-gemini-2.5-flash-image-by-google) [NextSeedream 4.5 (by Bytedance)](https://docs.flora.ai/models/image-models/seedream-4.5-by-bytedance)

Last updated 1 month ago

Was this helpful?