# Source: https://docs.flora.ai/nodes/image-node/image-to-image

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/nodes/image-node/image-to-image.md).

## 

Summary

Image to Image is an essential tool for creative evolution. It empowers transforming existing visuals, refining details, experimenting with styles, and enhancing narratives with precision. Whether you’re iterating on a concept sketch, reimagining a scene with new aesthetics, or blending multiple ideas into a cohesive composition, **Image to Image** unlocks new dimensions of creativity, enabling continuous exploration and storytelling through visual transformation.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F31YHJa2fX1iUVJcHTomW%252FScreenshot%25202025-02-23%2520at%25208.41.54%25E2%2580%25AFPM.png%3Falt%3Dmedia%26token%3D1b174093-192f-4ee4-97d2-5043a81f117a&width=768&dpr=3&quality=100&sign=3061b107&sv=2)

### 

Image to Image Models

Visit [Image Models](https://docs.flora.ai/models/image-models) to see a full list of image to image (i2i) models and their capabilities.

### 

Parameters

Image models generally accept the following parameters. Check each model for specifics.

Parameter

Type

Effect on Output

Prompt

Text

The text prompt is processed through various visual information extraction models (Canny, Depth, Redux), each uniquely interpreting different features of the input image to generate new visuals.

Style

Different kinds of stylistic presets (_3D, Anime, Cyberpunk, Extreme Detailer, Game Asset, Logo, Midjourney, Motion Blur, Panorama, Pixar, Pixel, Retrofuturism, Studio Ghibli, Tarot Card, Thermal Image, Vector, Victorian Drawing, Watercolor_).

The style presets modify the rendering phase by influencing color schemes, textures, and artistic techniques, transforming the structural output from ControlNet into diverse visual interpretations.

Strength

0%-100%

The strength parameter alters the amount that the text influences the output image versus the source image. The higher the strength is, the more influence the text has.

Image Size

_Auto,_

_Landscape_ - _16:9 (576x1024)_,

_Portrait - 4:3 (768x1024)_,

_1:1,_

_Landscape_ - _4:3 (1024x768)_, _Portrait_ - _9:16 (1024x576)._

This changes the output size of the node with a couple of options.

Seed

Seed

The seed is a deterministic number that indexes generations from the model. It's typically randomized, but you can set a seed if there's a particular output you're looking for! Keep in mind that all parameters must be the same in order for a given seed's output to persist.

[PreviousText to Image](https://docs.flora.ai/nodes/image-node/text-to-image) [NextVideo Node](https://docs.flora.ai/nodes/video-node)

Last updated 9 months ago

Was this helpful?