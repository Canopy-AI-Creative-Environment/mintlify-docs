# Source: https://docs.flora.ai/models/video-models/veo-3-by-google

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/video-models/veo-3-by-google.md).

### 

**Overview**

Advanced text→video model with native audio generation and high-quality outputs.

---

### 

**Quick facts**

- **Modes:** Text → Video · Image → Video.
 
- **Default clip length:** 8 seconds
 
- **Resolution:** 960×960 (square) · 1280×720 (landscape) · 720×1280 (portrait)
 
- **Aspect ratios:** 16:9, 1:1, 9:16
 

---

### 

**What it’s great for**

- Short cinematic clips with integrated audio.
 
- Rapid prototyping with sound design included.
 
- Short-form content pipelines.
 

---

### 

**Example outputs**

Scene with native audio — fox in misty forest

Motion frame — high-contrast macro shot

Audio-synced shot — dialogue moment

#### 

**Copy-and-paste prompts**

AskCopy

```
"A close-up, cinematic shot of a lone fox in a misty forest, fur rippling with each breath, slow dolly-in as it turns its head toward the camera, faint rustle of leaves and a distant low call filling the soundscape."
```

AskCopy

```
"High-contrast black and white macro video of an Asian female eye veiled by long strands of hair, shot on a 100mm macro lens with handheld-to-dolly motion; slow 8–10s dolly-in with parallax through hair, subtle rack focuses, micro-blink, moisture beads, drifting dust motes, film-grain,2000s cinema. Ominous dreamcore/mood with single soft key light, deep shadows, crushed blacks, specular pupil gleam, and faint lens/film defects."
```

AskCopy

```
"A cinematic video of a woman on a dimly lit train station platform, camera dollying in as she whispers, “I’m leaving tonight, and you won’t find me here again,” her voice echoing under flickering lights, blending with footsteps and the rising rumble of an approaching train."
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

Landscape (16:9)

Landscape (16:9), Square (1:1), Portrait (9:16)

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Text → Video

~4 minutes

Prompt

Videos with audio

Image → Video

~4 minutes

Image, Prompt

Animate stills with sound

---

### 

**Output options**

Option

Values / notes

Formats

MP4 (H.264 + AAC)

---

### 

**Prompt tips**

- Describe desired soundscapes in the prompt for richer audio results.
 
- Use explicit timing tokens for beats or cuts.
 

---

[PreviousVeo 3.1 (by Google)](https://docs.flora.ai/models/video-models/veo-3.1-by-google) [NextSora 2 Pro (by OpenAI)](https://docs.flora.ai/models/video-models/sora-2-pro-by-openai)

Last updated 1 month ago

Was this helpful?