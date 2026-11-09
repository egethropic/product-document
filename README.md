# Product Document

A reusable agent skill for turning CAD views, product copy and visual references into a designed brochure, flyer or product brief with editable typography and accurate product imagery.

The agent first creates a complete visual concept with image generation. It then extracts the background and decorative illustrations, replaces generated hardware with pose-matched CAD renders, and rebuilds the text and simple geometry as vectors. Backgrounds remain raster by default; textured illustrations and product renders can remain raster too.

Read the [skill](skills/product-document/SKILL.md), [workflow flowchart](skills/product-document/references/workflow.md) and [prompt templates](skills/product-document/references/prompts.md).

## Install

Copy the complete `skills/product-document` folder into your agent's skill directory. For Codex, that is `$CODEX_HOME/skills/product-document` or `~/.codex/skills/product-document` by default. Keep its references and license with it.

With Codex's skill installer, request:

> Install the product-document skill from egethropic/product-document, path skills/product-document.

The installed skill is available on your next turn. Other agents that support `SKILL.md` can use the same folder; configure their skill discovery according to their host's instructions. Registration does not install CAD/rendering software or image-generation access.

## Use

> Use $product-document to make an A4 promotional sheet from this CAD assembly. Include the product, connectors and sensor detail. Match the attached design references and use realistic materials and lighting. Deliver a PDF, preview and editable source.

Provide the authoritative CAD revision, product facts or copy, intended audience, page format, and image or text references. Earlier approved content and design selections can be reused. Only selected concepts proceed to finished production.

Terra is the preferred executor. An explicit request to use another supported model overrides that preference; the workflow does not require a Terra-only runtime. The host must provide image generation, CAD rendering and suitable document export tools. Procedural render materials and lighting remain in the renderer scene; STEP supports a more limited appearance representation.

## Validation scope

One complete product-sheet pilot has exercised multi-view CAD references, concept selection, background and illustration extraction, actual-CAD product replacement, editable SVG and single-page A4 PDF export. The user accepted the finished design. This is qualitative evidence from one pilot, not a general model benchmark or a guarantee across products and formats.

## License

[MIT](LICENSE). Supplied CAD, fonts, reference images and other product assets retain their own licenses; they are not included in this repository.
