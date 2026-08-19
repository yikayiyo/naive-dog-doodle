# Style Guide

Use this guide to translate a real dog into an original, naive observational drawing. The target is intentionally imperfect, but not careless: likeness comes from choosing the right simplifications.

## Visual character

- **Line:** thin-to-medium black ink or felt-tip line; slightly shaky, uneven, and casually joined. A few doubled or searching strokes are welcome. Avoid perfect Bézier curves, uniform vector outlines, heavy comic inking, or dense cross-hatching.
- **Shape:** begin with one deliberately wrong container shape, not a simplified anatomical silhouette. A dog may become a cloud, bean, potato, wedge, long rectangle, or bundle of sticks. Let a true source feature choose the metaphor: long legs become improbable lines, a broad body becomes a block, a fluffy chest swallows the torso into a cloud, and a compact dog becomes a loaf.
- **Face:** use only enough marks to capture expression—small eyes, a simple nose and mouth, a few muzzle or brow strokes. Preserve ear direction and muzzle length. Avoid large glossy anime eyes or a standard emoji face.
- **Color:** use two to four colors sampled conceptually from the dog and its visible gear. Apply color as loose colored-pencil, crayon, or dry scribbled texture with white gaps. Keep black dogs charcoal rather than a featureless solid silhouette. Do not fully render fur.
- **Space:** place the dog on a warm ivory or off-white paper field with generous margins. The image itself is the drawing, not a photographed sheet of paper.
- **Mood:** affectionate, observant, deadpan, and lightly funny. It should feel quickly drawn by a human who noticed the dog's peculiar shape.

## Translate the photo, do not trace it

Choose the shortest set of marks that preserves identity:

| Photo feature | Drawing treatment |
| --- | --- |
| Curly or fluffy coat | Scalloped silhouette plus sparse looping or scribbled color marks |
| Smooth dark coat | Charcoal side strokes with paper showing through; keep eyes and muzzle readable |
| Spots or patches | Loose irregular color regions in the correct broad locations |
| Long legs or narrow torso | Exaggerate the vertical rhythm while keeping joints and visible limb count plausible |
| Broad, stocky body | Use one large rounded block with short understated legs |
| Long ears | Treat each ear as a distinct floppy shape, not generic triangles |
| Harness or collar | Reduce to a few colored bands that follow the body correctly |
| Leash | One simple colored line leaving the frame; include only when visible or requested |
| Huge fluffy chest or head | Merge adjacent anatomy into one cloud, pear, or bean shape |
| Strong close-up perspective | Exaggerate one facial mass and make an abstract head-and-shoulders bust |
| Fast movement | Tilt one simple body mass and imply limbs with mismatched stick lines |

Occluded limbs may remain omitted. Never invent extra visible legs merely to make the anatomy complete. Deliberate distortion should amplify a true feature; it should not replace the dog with a generic breed cartoon.

## Composition defaults

- Use portrait 4:5 for upright, seated, or compact poses.
- Use landscape 4:3 for long standing or lying silhouettes.
- Keep the full visible body when the source provides it. If only the head is visible, make a head-and-shoulders drawing rather than inventing a body.
- Center loosely rather than geometrically. Leave breathing room around ears, paws, and tail.
- Exclude the source environment by default. Add one contextual object only when the user explicitly requests it or it is inseparable from the pose, such as a stroller opening around the dog's head.

## Prompt scaffold

Adapt this scaffold to the inspected dog. Keep concrete identity anchors; remove unused lines.

```text
Use case: stylized-concept
Asset type: standalone pet illustration
Primary request: reimagine the individual dog from Image 1 as an original highly abstract observational doodle; do not trace the photo or preserve realistic dog anatomy
Input images: Image 1 is the subject and pose reference; additional images, if any, are identity references for the same dog
Subject: one dog; <pose>; identity tokens: <three to five visible anchors>
Abstraction concept: replace most anatomy with <one source-driven cloud, bean, potato, wedge, block, or stick metaphor>; attach the identity tokens to this intentionally wrong shape
Scene/backdrop: plain warm ivory paper field, generous empty margin, no photographed paper or real-world setting
Style/medium: loose hand-drawn black felt-tip contour, naturally wobbly and asymmetrical; minimal facial marks; sparse colored-pencil or crayon scribbles with white paper showing through; charmingly amateur observational sketch
Composition/framing: <portrait 4:5 or landscape 4:3>; preserve the visible pose and full silhouette; loosely centered
Color palette: only the dog's major coat colors plus visible collar, harness, or leash colors
Constraints: abstraction before anatomy, identity before decoration; amplify one actual peculiarity into the dominant shape; correct visible limb count; keep major markings in their broad locations; do not invent hidden body parts, accessories, or background objects
Avoid: realistic canine silhouette, simplified pet portrait, breed-accurate anatomy, photorealism, polished digital painting, smooth vector art, generic mascot, chibi or anime eyes, perfect symmetry, solid airbrushed fill, dense fur rendering, watercolor wash, text, signature, watermark, border, mockup, hands, sketchbook photo, before-and-after layout, social-media UI
```

Do not mention or imitate a named artist. Use the formal characteristics above to keep the result original.

## Acceptance rubric

A strong result should answer “yes” to all of these:

- Would the owner recognize this specific dog without seeing the source beside it?
- Does one bold container shape visibly replace normal dog anatomy?
- Is at least one source-specific proportion or gesture charmingly exaggerated rather than merely simplified?
- Does the line look human and spontaneous without becoming visually confusing?
- Is the color sparse, dry, and imperfect rather than digitally filled?
- Is the canvas free of scenery, text, UI, hands, and sketchbook mockup framing?

Revise in this priority order: abstraction strength, identity tokens, accidental anatomy, pose, medium, composition. If the result still looks like a conventional pet portrait, start over with a more extreme shape metaphor; detail reduction alone will not fix it. Stop once all checks pass because extra polish usually weakens this style.
