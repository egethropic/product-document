# Prompt and handoff templates

Adapt these templates to the actual product and tool. Attach the referenced assets; mentioning an asset without supplying it does not transmit it. Keep authoritative copy separate from generated text.

## Complete concept

> Design a flat, straight-on [format, dimensions, sides/panels] for [audience and purpose]. Use the attached actual CAD renders as references for product identity and views. Use the supplied content and design references for hierarchy, palette, typography, imagery and mood: [content and reference roles]. Create a complete themed composition with product placement, background, decoration and text. Maintain readable hierarchy, margins, panel order and negative space. The result is a visual concept; do not invent technical features or claims. Produce [requested alternatives] with distinct compositions.

## Background-only edit

> Edit the selected attached concept. Preserve the canvas, composition, palette, lighting, textures, scenery and negative space. Remove all text, logos, product depictions, their cast shadows and reflections, and foreground decorations to be rebuilt separately. Reconstruct their underlying background naturally. Return an opaque full-page background without ghost lettering or fragments.

## Decorative illustration extraction

> From the attached selected concept, isolate [identify one decorative illustration and its boundaries]. Preserve its character and complete its obscured edges where needed. Remove the background, text, logos, product depictions and other decorations. Return the illustration as a separate asset with true transparency and clean edges.

Repeat separately for each custom illustration. Inspect edges, transparency and concept fidelity; correct artifacts without incorporating generated product imagery.

## CAD render handoff

For each product depiction, provide the renderer with:

- Selected concept ID, page, placement and crop; product identity and exact CAD revision.
- Orientation, camera projection and angle, framing, scale, visible faces and required details.
- Verified material and texture references, lighting direction, background/alpha and shadow needs; flag unconfirmed presentation choices.
- CAD source, renderer and version, scene/camera settings, output file and hash, and missing or simplified models.

Compare the resulting render with the CAD and selected placement for silhouette, proportions, openings, connectors, controls and markings. Correct the render or composition if the view is impossible; do not modify hardware to match a generated invention. Place the fresh render as its own layer and retain its provenance. Rendered artwork is not a dimensional drawing or a performance qualification.

Inspect lighting separately for each camera. A rig that lights the hero well can leave an opposite-facing connector view dark; reposition the key or reflector for that view while preserving the campaign's light character. Check material scale against scene units, keep texture restrained, and avoid smoothing planar CAD faces merely to soften curved connector surfaces.

Supplier CAD can combine metal shells, insulating inserts and contacts into one untextured body. Inspect manufacturer photos and material specifications before assigning the whole body one shader. Where existing surface regions match that evidence, use rendering-only face materials or masks; preserve CAD geometry and record inferred segmentation or unresolved appearance limits.

When asked to save those fixes into CAD, distinguish the saved renderer scene from the engineering model. STEP can preserve supported face/part colors, but not procedural shaders or studio lighting. Save an appearance copy and reopen it to verify colors and geometry. Render masks that cross unsplit CAD faces do not automatically transfer: disclose any missing accent coverage, and do not claim a partial colored STEP reproduces the complete finish. Preserve the full renderer scene alongside it.
