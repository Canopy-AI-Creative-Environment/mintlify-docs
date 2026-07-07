# Source: https://docs.flora.ai/editor/timeline-editor

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/editor/timeline-editor.md).

The Timeline Editor is FLORA's video editor, built directly into the canvas. It's a real multi-track timeline for trimming, sequencing, captioning, scoring, and rendering video — so the clips you generate in FLORA go all the way to a finished MP4 without leaving your workflow. Because the editor is a **node**, the finished cut flows right back onto the canvas as a new video you can keep building on.

## 

Overview

The Timeline Editor turns a node into a full video-editing workspace, connected live to the clips that feed it. In it you can:

- **Assemble a sequence** from your generated clips, laid out end to end on a single track
 
- **Trim and split** clips to the exact frames you want
 
- **Layer up to 10 tracks** of video, audio, text, captions, images, and shapes
 
- **Style each item** — position, size, crop, rotation, opacity, playback rate, volume, and fades
 
- **Caption and title** with your choice of font, stroke, and alignment
 
- **Render a finished MP4** server-side, saved back to the canvas as a new version
 
- **Export to a pro editor** as an EDL / XML / FCPXML bundle with your source media
 

This is ideal for cutting a social clip, assembling a product teaser, finishing an ad, or scoring a short — all without exporting to CapCut or Premiere just to put together what you already made in FLORA.

The Timeline Editor reads its clips **live from the nodes wired into it** and always uses each node's latest generation. That link back to your graph is what makes it different from a standalone editor — see [Connected inputs & live updates](https://docs.flora.ai/editor/timeline-editor#connected-inputs-and-live-updates).

---

## 

Getting Started

### 

Adding a Timeline Editor Node

1

**Add the Node**

From the node menu, select **Timeline** to add it to your canvas. (You can also add the node first and connect clips afterward — order doesn't matter.)

2

**Connect Source Clips**

Connect clip nodes to the Timeline node. Each connected input becomes one layer, in the order you connected them. Select several nodes to wire them all in at once.

You connect…

You get…

A video node

A video clip

An image node

A still clip (with a thumbnail)

An audio node

An audio track

A text node

An editable text layer

3

**Open the Editor**

**Double-click** the Timeline node, or click **Open Timeline Editor** in the node toolbar. The editor opens in place — the node becomes the editing surface, and the canvas stays pannable around it.

4

**Edit and Render**

Arrange, trim, and style your clips, then open the **Export** panel and choose **Edited File** to render a finished MP4 back onto the canvas.

The Timeline Editor is a paid feature — available on Starter and above (see [Plans & limits](https://docs.flora.ai/editor/timeline-editor#plans-and-limits)).

---

## 

The Editor Interface

The editor unfolds around the node itself — there's no full-screen takeover, and the FLORA chrome stays visible. It has three regions.

### 

The Preview

The live playback area, shown right on the node. It reflects whatever the playhead is over. Opening reframes the canvas so the node clears the surrounding chrome; if you pan or zoom the node out of view, a **Recenter** toast brings you back.

### 

The Properties Sidebar

On the right — a tools row plus an inspector that changes with your selection, organized into collapsible sections (at parity with the [Layer Editor](https://docs.flora.ai/nodes/layer-editor)).

Selected item

Controls

**Video clip**

Playback rate, volume, crop, rotation, rounded corners, position, size, opacity, fades

**Audio clip**

Volume, playback rate, fade in/out, timing

**Text / caption**

Font (Google Fonts), stroke, alignment, position, size, opacity, rotation

**Image / shape / GIF**

Position, size, crop, rotation, opacity, rounded corners

### 

The Timeline Drawer

Slides up along the bottom, holding the playback controls and the timeline — tracks, clips, playhead, and ruler. Clips show **film-strip thumbnails** (and audio shows a **waveform**), and each track has **hide** and **mute** toggles to solo or silence a layer. Drag the top edge to **resize its height**, and snap its **width** between default and full canvas width.

---

## 

Editing Clips

Your connected clips start on a **single track, end to end, in connection order** — a standard sequential assembly you then refine.

### 

Arranging

- **Drag** a clip left or right to reorder or move it; other clips make room.
 
- **Drag** a clip up onto another track to layer it (overlays, text, picture-in-picture). You can use up to **10 tracks**.
 

**Snapping** helps clips line up against each other and the playhead. Toggle it with the `N` key or the snapping toggle.

### 

Trimming

Drag a clip's **left edge** to change where it starts, or its **right edge** to change where it ends. Trimming is non-destructive — you're changing the in/out points of that placement, not the source media.

### 

Splitting at the Playhead

1. Move the **playhead** to the exact frame (scrub, or click the ruler).
 
2. Select the clip.
 
3. Click the **scissors button** (**Split Clip at Playhead**).
 

The clip splits into two, and you can trim, move, or delete either half. Split is available only when the playhead sits inside the selected clip.

### 

The Clip Menu

Right-click a clip for its context menu:

- **Go to Node** — frame the clip's source node on the canvas
 
- **Cut** / **Copy** / **Duplicate**
 
- **Bring to front** / **Send to back** — change stacking order where clips overlap
 

### 

Duplicating, Copying & Deleting

- **Duplicate** with `Cmd/Ctrl + D`.
 
- **Cut / Copy / Paste** with `Cmd/Ctrl + X` / `C` / `V`; **Select all** with `Cmd/Ctrl + A`.
 
- **Delete** with `Delete` or `Backspace` (this also removes the clip's connecting edge on the canvas).
 

### 

Styling a Clip

Select any item and shape it from the properties sidebar. **Every item** supports position, size, opacity, rotation, crop, layer order, and **fade in / fade out**. Video clips add playback rate, volume, and rounded corners.

There's no keyframe animation in this version, so an item's transform values are **constant for its duration**. To change a look partway through, split the clip and style each part separately. Undo any edit with `Cmd/Ctrl + Z` — undo applies to your edits only, never the surrounding canvas.

---

## 

Text & Captions

Add titles, lower thirds, credits, and timed captions directly to your video.

- **Add text in the editor** — press `T` to drop a new text item.
 
- **Connect a text node** — it comes in as an editable text layer, linked to its source node (Go to Node works on it, and renaming the node updates the label).
 

Style text from the sidebar: **font** (Google Fonts), **stroke** (an outline for legibility over busy footage), **alignment**, plus position, size, opacity, and layer order. Stack text above your video by putting it on a higher track.

**Captions** are handled as **timestamped caption pages** — text blocks tied to points in time, so each line shows at the right moment. Style them the same way as text.

---

## 

Audio

The Timeline Editor handles audio as its own kind of track, so you can lay music or a voiceover under your video and balance the mix.

- **Connect an audio node** (including audio you generated in FLORA), **drag** an audio asset from your library, or **upload** a file in the editor.
 
- Each source becomes its own layer, so a music bed and a voiceover can run on separate tracks.
 

Select an audio clip to set its **volume**, **playback rate**, **fade in / fade out**, and **timing** (trim its edges and drag it to line up with the picture). Video clips carry their own audio too, adjustable per clip — lower the video or music volume to let a bed sit under dialogue, and use **Mute** during playback to check the picture on its own.

---

## 

Connected Inputs & Live Updates

The Timeline Editor doesn't import copies of your clips — it reads them **live from the nodes wired into it**. Each connection is a layer that points back at its source node.

### 

Always the Latest Generation

The editor reads each connected node's **current active output** — normally the newest generation.

- **Regenerate while the editor is open**, and the layer refreshes to the new result automatically.
 
- **Regenerate while it's closed**, and the layer is up to date the next time you open.
 
- If you've selected an _older_ generation as a node's active output, the editor mirrors that — it matches what the node is currently showing.
 

When a source node regenerates, its layer is **replaced, not merged** — a per-clip trim on that clip resets, because it's now different media. Trims on other clips are unaffected.

### 

Go to Node

Every clip remembers where it came from. **Right-click a clip → Go to Node**, or **double-click** it, to frame its source node. Clips are labelled by their **source node's title** (not a file name or ID), and the label updates live if you rename the node. Text clips carry this link too.

### 

Adding Media Without a Node

- **Drag from your library** — any FLORA asset onto the timeline. Dragged-in assets are standalone (not linked to a source node).
 
- **Upload a file** — it lands on the timeline _and_ appears on the canvas as a connected media node, so it stays part of your graph.
 

New dropped or uploaded media lands as a new track starting at 0:00 — drag it along the track to place it.

### 

Good to Know

- **Empty inputs are allowed** — connect a node before it has generated anything; nothing appears until real content exists (you'll see a _"No generations to edit"_ notice).
 
- **Deleting a clip whose source is still connected** is temporary — it returns on reopen. Disconnect the source node to remove it for good.
 

---

## 

Playback

### 

The Playhead

The vertical line marking the current frame; the preview always shows what it sits on. **Click** the ruler to move it, or **drag** to scrub frame by frame. While playing, the timeline follows the playhead so it stays in view.

### 

Playback Controls

Control

What it does

Play / Pause

Plays from the playhead; pauses in place (`Space`)

Seek bar

Drag to move through the whole composition

Jump to start / end

Send the playhead to the beginning or the end

Loop

Repeat playback continuously

Mute

Silence preview audio

Fullscreen

Expand the preview to fill the screen

Only Play / Pause has a keyboard shortcut; the rest are buttons.

### 

Zooming

Zoom the timeline horizontally with the **zoom slider**, or by **pinching / scrolling** on a trackpad while the editor is focused. Zooming affects only the timeline, not the canvas.

The in-editor preview is a fast approximation; the final render is produced server-side at full quality. If a clip hasn't rendered yet, the preview shows its source's first frame rather than a blank box.

---

## 

Rendering & Export

The Timeline Editor gives you two ways to get your edit out, both in the node's **Export** panel.

### 

Render to a Finished Video

Choose **Edited File**. FLORA renders your timeline **server-side** — on FLORA's infrastructure, not in your browser — so you can keep working or close the tab while it runs. You'll see a render-time estimate up front and progress as it renders. The result is an **MP4 (H.264 video, AAC audio)**, saved back onto the canvas as a **new version of the Timeline Editor node**.

**"Save Edits" vs. "Edited File."** _Save Edits_ bakes your current timeline down to a new version. _Edited File_ does the same and then downloads the MP4. Either way, a render is what produces a version.

### 

Unexported Edits

Your edits live on the node as you work, but **downstream nodes keep using the last exported version** until you export again. While you have changes that haven't been rendered, the node shows an **"Unexported edits"** badge. Downloading a cut that hasn't been rendered yet triggers a render first, then downloads the result.

### 

What a Render Costs

Rendering is the one metered action — it draws on your workspace's **credits**, scaled by the **length and resolution** of the output. The editor shows the estimated cost before you render. Editing, previewing, and the NLE export are always free. See [How renders are billed](https://docs.flora.ai/editor/timeline-editor#how-renders-are-billed).

### 

Render Quality

Renders use a balanced **Standard** profile by default. Where the picker is available, you can choose **High** (higher quality, slower) or **Compact** (smaller file). Set defaults per profile — output max edge, CRF, encoder preset, audio bitrate — in **Account → Timeline Editor** preferences.

### 

Export to a Pro Editor (NLE Bundle)

To finish somewhere else, use the **Timeline + Assets** section — pick a format and download a ZIP with the project file plus your source media:

Format

Opens in

**EDL** (CMX3600)

Most NLEs

**XML** (FCP7 XML)

Premiere Pro

**FCPXML**

Final Cut Pro, DaVinci Resolve

The timeline is reconstructed with clips relinked to the packaged sources. This export is client-side and runs no render.

Rendering runs server-side. If a server render isn't available and your browser falls back to in-browser encoding, use the latest **Chrome or Edge** — some browsers can't encode MP4 locally yet.

---

## 

Plans & Limits

The Timeline Editor is a paid feature. Output length and resolution scale with your plan; frame rate, format, and track/clip capacity are shared across paid plans. Rendering draws on your workspace's credits.

### 

Availability

Plan

Timeline Editor

Free

Not included

Starter

✅

Pro

✅

Max

✅

Enterprise

✅

If your plan doesn't include it, you'll see _"Timeline export is not included on your current plan."_

### 

Length, Resolution & Inputs by Plan

Limit

Starter

Pro

Max

Enterprise

Max duration

60 s

120 s

300 s (5 min)

600 s (10 min)

Max resolution

1080p (1920 px)

1080p (1920 px)

4K (4096 px)

4K (4096 px)

Image inputs

10

15

20

40

Video inputs

10

15

20

40

Audio inputs

5

8

10

20

Pro adds all aspect ratios (vertical/portrait) at 1080p; Max and Enterprise unlock 4K (up to 4096×2304).

### 

Shared Across All Paid Plans

Limit

Value

Frame rate

30 FPS

Output format

MP4 — H.264 video, AAC audio

Tracks (parallel layers)

10

Timeline items (clip placements)

100

Unique source assets

40

Max video file size (per upload)

500 MB

**Assets** are unique source files (one clip reused five times = 1 asset); **items** are placements on the timeline (that clip in five places = 5 items); **tracks** are the layers items sit on.

### 

How Renders Are Billed

- Render cost is charged in **credits** and scales with the **length and resolution** of the output — a short 1080p cut costs a fraction of a full-length 4K one.
 
- **Enterprise** plans include a monthly render allowance (about **$100 of render usage per user**) before overages apply.
 

For the credits included with your plan and current render pricing, see the [How Pricing Works](https://docs.flora.ai/plans-and-billing/pricing) section.

### 

Guardrails

- **Concurrency** — you can run up to **3 renders at once per user**; additional renders queue until one finishes.
 
- **Device playback** — preview plays in your browser, so heavy timelines can stutter on lower-memory machines. You may see a notice like _"This device supports up to 5 simultaneous video tracks — playback may stutter above that."_ It's a warning, not a hard block; the final server render is unaffected. Hide or mute tracks you're not working on to smooth playback.
 

---

## 

Keyboard Shortcuts

While the editor is focused, your normal canvas shortcuts are paused — so `Cmd/Ctrl + Z` undoes your last edit and never deletes the node. Shortcuts don't fire while you're typing in a text field.

Action

Shortcut

Play / Pause

`Space`

Undo

`Cmd/Ctrl + Z`

Redo

`Cmd/Ctrl + Shift + Z` (or `Cmd/Ctrl + Y`)

Select all

`Cmd/Ctrl + A`

Duplicate

`Cmd/Ctrl + D`

Cut / Copy / Paste

`Cmd/Ctrl + X` / `C` / `V`

Delete

`Delete` or `Backspace`

Toggle snapping

`N`

Add text

`T`

Add media (import)

`Cmd/Ctrl + I`

Export EDL / XML / FCPXML

`7` / `8` / `9` (Export panel open)

**Split** has no hotkey — use the scissors button. Loop, mute, fullscreen, and jump-to-start/end are buttons, not keys. Zoom with the slider or a trackpad pinch/scroll.

---

## 

Limitations

Limitation

Details

No transitions beyond fades

No crossfades, dissolves, or wipes — only per-item fade in/out

No effects or color

No filters, LUTs, blur, distortion, or color grading

No keyframe animation

Per-item transforms are static for the clip's duration

Fixed output specs

30 FPS, MP4 / H.264 only

Plan-capped length & size

Duration and resolution are capped by plan (60–600s, 1080p–4K)

No Free access

The Timeline Editor is a paid feature

For anything beyond this — color, VFX, or long-form finishing — use the [NLE export](https://docs.flora.ai/editor/timeline-editor#export-to-a-pro-editor-nle-bundle) and finish in DaVinci Resolve, Final Cut, or Premiere.

---

## 

Troubleshooting

### 

A connected clip isn't showing

The source node hasn't generated anything yet, or its **active generation** isn't the one you expect — the editor shows the node's currently active output.

### 

My trim reset itself

The source node regenerated, so its layer was rebuilt from the new result. To keep a trim regardless of regeneration, drag the finished asset in from your library (standalone) instead of leaving it linked.

### 

A clip I deleted came back

Deleting a clip whose source is still connected is temporary. **Disconnect the source node** to remove it permanently.

### 

Render won't start

You may not be on a plan that includes it, you may be over your plan's duration/resolution cap, or you may be at the 3-renders-per-user concurrency limit. Rendering is server-side, so it continues even if you close the tab.

---

## 

Tips for Better Edits

- **Preview freely, render once** — editing and previewing are free; you're only billed on render, so lock the cut before you export.
 
- **Split to restyle** — since transforms are static per clip, split a clip to change a look partway through.
 
- **Name your source nodes** — clips are labelled by node title, so clear names make a busy timeline readable.
 
- **Hide or mute tracks** you're not working on to keep preview smooth on heavier edits.
 
- **Use Go to Node** to jump back and regenerate a weak clip without losing your place in the edit.
 

---

## 

Common Use Cases

- **Social clips** — cut generated shots into a vertical reel with captions and a music bed
 
- **Product teasers** — assemble a 30–60s sequence, trim to the beat, and render a clean MP4
 
- **Ads & sizzle reels** — quick-cut multiple clips end to end with titles and audio
 
- **Finishing hand-off** — assemble a rough cut in FLORA, then export the NLE bundle for color and VFX elsewhere
 

[PreviousImage Editing](https://docs.flora.ai/editor/image-editing) [NextNavigation](https://docs.flora.ai/editor/navigation)

Last updated 6 hours ago

Was this helpful?