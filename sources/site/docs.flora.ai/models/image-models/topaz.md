# Source: https://docs.flora.ai/models/image-models/topaz

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/image-models/topaz.md).

## 

**Topaz (Photo & Video enhancement)**

**Professional photo & video enhancement tools for de-noise, de-blur, and upscaling.**

---

### 

**Quick facts**

- **Modes:** Image → Image (upscale / denoise / deblur) · Video → Video (upscaling)
 
- **Default output / size:** Image 2× (range 1×–4×) · Video 2× (range 1×–4×)
 
- **Aspect ratios:** Preserves input aspect ratio (image & video)
 
- **Enhancement presets:** Standard V2, Low Resolution V2, CGI, High Fidelity V2, Text Refine
 

---

### 

**When to use each mode**

- **Topaz Photo (image):** Best for photographers and designers who need artifact-free enlargements, text sharpening, or restoration without touching motion settings.
 
- **Topaz Video:** Use for documentary, broadcast, or archival clips that need 2×–4× upscale or frame-rate adjustments while keeping motion smooth.
 

---

### 

**What it’s great for**

- Photographers and studios preparing images for print.
 
- Restoring and cleaning archival photos/video.
 
- High-quality video upscaling and restoration.
 

---

#### 

**Topaz Tips**

AskCopy

```
Upscale to 2x, remove noise while preserving textures
```

AskCopy

```
Restore scanned photo: remove dust and scratches, sharpen faces
```

AskCopy

```
Video upscale: 1080p -> 4K, maintain motion clarity
```

---

### 

**Parameters (editor-ready)**

#### 

**Topaz Photo (image)**

Name

Type

Default

Notes

`Image`

Upload

—

Required still image input

`Enhancement`

Select

Standard

Standard V2 (default), Low Resolution V2, CGI, High Fidelity V2, Text Refine

`Scale`

Slider

2×

1×–4× (0.5 increments); higher values increase cost and render time

`Seed`

Seed

Random

Optional; set for reproducible enhancement

#### 

**Topaz Video**

Name

Type

Default

Notes

`Video`

Upload

—

Input clip (≤8192×8192)

`Scale`

Slider

2×

1×–4× (0.5 increments); requests above 4× are clamped

`Target FPS`

Slider

24

16–60 FPS; retimes output to match selection

`Aspect Ratio`

Inherited

Auto

Hidden control; keeps the original frame proportions

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Image → Image

~10 seconds

Media

Upscale & restore photos

Video → Video

~1 minute

Media

Video upscaling & stabilization

---

### 

**Output options**

Option

Values / notes

Scale

Image: 1×–4× · Video: 1×–4× (auto-clamped to max 8192×8192 output)

Formats

PNG, JPG (image) · MP4 (video)

Notes

Enhancement presets: Standard V2, Low Resolution V2, CGI, High Fidelity V2, Text Refine

---

### 

**Prompt tips**

- For portraits or text, start with Standard V2; switch to Low Resolution V2 for tiny originals or Text Refine for signage.
 
- Preview a short crop before long renders to dial in scale, FPS, and enhancement choices.
 

---

[PreviousMagnific Upscaler & Enhancer](https://docs.flora.ai/models/image-models/magnific-upscaler-and-enhancer) [NextFlux Kontext Max (by Black Forest Labs)](https://docs.flora.ai/models/image-models/flux-kontext-max-by-black-forest-labs)

Last updated 25 days ago

Was this helpful?