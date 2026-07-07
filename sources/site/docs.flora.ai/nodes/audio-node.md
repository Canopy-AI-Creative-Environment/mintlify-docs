# Source: https://docs.flora.ai/nodes/audio-node

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/audio-node.md).

The Audio Node brings audio generation and transcription to the FLORA canvas. You can generate speech from text, create sound effects, and transcribe audio to text — all integrated into your node-based workflows.

## 

Overview

Audio nodes support two directions of generation:

- **Text to Audio** — Generate speech or sound effects from a text prompt
 
- **Audio to Text** — Transcribe or analyze audio content into text
 

These modes are determined automatically based on how you connect the audio node to other nodes on your canvas.

---

## 

Text to Audio

### 

How It Works

Connect a text prompt or text node output to an audio node to generate speech or sound effects. The audio node will produce an audio file based on your prompt and selected model.

### 

Voice Selection

Audio nodes include an inline **voice selector** in the floating controls and pre-output state. You can:

- **Browse voices** — Open the voice dropdown to see all available voices for the selected model
 
- **Preview voices** — Click the play button next to any voice to hear a sample before selecting
 
- **Switch voices** — Change the voice at any time without leaving the node
 

The voice selector reads options directly from the model's available parameters, so the voice list updates automatically when you switch models.

### 

Supported Models

Audio generation is available through providers including **ElevenLabs** for text-to-speech and sound effects. Available voices and capabilities vary by model.

---

## 

Audio to Text

### 

How It Works

Connect an audio node's output to a text node to enable audio-to-text transcription. FLORA automatically detects the `Audio to Text` mode and routes the audio through a speech-to-text model.

### 

Supported Models

Audio-to-text transcription is supported by:

- **ElevenLabs** — Speech-to-Text via the ElevenLabs STT endpoint
 
- **Gemini** — Audio input is sent as inline data alongside your text prompt, enabling audio analysis and transcription
 

### 

Connecting Audio to Text Nodes

1. Add an audio node to your canvas with generated or uploaded audio
 
2. Drag a connection from the audio node's right output handle to a text node's input
 
3. The text node automatically switches to `Audio to Text` mode
 
4. Run the text node to transcribe or analyze the audio
 

---

## 

Credit Costs

Audio generation costs vary by model and duration. Before generating, hover over the **generate button** to see a credit cost tooltip showing:

- **Estimated credit cost** for the generation
 
- **Your available credits**
 

Credits are charged when the generation starts. If a generation fails, credits are automatically refunded.

---

## 

Tips

- **Preview voices before committing** — Use the play buttons in the voice selector to find the right voice for your project before spending credits
 
- **Chain audio into text** — Connect audio outputs to text nodes for transcription, then feed that text into image or video prompts for end-to-end multimedia workflows
 
- **Check model capabilities** — Different audio models support different voices, languages, and output qualities. Check the model details for specifics.
 

---

_Last updated: April 2026_ The audio node brings voice, sound, and sonic atmosphere into your FLORA canvas. It closes the loop between what you see and what you hear, letting you generate voiceovers, sound effects, and transcriptions alongside the image and video work already happening on your canvas. No jumping out to a separate tool, no booking scratch VO, no silent concepts. Audio nodes turn sound into another first-class node you can pipe into the rest of your workflow.

Here is a quick introduction on how to get started with audio nodes:

## 

Capabilities

- Text-to-speech. Type a script, choose a voice, and get a voiceover back. Play it on the canvas, export as MP3 or WAV.
 
- Text-to-SFX. Describe a sound effect in plain language and generate it in place.
 
- Text-to-Music. Describe a sonic environment in plain language and recieve a matching track.
 
- Audio-to-text. Transcribe an audio clip into a text node for editing, captioning, or downstream prompting.
 
- Lipsync. Pair an audio node with a video node to drive a lipsynced performance.
 
- FAUNA-aware. FAUNA can create and chain audio nodes for you as part of a multi-step workflow.
 

## 

Models

Visit our [Audio Models](https://docs.flora.ai/models/audio-models) section to learn about the video models and capabilities available in the Video Node.

[PreviousAudio to Video](https://docs.flora.ai/nodes/video-node/audio-to-video) [NextText to Audio](https://docs.flora.ai/nodes/audio-node/text-to-video)

Last updated 1 month ago

Was this helpful?