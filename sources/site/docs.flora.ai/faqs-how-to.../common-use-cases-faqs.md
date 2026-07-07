# Source: https://docs.flora.ai/faqs-how-to.../common-use-cases-faqs

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/faqs-how-to.../common-use-cases-faqs.md).

Is there a way to export a video at more than 24 FPS?

Yes - you can connect your videos to another video node and use the Topaz Upscaler, which offers an FPS (frames per second) parameter. Set the parameters on the sidebar to whatever value you are looking for.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FMumxgVYekn9bzvNFh8oH%252Fimage%2520%2848%29.png%3Falt%3Dmedia%26token%3Dd0566ab9-7b1c-4114-8f11-e3f6b758228c&width=768&dpr=3&quality=100&sign=d9db806c&sv=2)

What upscalers does FLORA offer, and what are their maximum resolutions?

FLORA includes 5 image upscalers and 5 video upscalers.

**Image upscalers**

Model

Scale options

How big can the result be?

Magnific Creative

2×, 4×, 8×, 16×

Max 10056×10056

Magnific Precision / Precision V2

2×

Max 10056×10056 (input max 5028×5028)

Topaz Upscaler

1×–4×

No pixel limit — always 4× your input

Topaz Generative

1×–4×

No pixel limit — always 4× your input

**Video upscalers**

Model

Scale options

How big can the result be?

Topaz Upscaler

1×–4×, plus FPS control (16–60)

Max 8192×8192

Magnific Creative / Precision / Creative Turbo

Pick a target: 1K, 2K, or 4K

Up to 4K

Bria Video Upscaler

2× or 4×

Max 14142×14142 (clips trimmed to 29s)

**How the Magnific image limit works:** neither side of the result can exceed 10056px — the same maximum Magnific enforces on its own platform. If the scale you pick would go over that, FLORA automatically uses the biggest scale that fits — your image is never cropped or stretched. In practice:

- 16× works on images up to 628px
 
- 8× up to 1257px · 4× up to 2514px · 2× up to 5028px
 

Do FLORA's upscalers give the same results as using Magnific or Topaz directly?

Yes — FLORA runs the same Magnific and Topaz models you would use on their own platforms, so the quality at any given scale is identical. The only differences are the limits:

- **Magnific Creative (image):** full parity — same scale options (2×–16×) and the same maximum output (10056×10056) as Magnific's own platform.
 
- **Magnific Precision (image):** 2× in FLORA; Magnific offers higher scales directly.
 
- **Magnific video upscalers:** no difference — 4K is the maximum everywhere, including on Magnific's own platform.
 
- **Topaz (image):** up to 4× in FLORA — no pixel limit on the result.
 
- **Topaz (video):** same output limit as using Topaz directly (8192×8192). FLORA's scale control goes up to 4×, while the provider offers up to 8×.
 

What's the maximum file size for uploading to Flora?

The upload limit is 350mb for images, but model providers often have lower ceilings.

[PreviousUnsplash](https://docs.flora.ai/faqs-how-to.../unsplash) [NextTips & Tricks](https://docs.flora.ai/faqs-how-to.../tips-and-tricks)

Last updated 25 days ago

Was this helpful?