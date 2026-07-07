# Source: https://docs.flora.ai/faqs-how-to.../styles

For the complete documentation index, see [llms.txt](https://docs.flora.ai/llms.txt). This page is also available as [Markdown](https://docs.flora.ai/faqs-how-to.../styles.md).

**Note:** The Styles feature is currently unavailable and has been deprecated for now. You can still upload LoRAs to supported models (such as Flux Dev), but other style tools are not accessible at this time. Stay tuned for future updates with improved style features.

## 

Overview

FLORA’s **Styles** feature allows you to **apply specific visual styles to your image generations**. Styles Feature enhances t2i (text-to-image) and i2i (image-to-image) generation by allowing users to apply **predefined aesthetic filters** or **train their own custom styles**. This feature enables greater creative control, ensuring that outputs align with specific artistic or brand identities.

**Model Compatibility:** Style LoRAs are fine-tuned exclusively on **Flux Dev** and work best with that model. When using styles with other image models, FLORA will automatically generate a text summary describing the style's visual characteristics, which is then included in the prompt sent to the model. Results may vary depending on how well the target model interprets these style descriptions.

### 

**1\. Predefined Styles**

FLORA provides a curated selection of **predefined styles**, optimized for high-quality and consistent results across different image generations. These styles modify the **aesthetics, color, mood, tone, and content (characters, objects)** of generated images. Each preset comes with imagery and titles that highlight when it shines (for example, Motion Blur for kinetic shots or Extreme Detailer for macro textures). Simply browse the collection, pick what fits, and the editor handles the rest.

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F7Me96qciu9DqMayCBSq0%252FSTYLES_PRESETS.gif%3Falt%3Dmedia%26token%3D51c657a7-42bf-4af1-9314-4aa03168f9df&width=768&dpr=3&quality=100&sign=21ad3b1a&sv=2)

#### 

**1.1 Styles for Flux Dev**

Users can choose from a growing library of styles, categorized as follows:

**Fisheye**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FWUdd0cHK1rAlMOh424bU%252Fmichellema_360-degree_fisheye_shot_of_the_interior_of_an_aban_0611ec8b-5516-4502-8838-84c1ace829b6_1.png%3Falt%3Dmedia%26token%3Dae7ee70a-9a64-4858-9598-409117e42e49&width=768&dpr=3&quality=100&sign=3538e9cf&sv=2)

> Depth cues, model shading, digital flesh.

**3D**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FSkXVJgN9Wd9opgIlYVQg%252Fmichellema_A_few_spheres_floating_in_the_air_a_C4D_rendering__a4c961db-03c4-4653-a99e-ddb15ebf803f_3%2520%281%29.png%3Falt%3Dmedia%26token%3Da3193d10-af4e-4f45-a96f-445adc5f835b&width=768&dpr=3&quality=100&sign=c489955&sv=2)

> Not about real-world cameras—more like Blender renders. LoRA captures things like subsurface scattering, ambient occlusion, baked shadows. Geometry feels synthetic, form takes priority over texture.

**X-Ray**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FJslIfCPrfqaxLH9CqJIK%252Fmichellema_X-ray_of_an_ancient_sea_monster_long_body_with_man_e0b87eaf-4e10-44fd-9610-47f40f3f244c_1.png%3Falt%3Dmedia%26token%3D4fb4cc15-6d2d-4653-8a4f-4d445875b208&width=768&dpr=3&quality=100&sign=d6cb085a&sv=2)

> Imagined transparency. Subjects are peeled open—bones, wiring, inner systems exposed. A LoRA that trains on radiographic motifs but fakes the effect across arbitrary subjects. Useful for metaphor: revealing the hidden.

**Studio Lighting**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F4zZc2VZoG9rC4T3Qp3Ng%252Fmichellema_Studio_lighting_professional_photograph._A_close-u_f97445b0-c818-40a7-a589-16e3699d85d0_3.png%3Falt%3Dmedia%26token%3D098b2822-091f-432d-b723-6f23a60158a5&width=768&dpr=3&quality=100&sign=30378e62&sv=2)

> Controlled shadows, sharp highlights. Key light, fill light, rim light—classic three-point setup. Every pixel feels considered. LoRA adapts subject matter to sit inside a constructed scene, often with high contrast and shallow depth of field.

**Motion Blur**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F5JraJGGy5gMXaJHyMVps%252Fmichellema_Close-up_of_feet_running_in_grass_motion_blur_in_t_6d6a28c1-37a5-46d1-baaa-a3104e728ca6_0.png%3Falt%3Dmedia%26token%3D70d24f3e-384e-45f6-8f44-d0db8d42af1e&width=768&dpr=3&quality=100&sign=1730db06&sv=2)

> Speed encoded into the image. Simulates long exposure or rapid motion. Directional streaking, trailing forms. Often used in cyberpunk, dance, or action-heavy outputs. The blur is compositional—it pulls the eye.

**Monochrome**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F11DNuRYtZ6ZB5QsqdvhY%252Fmichellema_A_grainy_black-and-white_still_from_an_old_film_of_acc35710-6021-463d-941b-d928eee9a71c_3.png%3Falt%3Dmedia%26token%3Da8e93b77-e170-4e9a-ab62-d19e50b78cbd&width=768&dpr=3&quality=100&sign=17caa6fd&sv=2)

> One hue, infinite values. LoRA removes color information, but enhances detail through contrast. Could be charcoal, cyanotype, or film noir. Emphasizes shape, light, emotion—less distraction, more weight.

**Architectural**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FB4nRlwdQ06Ru1XCtOwbb%252Fmichellema_A_hand-drawn_black_and_white_architectural_drawing_83b0b35e-ca2e-4df4-9e40-3912fe9323bd_1.png%3Falt%3Dmedia%26token%3Da26a15d4-87ff-46f8-b342-b0f23fb47381&width=768&dpr=3&quality=100&sign=6413c524&sv=2)

> Structured, rectilinear, scale-aware. Linearity dominates—LoRA learns blueprints, elevations, orthographic projection. Often defaults to modernism unless nudged. Useful for clean geometry and visual order.

**Soft Focus**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FmcGPNmyDP8vRn5GJ7TTM%252Fmichellema_A_close-up_of_pearls_scattered_on_the_skin_with_li_121a92fa-1018-4458-b810-c5611b3b1738_1.png%3Falt%3Dmedia%26token%3D0dcdb6e7-cb8d-4c93-9cc2-f1f98a1a6816&width=768&dpr=3&quality=100&sign=b743358b&sv=2)

> Dream logic. Edges melt. Light blooms. Often draws from portraiture, especially analog. Feels cinematic or romantic. This LoRA suppresses crisp detail in favor of mood.

**Animated**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FdDfxTfLM3yXVGnB3T53i%252Fmichellema_Cartoon-style_Disney-inspired_artwork_depicting_a__415b3d9c-3a2c-44a4-bf3c-36c6152c11e0_2.png%3Falt%3Dmedia%26token%3Db7c61912-4a71-4eaf-88f3-ff46c41ee2c4&width=768&dpr=3&quality=100&sign=afcbf0ca&sv=2)

> Stylized, minimal texture, exaggerated form. Pulls from anime, Western animation, or game cutscenes. Flat shading, color blocking, large eyes, expressive lines. A LoRA that suppresses photorealism in favor of symbol.

**Vector**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FhNZOsPkaif7NfYMsBm1F%252Fmichellema_A_white_flower_with_pink_stamens_and_a_green_stem__4de48de7-3b13-4a52-b159-ddae2975ed6e_1%2520%281%29.png%3Falt%3Dmedia%26token%3D0089eaaa-cbb9-4536-865c-ab57c0e7a4cb&width=768&dpr=3&quality=100&sign=891d8667&sv=2)

> Infinitely scalable. Line clarity, color fields, no noise. Think Figma assets, logo packs, poster icons. A LoRA that favors SVG-like outcomes. It flattens depth, prioritizes readability.

**Photorealistic**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FyxPDcrHDAqgOKKlfUwnn%252Fmichellema_In_the_pink_and_red_mountains_of_Quilotoa_two_cycl_aefff658-4632-42ea-96a6-2e6b79f4cdaf_0.png%3Falt%3Dmedia%26token%3D0775afc6-6f32-49c1-b6f7-a967002a0adb&width=768&dpr=3&quality=100&sign=4c6fae5a&sv=2)

> As close to lens-based capture as possible. High fidelity textures, correct shadows, plausible lighting, skin imperfections. LoRA draws on real-world datasets and DSLR optics. Often pairs well with materiality prompts.

**Line Drawing**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FmuNPH4wcutnHL5odJI2C%252Fmichellema_A_simple_sketch_of_an_abstract_dream-like_interpre_d21f2e31-41a1-4cd1-964c-4defd39cae02_1.png%3Falt%3Dmedia%26token%3Da3e284d8-d901-472d-b987-db5fcb650e22&width=768&dpr=3&quality=100&sign=f443507a&sv=2)

> Gesture over mass. Black ink, pencil, or digital stroke. Negative space plays a role. LoRA reduces values to contours—ideal for diagrams, instructions, or ideation sketches.

**Product Mockup**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252F8p5iYmrfRh5Lwr7pgoCa%252Fmichellema_A_minimalist_mobile_phone_with_the_text_Night_on_t_b737abbc-0c1f-4fe3-9987-f6c1c2b07c85_3.png%3Falt%3Dmedia%26token%3Dfd93032c-5e8f-4706-9a39-ce0baa7496fd&width=768&dpr=3&quality=100&sign=75e51f28&sv=2)

> Perfect surfaces. Rendered packaging, floating objects, top-down minimal backdrops. LoRA learns from ecommerce, product design, and pitch decks. Prioritizes clean, centered, desirable.

**Extreme Detailer**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FDk5cmmCc8T53gyCkXiKe%252Fmichellema_Extreme_close_up_macro_hyper_detail_cinematics_of__e1e8d4a4-8a6a-4d64-a0ae-4fe24d78600b_0.png%3Falt%3Dmedia%26token%3D9683b003-ee96-4b0d-956d-96e02ad3bbf0&width=768&dpr=3&quality=100&sign=b3cfca5b&sv=2)

> Texture fanatics. Zoom in: every pore, crack, wrinkle. This LoRA overfits on microstructures—hyperreal to the point of obsession. Can verge on the grotesque if unchecked.

**Cinematic**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FWmvwwXhzw4VOcvf4xi97%252Fmichellema_A_film_photograph_of_an_empty_highway_tunnel_taken_7ffd7f03-afa0-4f0e-ae73-86c74eed9f31_0.png%3Falt%3Dmedia%26token%3D09212158-dcee-44a9-a047-5071c7070826&width=768&dpr=3&quality=100&sign=69fbd105&sv=2)

> Frame as story. Aspect ratio matters. Lighting dramatizes. Color grading carries tone. LoRA may reflect film stock, composition theory, or golden hour. Meant for stills that feel like scenes.

Each style adjusts image attributes such as **aesthetics, composition, mood, tone, and content.**

---

### 

**2\. Custom Style Training**

For users seeking **high-level, customized creative ownership**, FLORA enables **custom style training**, allowing users to upload reference images and train a model that adapts to their unique aesthetic.

#### 

**2.1 How Custom Style Training Works**

![](https://docs.flora.ai/~gitbook/image?url=https%3A%2F%2F526296967-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252FWthH0GpcCHwVdtbvahZS%252Fuploads%252FUhxVcYmiJNml2W9xtoew%252FSTYLES_CUSTOM_TRAINING.gif%3Falt%3Dmedia%26token%3De08b03ac-b170-46e6-ac7e-94fee5d6c582&width=768&dpr=3&quality=100&sign=f6fecfc3&sv=2)

1. **Upload Reference Images** – Provide a set of images that represent the desired visual style. Hit Create Style button to start the training.
 

For best result, a minimum of 8 images are required to start the training process.

1. **Training Process** – When the training is done, you'll get a notification.
 
2. **Preview** – You can find your customized Style on the left side tool bar. Your custom style will also show up on the tool bar above the image node, with all the other default styles.
 

[PreviousWorkspaces](https://docs.flora.ai/faqs-how-to.../workspaces) [NextUnsplash](https://docs.flora.ai/faqs-how-to.../unsplash)

Last updated 1 month ago

Was this helpful?