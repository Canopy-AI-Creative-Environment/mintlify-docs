# Source: https://docs.flora.ai/nodes/video-node/audio-to-video

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/video-node/audio-to-video.md).

Audio-to-Video workflows turn the output of an audio node into an input for a video node, so the sound you've generated on the canvas: a voiceover, a line of dialogue, a sound effect, a music cue drives the visuals you produce next. This is how speech becomes a lipsynced performance, how a still image becomes a talking avatar, and how generated sound lands on the same canvas as the video it belongs to, without ever leaving FLORA.

The shape of the workflow is always the same. You generate or upload audio in an audio node, connect that audio node's output to a video node, connect a second input (either a video of a speaker for lipsync or a reference image for avatars), and pick a model that accepts audio as an input. The video node treats the audio as a conditioning signal matching mouth movement to speech, aligning motion to rhythm, or syncing timing to a beat. Then is renders a clip that already has the sound baked in.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FowlBGpN5U5cHgULn700l%252FAdobe%2520Express%2520-%2520audionode.gif%3Falt%3Dmedia%26token%3Dd2afdc71-5809-4632-94d3-da301ee7dfdc&width=768&dpr=3&quality=100&sign=ff4ba68b&sv=2)

### 

Parameters

Parameter

Type

Effect on Output

Audio

Audio

The audio output from an audio node. Connect a generated voiceover, SFX, music track, or uploaded clip — this is the track that drives the video.

Video

Video

The visual source the audio is applied to. Connect a video node for lipsync workflows, or an image node for talking-avatar generations.

Prompt

Text

Optional text guidance passed to models that accept it alongside audio and visual inputs. Useful for steering delivery, style, or camera behavior on models that expose those controls.

Duration

Derived

Most audio-to-video models produce a clip whose length matches the input audio. Trim the audio track before generating if you want a shorter output.

Audio to Video

The Audio to Video workflow takes an audio track and generates a synced video from it. When you connect an audio node to a video node and switch to an audio-aware model. The model then reads the audio as part of the conditioning taking into account the delivery, timing, and motion in the output all follow the track you provided.

You can interact with it in a number of ways:

- Connect any audio node output to the video node to populate the audio input
 
- Optionally connect an image node as a subject or scene reference
 
- Use the prompt to describe the setting, camera, and style the model should render
 
- Switch the model to WAN 2.6 or WAN 2.7 for audio-driven generation
 
- Adjust aspect ratio and resolution to match your delivery format
 

How to use

Prompting matters for Audio to Video too — your audio carries dialogue and timing, but the prompt carries the scene.

[PreviousImage(s) to Video](https://docs.flora.ai/nodes/video-node/image-s-to-video) [NextAudio Node](https://docs.flora.ai/nodes/audio-node)

Last updated 2 months ago

Was this helpful?