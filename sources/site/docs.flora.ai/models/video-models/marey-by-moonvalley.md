# Source: https://docs.flora.ai/models/video-models/marey-by-moonvalley

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/video-models/marey-by-moonvalley.md).

### 

**Overview**

High-quality video generation and motion-transfer model for short cinematic clips.

---

### 

**Quick facts**

- **Modes:** Text → Video · Image → Video · Motion / Pose Transfer (video → video)
 
- **Default clip length:** 5s (supports 10s)
 
- **Aspect ratios:** Auto, 16:9, 4:3, 1:1, 3:4, 9:16
 
- **Licensing:** Trained only on fully licensed, high-resolution footage (no scraped or user-submitted data)
 

---

### 

**What it’s great for**

- Short cinematic pieces and motion studies
 
- Turning still images into motion (image → video)
 
- Transferring motion or pose from reference videos to targets
 

---

### 

**Example outputs**

Hero frame — static hero still

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FB99S3BfFblakBV453t4I%252FScreenshot%25202025-09-16%2520at%25205.16.54%25E2%2580%25AFPM.png%3Falt%3Dmedia%26token%3D946acc95-ba6c-4dac-a065-e8d574780999&width=768&dpr=3&quality=100&sign=3951fdf7&sv=2)

5s cinematic clip (image → video)

10s pose-transfer sequence

#### 

**Copy-and-paste prompts**

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

Natural-language scene, motion, style description (required)

`Duration`

Select

5s

5s (default), 10s (cost multiplier 2×)

`Aspect Ratio`

Select

Landscape (16:9)

Landscape (16:9), Landscape (4:3), Square (1:1), Portrait (3:4)

`Seed`

Seed

Random

Optional for deterministic / repeatable outputs

---

### 

**Modes & endpoints**

Mode

Estimated time

Required inputs

Typical use

Text → Video (t2v)

~300s

Prompt

Short cinematic clip from text

Image → Video (i2v)

~420s

Image, Prompt

Animate still images

Video → Video (motion transfer)

~400s

Video, Prompt, Optional First Frame

Transfer motion from reference to target

Video → Video (pose transfer)

~300–400s

Video, Prompt

Transfer pose/gesture from reference video

---

### 

**Output options**

Option

Values / notes

Duration

5s (default), 10s (longer clips may cost more)

Aspect ratio

16:9 (1920×1080), 4:3 (1536×1152), 1:1 (1152×1152), 3:4 (1152×1536), 9:16 (1080×1920)

Notes

Marey generates up to ~5 seconds of consistent 24 FPS footage per clip in its public offering.

---

### 

**Prompt tips**

- Specify **motion** explicitly: e.g., “slow dolly in”, “camera orbit”, “subtle head turn”.
 
- Mention **shot specifics** when important: camera framing, lens feel, lighting, and duration.
 
- Use seed for repeatable variants or test different seeds to explore diversity.
 

---

### 

**Safety**

Marey is built for professional filmmaking workflows and emphasizes ethical sourcing and legal clarity for commercial use.

---

[PreviousWAN 2.6 (by Alibaba)](https://docs.flora.ai/models/video-models/wan-2.6-by-alibaba) [NextAudio Models](https://docs.flora.ai/models/audio-models)

Last updated 1 month ago

Was this helpful?