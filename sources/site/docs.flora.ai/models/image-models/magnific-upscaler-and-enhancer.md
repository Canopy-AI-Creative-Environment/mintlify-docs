# Source: https://docs.flora.ai/models/image-models/magnific-upscaler-and-enhancer

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/magnific-upscaler-and-enhancer.md).

### 

**Overview**

Image upscaler and enhancer for high-detail restoration and creative upscaling.

---

### 

**Quick facts**

- **Modes:** Image → Image (upscale / enhance / transform)
 
- **Default output / size:** Precision 2× (fixed) · Creative 2×–16×
 
- **Aspect ratios:** Preserves input aspect ratio
 
- **Variants:** Precision (detail-first) · Creative (promptable stylization)
 

---

### 

**When to use each model**

- **Magnific Precision:** Best when you must preserve the original look—restoring archival scans, print prep, or broadcast stills where only a 2× upscale is needed. Fine-tune sharpness, grain, and ultra-detail without prompting.
 
- **Magnific Creative:** Choose this when you want to reinterpret the source—concept art, stylized photography, marketing assets, or when you need 4×–16× upscales. Add a prompt, pick an optimization preset, and steer creativity, detail, resemblance, and fractality.
 

---

### 

**What it’s great for**

- Photo upscaling for print and large-format uses.
 
- Enhancing texture, denoise, and creative detail reimagination.
 
- Preparing assets for VFX or large displays.
 

---

### 

**Example outputs**

Low-resolution input sample

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FTSa2FNcizrRkUStwHkEo%252Fimage.png%3Falt%3Dmedia%26token%3De708c9e9-9864-4dc1-94a7-471df2978df5&width=768&dpr=3&quality=100&sign=2c982e0a&sv=2)

Upscaled result — 4× detail restoration

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FLTdcL1etUISF5AopgZB1%252Fimage.png%3Falt%3Dmedia%26token%3De3bb30b0-ffcd-4c8f-b8fa-aab4fb33529a&width=768&dpr=3&quality=100&sign=e81230b6&sv=2)

#### 

**Copy-and-paste prompts**

AskCopy

```
Upscale image to 4x, preserve skin detail, remove JPEG artifacts
```

AskCopy

```
Enhance texture and noise removal for print, keep natural lighting
```

### 

**Parameters**

#### 

**Magnific Precision parameters**

Name

Type

Default

Notes

`Image`

Upload

—

Required input image

`Scale Factor`

Select

2×

Fixed 2× enlargement (API enforces max allowed scale)

`Sharpen`

Slider

50

0–100; higher values accentuate edges but can look artificial

`Smart Grain`

Slider

7

0–100; reintroduces natural texture for photo realism

`Ultra Detail`

Slider

30

0–100; boosts fine structure and clarity

#### 

**Magnific Creative parameters**

Name

Type

Default

Notes

`Prompt`

Text

—

Optional guidance for creative reinterpretation

`Image`

Upload

—

Required input image

`Optimization Preset`

Select

Standard

Standard, Soft Portraits, Hard Portraits, Art & Illustration, Video Game Assets, Nature & Landscapes, Films & Photography, 3D Renders, Sci-Fi & Horror

`Scale Factor`

Select

2×

2×, 4× (2× cost), 8× (4× cost), 16× (8× cost); engine auto-limits if resolution would exceed 10056×10056

`Creativity`

Slider

2

\-10 to 10; higher values introduce more generative edits

`Detail (HDR)`

Slider

6

\-10 to 10; controls definition and micro-contrast

`Resemblance`

Slider

6

\-10 to 10; keeps the output closer to the original when lowered

`Fractality`

Slider

6

\-10 to 10; governs prompt strength and intricate patterns

`Engine`

Select

Auto

Auto, Illusio (illustrations), Sharpy (photos), Sparkle (balanced; reduces JPEG artifacts)

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Image → Image (upscale)

~15 seconds

Image

Upscale for print & detail

Image → Image (enhance)

~15 seconds

Image

Denoise and texture work

---

### 

**Output options**

Option

Values / notes

Scale

Precision: 2× fixed · Creative: 2×, 4×, 8×, 16× (auto-clamped if output would exceed 10056×10056)

Formats

PNG, JPG

Notes

Creative presets: Standard, Soft Portraits, Hard Portraits, Art & Illustration, Video Game Assets, Nature & Landscapes, Films & Photography, 3D Renders, Sci-Fi & Horror

---

### 

**Prompt tips**

- For Precision, start with the base 2× upscale and nudge Sharpen/Ultra Detail carefully—small increments keep it photoreal.
 
- For Creative, pair a succinct prompt with an Optimization preset that matches the content (e.g., Soft Portraits for faces).
 
- Dial Resemblance down if you want a bolder reimagining; push Fractality up only when you need intricate stylized detail.
 

[PreviousSeedream 4.5 (by Bytedance)](https://docs.flora.ai/models/image-models/seedream-4.5-by-bytedance) [NextTopaz](https://docs.flora.ai/models/image-models/topaz)

Last updated 25 days ago

Was this helpful?