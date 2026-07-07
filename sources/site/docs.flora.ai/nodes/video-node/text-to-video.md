# Source: https://docs.flora.ai/nodes/video-node/text-to-video

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/video-node/text-to-video.md).

## 

Summary

Text-to-Video models generate videos by taking a text prompt as input, using the prompt to guide scene composition, motion, and style, resulting in dynamic video content that matches the described narrative or visual concept.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FfbfQzWdougCcIi5c3f7c%252FScreenRecording2025-02-24at1.56.19PM-ezgif.com-video-to-gif-converter.gif%3Falt%3Dmedia%26token%3D715c3588-11e2-40c4-8b1b-d07ed9583cb6&width=768&dpr=3&quality=100&sign=6e775c62&sv=2)

### 

Parameters

These are parameters that are applicable to all our base models.

Parameter

Type

Effect on Output

Prompt

Text

The text prompt is processed through the selected model.

Aspect Ratio

_Landscape_ - _16:9 (576x1024)_,

_Portrait_ - _9:16 (1024x576), Square - 1:1._

This changes the output size of the node with a couple of options.

Seed

Seed

The seed is a deterministic number that indexes generations from the model. It's typically randomized, but you can set a seed if there's a particular output you're looking for! Keep in mind that all parameters must be the same in order for a given seed's output to persist.

### 

How to use

Prompting is everything for Text to Video. Refer to the [Text to Text](https://docs.flora.ai/nodes/text-node/text-to-text) card to explore more workflow combinations, or browse example workflows on the [Community page](https://app.flora.ai/community).

[PreviousVideo Node](https://docs.flora.ai/nodes/video-node) [NextImage(s) to Video](https://docs.flora.ai/nodes/video-node/image-s-to-video)

Last updated 1 month ago

Was this helpful?