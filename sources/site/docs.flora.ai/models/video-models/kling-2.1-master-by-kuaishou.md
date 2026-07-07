# Source: https://docs.flora.ai/models/video-models/kling-2.1-master-by-kuaishou

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/models/video-models/kling-2.1-master-by-kuaishou.md).

### 

**Overview**

Text → video model for motion-rich short clips.

---

### 

**Quick facts**

- **Modes:** Text → Video · Image → Video
 
- **Default clip length:** 5 seconds (optionally 10s)
 
- **Aspect ratios:** 9:16
 

---

### 

**What it’s great for**

- Short cinematic motion generation.
 
- Motion diversity and prompt adherence in quick clips.
 
- Iterative creative experiments across quality tiers.
 

---

### 

**Example outputs**

Image reference — deer close-up

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FZLCAy7ieAYYXwQOGQ1we%252Fimage.png%3Falt%3Dmedia%26token%3Da0891d05-5f03-4b9e-8e4c-3a0af3d44da6&width=768&dpr=3&quality=100&sign=d02ae1b2&sv=2)

Image reference video

5s text → video motion shot

Action motion frame

#### 

**Copy-and-paste prompts**

AskCopy

```
"Fashion editorial close-up video: lower body mid-run on a sunlit walkway with diagonal shadows; vivid red knee-high socks with fluttering ribbon, glossy black Mary Jane kitten heels; elegant and playful mood; strong motion blur, shallow depth of field, warm film grain, high contrast, minimalist background."
```

AskCopy

```
"A high-energy action motion sequence: capture a subject mid-movement as if frozen in time, then released back into motion. Begin with a moment of suspension — the body in mid-air, hair and fabric pulled upward — then flow into the follow-through of impact or landing. Cinematic realism with strong directional light, high shutter speed look for clarity, natural motion blur trailing behind the limbs. Camera: dynamic tracking at 35mm, shifting from a low angle to eye level, emphasizing intensity. The sequence should feel like a compressed burst of energy — one decisive action visualized across just a few seconds."
```

AskCopy

```
"A white deer stands on a rocky hilltop under a dark blue sky. The camera zooms rapidly towards the deer's face. The deer stares directly at the camera, its white fur distinct against the rocks. Shadows play across its antlers as the camera moves closer."
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

5s

5s, 10s

`Aspect Ratio`

\-

Portrait (9:16)

\-

---

### 

**Modes**

Mode

Estimated time

Required inputs

Typical use

Text → Video

~3 minutes

Prompt

Short cinematic clips

Image → Video

~3 minutes

Image, Prompt

Animate assets

---

### 

**Output options**

Option

Values / notes

Duration

5s, 10s

Aspect ratio

9:16

---

### 

**Prompt tips**

- Describe camera motion explicitly; Kling responds well to motion tokens.
 
- Use short duration for cost/time efficiency.
 

---

[PreviousKling 2.5 Turbo Pro (by Kuaishou)](https://docs.flora.ai/models/video-models/kling-2.5-turbo-pro-by-kuaishou) [NextKling O1 (by Kuaishou)](https://docs.flora.ai/models/video-models/kling-o1-by-kuaishou)

Last updated 1 month ago

Was this helpful?