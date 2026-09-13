# Monumental Halftone Editorial Collage Poster — 1.9.2

Historical-cultural-heritage posters with one dominant realistic subject, reference-locked typography and irregular printed collage.

## Using it

Copy the complete folder to your agent's skills directory. Keep `references/` and `examples/` with `SKILL.md`. Fill `input-template.yaml` or supply the same information conversationally. The Skill automatically selects one of the bundled `references/layouts/R1.jpg` through `R4.jpg`, or you can name an ID explicitly.

The GitHub package is self-contained: all four layout masters, a text-only blueprint and a manifest are included. A new user only supplies their own heritage subject image(s) and copy. The bundled posters are composition-only masters, never source assets for unrelated subjects.

## What is locked

The chosen master controls title scale/line split, left rail, major image territories, hero entry, foreground hierarchy, dominant direction and z-order. The real source subject is the first visual center.

The preflight also requires an impact lock: one unmistakable hero silhouette, one visible scale breach into type or canvas, one source-supported depth event, and strong value separation between the realistic hero and flatter printed support. A structurally correct but flat composition must be rejected.

For frontal architecture, the Skill also enforces subject lift: the depth-bearing arch, door, reveal or passage stays photographic while its surrounding facade is omitted or converted to flat print. The hero must sit visibly over the collage instead of remaining continuous with one large background photo.

## What can vary

Selected source crops, replacement copy, visibly processed auxiliary imagery, small tears, fragment angles, local offsets and print variation. Appropriate background ornament is resolved before generation and kept off the hero and type.

## Prompt quality

`references/reference-manifest.yaml` chooses the master, `references/layout-blueprints.md` makes all four structures executable even if the images cannot be viewed, and `references/prompt-template.md` compiles the actual outgoing prompt. Every call attaches one bundled master plus chosen original sources. Every auxiliary layer gets an explicit print treatment. Package validation does not guarantee visual quality; inspect every result.

Original content fields remain replaceable. `reference_layout_id: auto` and `reference_image: auto-bundled` make the default portable. New controls remain optional: approved revision master, collage variation and ornament mode.

No license is included. Review and add a license before granting reuse permissions.
