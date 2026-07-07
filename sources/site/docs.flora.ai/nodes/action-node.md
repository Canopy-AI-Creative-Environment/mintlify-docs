# Source: https://docs.flora.ai/nodes/action-node

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/action-node.md).

Action Nodes bring traditional editing tools—color grading, video trimming, frame extraction, text manipulation, and more—into your canvas as workflow steps. Instead of exporting media to an external editor and re-importing the result, you can drop an Action Node right into your workflow and connect it like any other node.

## 

Overview

Actions handle the kinds of operations you'd normally reach for a dedicated editing app to do:

- **Adjusting color and tone** on an image or video
 
- **Splitting or stitching** video clips together
 
- **Extracting frames** from a video as still images
 
- **Changing aspect ratios** with crop or pad options
 
- **Manipulating text** with find-and-replace, splitting, or concatenation
 
- **Splitting or merging audio tracks** from video files
 

Because they live on the canvas alongside your generation nodes, Techniques, and Batch Nodes, actions slot naturally into any workflow—no round-tripping required.

---

## 

Getting Started

### 

Adding an Action Node

1

**Open the Add Node Menu**

Press the **+** button or use the canvas shortcut to open the node menu. Under the **Utilities** section, click **Action**.

2

**Choose an Action**

A picker panel opens showing all available actions. Browse the list or use the search bar to find what you need. Each action shows its input and output types (image, video, text) so you know what to connect.

3

**Connect Inputs**

Drag a connection from an upstream node (an Image, Video, or Text node) to the Action Node's input handle. The action will process whatever media is connected.

4

**Configure Parameters**

Each action has its own set of adjustable parameters (sliders, dropdowns, color pickers, toggles). Adjust these to dial in the exact result you want.

5

**Run**

Click the **Run** button on the Action Node. The result appears in one or more output slots depending on the action.

---

## 

Available Actions

Actions span image, video, and text operations. Here's the full catalog:

### 

Image Actions

Action

What It Does

Key Parameters

**Color Grade Image**

Cinematic color grading with adjustable tone

Warmth, Contrast, Saturation, Brightness

**Color Filter**

Apply preset filters: Grayscale, Sepia, Duotone, Clarendon, Moon, Nashville, Noir, Fade, and more

Filter preset, Intensity

**Color Tint**

Tint an image with a chosen color using blend modes (Multiply, Screen, Overlay, Soft Light)

Tint Color, Intensity, Blend Mode

**Filter Color**

Isolate, replace, or remove pixels matching a target color (chroma key, background removal, color swap)

Target Color, Tolerance, Mode

**Change Image AR**

Change aspect ratio by center-cropping or padding without upscaling

Aspect Ratio, Fit (Crop/Pad), Background Mode

**Rotate Image**

Rotate by any angle with optional canvas expansion

Angle, Expand Canvas, Background Color

**Flip Image**

Mirror horizontally, vertically, or both

Direction

**Blur**

Gaussian, Box, Motion, Radial, Bilateral, Bokeh, Tilt-Shift, or Target Color blur

Blur Type, Radius/Amount

**Duplicate Image**

Output N copies of an image for branching into parallel workflow lanes

Number of Copies

### 

Video Actions

Action

What It Does

Key Parameters

**Color Grade Video**

Cinematic color grading for video

Contrast, Saturation, Brightness, Gamma

**Video Color Filter**

Preset color filters for video: Grayscale, Sepia, Invert, Clarendon, Moon, Nashville, and more

Filter preset

**Video Effect**

Stylistic effects: Vignette, Film Grain, Pixelate, Camera Shake, Chromatic Aberration, VHS

Effect type, Intensity

**Stitch Videos**

Join multiple clips into one with optional transitions and aspect-ratio normalization

Transition type, Duration, Aspect Ratio, Fit Mode

**Split Video**

Cut a video into segments by equal parts, fixed duration, or scene detection

Split Mode, Segment count, Sensitivity

**Extract Video Frames**

Pull still frames from video as PNG images

Mode (Single, Evenly Spaced, Interval, Scene Changes)

**Image to Video Ken Burns**

Animate a still image with smooth pan/zoom into a video

Duration, Zoom Level, Pan Direction, Easing

**Video to Frame Grid**

Arrange extracted frames in a grid contact sheet

Rows, Columns, Cell Width, Gap

**Video to Long Exposure**

Stack all frames into a single long-exposure image (Average, Lighten, Darken blend)

Blend Mode

**Boomerang**

Play a video forward then reverse for a looping clip

Loops, Speed, Frame Stride

**Reverse Video**

Play a video backwards

Reverse Audio, Keep Original Audio

**Speed Up Video**

Increase playback speed

Speed Factor, Keep Audio

**Slow Down Video**

Decrease playback speed

Slow Factor, Keep Audio

**Watermark**

Burn a text or image watermark into a video

Text/Image, Position, Opacity, Scale

**Greenscreen Remove**

Chroma-key out a background color and output transparent video

Color Preset, Similarity, Edge Blend

**Duplicate Video**

Output N copies of a video for branching workflows

Number of Copies

### 

Text Actions

Action

What It Does

Key Parameters

**Split Text**

Split text into parts by separator, regex, paragraph, line count, or character count

Split Mode, Separator, Max Parts

**Find and Replace**

Find and replace text with optional regex, case-insensitive, and whole-word modes

Find, Replace, Use Regex, Case Sensitive

**Concat Text**

Combine multiple text inputs into one

Separator, Prefix, Suffix, Trim, Skip Empty

---

## 

How Actions Work

### 

Inputs and Outputs

Every action declares typed **input slots** and **output slots**. The Action Node shows modality badges (image, video, text) on each slot so you can see at a glance what connects where.

- **Single inputs** accept exactly one connection (e.g., one image to color-grade)
 
- **Dynamic inputs** accept multiple connections (e.g., Stitch Videos takes 2+ video clips)
 
- **Single outputs** produce one result (e.g., a color-graded image)
 
- **Dynamic outputs** produce a variable number of results (e.g., Split Video outputs multiple video segments)
 

### 

Parameters

Actions expose configurable parameters directly on the node—no prompt writing needed. Parameter types include:

- **Sliders** for numeric values (warmth, contrast, speed factor)
 
- **Dropdowns** for preset options (blur type, filter style, aspect ratio)
 
- **Color pickers** for color-based operations (tint color, background color)
 
- **Toggles** for boolean options (keep audio, expand canvas)
 
- **Text fields** for string inputs (watermark text, separator)
 

Some parameters are conditional—they only appear when a related setting is active. For example, the Blur Amount slider in Change Image AR only shows when Fit is set to "Pad" and Background Mode is "Blur."

## 

Actions in Workflows

Actions become especially powerful when connected into larger workflows alongside other Flora nodes.

### 

Chaining with Generation Nodes

Use actions to prepare media before or after AI generation:

AskCopy

```
[Text Node] → [Image Node: Generate] → [Color Grade Image] → Final Output
              "product on white bg"     warmth=0.2, contrast=1.3
```

Generate an image with AI, then apply deterministic color grading for a consistent brand look.

### 

Combining with Techniques

Actions work seamlessly as steps before or after Techniques:

AskCopy

```
[Image Upload] → [Change Image AR] → [Technique: Product Lifestyle] → Final Output
                  9:16 portrait
```

Reformat your image to the right aspect ratio before feeding it into a multi-step technique.

### 

Actions Inside Techniques

Action Nodes can be included directly inside a Technique's workflow graph. When you build a technique in the Technique Builder, you can wire action nodes alongside generation nodes—the action executes via the sandbox during the technique run, and its outputs flow through to downstream nodes or technique outputs.

This means you can package deterministic post-processing (color grading, frame extraction, audio splitting, etc.) as part of a reusable technique pipeline. For example:

AskCopy

```
[Input Image] → [Image Node: Generate styled version] → [Color Grade Image] → [Output]
```

The action node runs automatically as part of the technique—users of the technique don't need to set up or configure the action separately.

When viewing a technique's internal workflow (via **View workflow** on a Technique Node), action nodes appear as violet "Action" blocks with a distinct icon, making them easy to distinguish from generation nodes.

### 

Batch Processing

Connect a [Batch Node](https://docs.flora.ai/nodes/batch-node) to an Action Node to apply the same operation across many items at once:

AskCopy

```
[Image 1] ─┐
[Image 2] ─┼─→ [Batch Node] ─→ [Color Grade Image] → 4 graded outputs
[Image 3] ─┤     (4 items)      warmth=0.15
[Image 4] ─┘
```

Every item in the batch is processed with identical settings—perfect for maintaining visual consistency across a set of assets.

### 

Multi-Step Action Chains

Actions can chain together for complex transformations without any AI:

AskCopy

```
[Video Upload] → [Split Video] → [Extract Frames] → [Color Filter: Noir]
                  3 segments       per segment          per frame
```

### 

Cross-Modality Conversions

Some actions convert between modalities, enabling creative cross-format workflows:

AskCopy

```
[Image] → [Ken Burns Video] → [Stitch Videos] → Final Video
[Image] → [Ken Burns Video] ─┘
```

Turn still images into animated clips and stitch them into a sequence—all without AI generation.

### 

Audio Workflows

The audio actions enable creative audio-visual workflows:

AskCopy

```
[Video Upload] → [Split Audio from Video] → Audio track + Muted video
```

AskCopy

```
[Video] ─→ [Merge Audio into Video] → Video with new soundtrack
[Audio] ─┘
```

Extract audio for transcription or remixing, or replace a video's audio track with a voiceover or music track generated from an Audio Node.

---

## 

Tips

- **Test with one input first** before connecting a batch—dial in your parameters on a single item, then scale up
 
- **Chain actions freely**—they're lightweight and fast, so stacking multiple actions adds minimal time
 
- **Use Duplicate Image/Video** to branch a single input into parallel workflow lanes with different downstream processing
 
- **Dynamic outputs** (like Split Video or Extract Frames) produce multiple result nodes—each can feed into its own downstream workflow
 
- **Audio actions stream-copy** when source codecs are mp4-native (e.g., h264 + AAC), making them near-instant for common video formats
 

[PreviousLayer Editor](https://docs.flora.ai/nodes/layer-editor) [NextBatch Node](https://docs.flora.ai/nodes/batch-node)

Last updated 1 month ago

Was this helpful?