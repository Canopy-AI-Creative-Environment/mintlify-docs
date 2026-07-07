# Source: https://docs.flora.ai/models/video-models/seedance-by-bytedance

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/video-models/seedance-by-bytedance.md).

### 

**Overview**

Multi-shot text or image → video model for coherent, cinematic multi-shot output.

---

### 

**Quick facts**

- **Modes:** Text → Video · Image → Video.
 
- **Default clip length:** 5 seconds (3s–12s selectable)
 
- **Aspect ratios:** 21:9, 16:9, 4:3, 1:1, 3:4, 9:16
 
- **Training / licensing:** Proprietary model by Bytedance, licensed for commercial use within FLORA
 

---

### 

**What it’s great for**

- Multi-shot narrative sequences and longer-form short clips.
 
- High-coherence motion and smooth playback.
 
- Storytelling use cases requiring multiple shots.
 

---

#### 

**Copy-and-paste prompts**

AskCopy

```
Three-shot sequence: establish city skyline, mid shot of protagonist walking, close-up face — cinematic pacing — 10s total
```

AskCopy

```
Image→Video: animate product spin across three cuts, consistent lighting and reflections
```

AskCopy

```
Single-shot 1080p: slow crane up from street to rooftop, ambient city ambience
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

`Duration`

Select

10s

3s–12s options (higher values increase cost)

`Resolution`

Select

1080p

480p, 720p, 1080p

`Seed`

Seed

Random

Optional

`Fixed Camera`

Select

No

Yes, No

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Text → Video (multi-shot)

~2 minutes

Prompt

Narrative multi-shot sequences

Image → Video

~2 minutes

Image, Prompt

Animate assets across shots

---

### 

**Output options**

Option

Values / notes

Resolution

1280×720, 1920×1080

Duration

3s, 4s, 5s, 6s, 7s, 8s, 9s, 10s, 11s, 12s

Formats

MP4 (H.264 + AAC)

Notes

Designed for narrative and smooth motion

---

### 

**Prompt tips**

- Break multi-shot intent into clear shot descriptions (shot 1:, shot 2:, shot 3:).
 
- Use pacing terms like “slow”, “cut-to”, “dolly”, and exact durations.
 

---

[PreviousKling O1 (by Kuaishou)](https://docs.flora.ai/models/video-models/kling-o1-by-kuaishou) [NextLTX-2 Pro (by Lightricks)](https://docs.flora.ai/models/video-models/ltx-2-pro-by-lightricks)

Last updated 1 month ago

Was this helpful?