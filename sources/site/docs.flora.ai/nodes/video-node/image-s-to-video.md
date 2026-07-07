# Source: https://docs.flora.ai/nodes/video-node/image-s-to-video

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/video-node/image-s-to-video.md).

## 

Summary

Image-to-Video models generate videos by taking a single image or multiple images as input, using the input image(s) to guide scene continuity, motion, and transitions, resulting in dynamic video content that expands the static visuals into a moving narrative while maintaining visual consistency.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252Fy4FdoUEsmYxofdQl0KZs%252FScreenRecording2025-02-24at2.40.52PM-ezgif.com-video-to-gif-converter.gif%3Falt%3Dmedia%26token%3De8b5f2a4-63cd-4a4e-b232-f0f5ed65e755&width=768&dpr=3&quality=100&sign=147a55ac&sv=2)

### 

Parameters

These are parameters that are applicable to all our base models.

Parameter

Type

Effect on Output

Prompt

Text

The text prompt is processed through the selected model.

Seed

Seed

The seed is a deterministic number that indexes generations from the model. It's typically randomized, but you can set a seed if there's a particular output you're looking for! Keep in mind that all parameters must be the same in order for a given seed's output to persist.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FYFeK1YuGUowX4PfnU1BG%252FScreenRecording2025-02-24at4.02.15PM-ezgif.com-video-to-gif-converter.gif%3Falt%3Dmedia%26token%3D9b5ed9b0-2376-4560-a007-65484f3b3eb2&width=768&dpr=3&quality=100&sign=a86f2def&sv=2)

### 

Images to Video

The Images to Video node generates a video by connecting multiple frames. You can input up to 9 frames and the model will fill in the gaps! It primarily uses IP-Adapter based morphing techniques that's happening in the backend.

You can interact with it in a number of ways:

- Input images by clicking the upload button in the node itself
 
- Connect any image output to the node and it'll populate the images section
 
- Reorder or delete images once populated
 
- Use the prompt to help guide the output!
 

[PreviousText to Video](https://docs.flora.ai/nodes/video-node/text-to-video) [NextAudio to Video](https://docs.flora.ai/nodes/video-node/audio-to-video)

Last updated 1 month ago

Was this helpful?