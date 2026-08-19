---
name: naive-dog-doodle
description: Turn dog photos into standalone naive hand-drawn illustrations using radical shape abstraction, wobbly black lines, sparse colored-pencil marks, and a few recognizable identity tokens. Use when the user wants a dog photo reimagined as an intentionally crude, loose, childlike observational doodle rather than a simplified pet portrait. Do not use for photorealistic portraits, polished vector mascots, or animals other than dogs.
---

# Naive Dog Doodle

Generate one finished illustration that still reads as the dog in the supplied photo. Favor recognition and lively observation over polish.

Before generating, read [references/style-guide.md](references/style-guide.md). It defines the visual language, photo-to-drawing translation rules, prompt scaffold, and acceptance checks for this skill.

## Inputs

- Require at least one usable dog photo. If none is available, ask the user to attach one.
- Treat every supplied dog photo as a **subject reference**, not as an edit target, unless the user explicitly asks to preserve the original scene.
- When a local photo has not yet been inspected, view it before generation.
- If several photos show the same dog, combine only consistent identity cues. Prefer the clearest photo for pose and the clearest close-up for face and markings.
- If several different dogs are present and the intended subject is unclear, ask which dog to draw. Otherwise proceed without a confirmation round.

## Extract the dog's identity

Before writing the image prompt, identify a compact set of observable anchors:

1. Overall silhouette and pose.
2. Head, muzzle, ear, leg, body, and tail proportions.
3. Major coat colors and distinctive markings.
4. Expression or posture.
5. Collar, harness, or leash only when visible and useful for recognition.

Reduce the dog to two decisions:

- Three to five identity tokens that make this individual recognizable.
- One dominant shape metaphor prompted by the photo, such as a cloud, bean, potato, wedge, block, or bundle of sticks.

Do not guess breed, personality, sex, hidden anatomy, or hidden markings. Do not normalize unusual proportions toward a generic ideal dog, and do not use the realistic photographed silhouette as the main scaffold.

## Generate

- Use the built-in image generation tool in its normal image-reference flow.
- Generate a **new standalone illustration** using the dog photo as the subject reference. Do not generate a photo of a sketchbook, a before-and-after layout, or an overlay on the source photo.
- Let the dominant shape metaphor replace most realistic anatomy, then attach the selected identity tokens. The result should be more abstract than a simplified pet portrait.
- Do not trace the photographed silhouette. Make proportions intentionally wrong in a source-specific way: stretch, squash, merge, or omit forms to amplify the dog's most memorable feature.
- Default to one dog, one uncluttered warm-white paper field, and no decorative objects. Keep visible collar, harness, or leash only when it contributes to the likeness or the user asks for it.
- If only the head or upper body is visible, create an abstract bust instead of inventing a complete dog.
- Follow a user-specified pose, background, aspect ratio, or accessory. Otherwise choose the canvas orientation from the dog's pose as described in the style guide.
- Do not add names, captions, signatures, watermarks, borders, social-media UI, or unrelated scenery.
- Produce one final image unless the user requests variants.

## Validate and refine

Inspect the result rather than accepting it from the prompt alone. Check, in this order:

1. It resembles the same individual dog through three to five identity tokens rather than realistic rendering.
2. One bold, funny shape decision visibly replaces normal canine anatomy. If it could pass as a simplified pet portrait, reject it and generate a fresh abstraction instead of merely removing detail.
3. The pose remains readable and there are no accidental defects such as extra limbs, duplicated facial features, or impossible harness geometry.
4. The drawing feels loose, sparse, asymmetrical, and handmade rather than polished, vector-like, or generically cute.
5. Color appears as limited, imperfect pencil or crayon marks rather than smooth digital fill.
6. The output is only the illustration on a plain field, with no source-photo environment, mockup, text, UI, or watermark.

If a check fails, revise only the most important failure and repeat the relevant constraints. Do not remove deliberate wobble or asymmetry merely to make the drawing cleaner.

Return the final image inline. If the user names a destination or the image is for the current project, save the selected output there non-destructively and report the path.
