# Source: https://docs.flora.ai/nodes/audio-node/text-to-video

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/audio-node/text-to-video.md).

You can start an audio workflow from a text node. Write a script, describe a sound, or sketch the music you want, then connect it to an audio node and pick a model. What comes back is playable audio on the canvas. Ready to export, layer under a video, or drive a lipsynced performance in a video node.

Speech

Text-to-speech turns a written script into a voiceover. Type what you want said, pick a voice from the preset library, and generate. Good for narration on explainer videos, scratch VO for concept pitches, or any moment where a voice needs to land on the canvas without a recording session.

You can interact with it in a number of ways:

- Type or paste your script into the prompt field
 
- Select a voice from the dropdown, or use a recorded custom voice asset
 
- Use expressive prompt tags (e.g. whisper, shout, happy) on models that support them to shape delivery
 
- Connect the output to a video node with a lipsync model to drive a lipsynced performance
 

SFX

Text-to-SFX generates individual sound effects from a plain-language description. Describe the sound — "heavy wooden door slamming shut in a stone hallway" — and generate. Useful for ambient texture, hit sounds, foley, and anywhere you'd otherwise be digging through a stock library.

Best practices:

- Be specific about the source and environment (material, space, distance)
 
- Generate a few variations with different seeds and pick the strongest
 
- Layer multiple SFX audio nodes for richer atmospheres
 

Music

Text-to-music generates short music tracks from a text prompt describing genre, mood, instrumentation, or reference. Useful for background beds on social clips, pitch videos, and mood-setting on ad concepts where you don't want to license a track.

You can interact with it in a number of ways:

- Describe the track — genre, tempo, instruments, mood, references
 
- Generate variations across seeds to find the right feel
 
- Pair music output with a video node for a scored clip
 

How to use:

Here are some example workflows using Text to Audio:

- Write a script → generate speech → connect to a video node with a lipsync model → export a lipsynced clip
 
- Generate a product-demo voiceover → layer a music bed from text-to-music → export a finished promo
 
- Generate three SFX variations for a scene → pick the strongest → layer onto a generated video
 

Models

Visit our [Audio Models](https://docs.flora.ai/models/audio-models) section to learn about the speech, SFX, and music models available in the Audio Node.

## 

Limits & formats

**Character limit (ElevenLabs Multilingual v2)** ElevenLabs Multilingual v2 has a 450-character limit per generation. Text longer than 450 characters is truncated — this is why a script with 800+ characters may only produce audio for the first ~450. To narrate longer scripts, split the text across multiple audio nodes and chain them.

**Output format** Audio is delivered as MP3. WAV output is not currently available for ElevenLabs voice models in FLORA.

**Bitrate** The MP3 bitrate is fixed at 128 kbps and cannot be changed.

[PreviousAudio Node](https://docs.flora.ai/nodes/audio-node) [NextDocument Node](https://docs.flora.ai/nodes/document-node)

Last updated 1 month ago

Was this helpful?