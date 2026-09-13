---
name: monumental-halftone-editorial-collage-poster
description: Create historical-cultural-heritage posters with a dominant photographic hero, giant editorial typography, and irregular halftone collage using four bundled layout masters. Use for heritage sites, architecture, sculpture, museum objects, or related cultural subjects; not for general-purpose posters.
metadata:
  version: "1.9.2"
---

# Monumental Halftone Editorial Collage Poster

Create one 3:4 historical-cultural-heritage poster. The real source subject is the first fixation, giant type is second, and processed contextual collage is third. Preserve credible material and structure while using forceful editorial scale, printmaking contrast and controlled irregularity.

## Portable reference system

This Skill is self-contained. The four composition masters ship inside `references/layouts/`; never ask the user to find or upload those external reference posters.

1. Resolve this Skill folder and inspect `references/reference-manifest.yaml`.
2. Auto-select one layout from subject geometry unless the user supplied `reference_layout_id`:
   - R1: long wall, horizontal facade or strong diagonal sweep.
   - R2: face, statue, relief or close-up entering from an outer edge.
   - R3: central gate, tower, axial building or tunnel perspective.
   - R4: tall standing/seated figure or vertical object suited to a center-right hero.
3. Visually inspect and attach the chosen `references/layouts/R#.png` as the layout-only reference. Attach only the chosen user sources after it.
4. Read the matching section of `references/layout-blueprints.md`. That blueprint is the executable fallback if the image cannot be viewed or attached.

The bundled master controls spatial grammar only. Never copy its site, sculpture, literal wording, birds, trees, circles, slogans or fake inscriptions into a new subject. If a packaged layout file is missing and its blueprint is unavailable, the package is incomplete: stop rather than invent a generic heritage poster.

## Inputs and source truth

Keep all replaceable fields in `input-template.yaml`. The only required user content is `hero_image` and `display_title`; a local title is strongly recommended. `reference_layout_id: auto` and `reference_image: auto-bundled` are valid defaults.

Original subject photographs are authoritative for identity, anatomy, architecture, material, damage and inscriptions. Treat supplied images as candidates: select only pieces with a clear visual job and record unused files. An approved previous result may become the revision composition master, but never the identity source.

Copy may be exact or concise editorial atmosphere. Do not fabricate dates, quotations, provenance, dynasties, coordinates, official labels, or historical claims. A small red seal is allowed as a graphic accent only when its exact characters are supplied or explicitly approved; it is not documentary evidence.

## PRE-GENERATION HARD GATE

Do not call image generation until every row is resolved:

1. **Scope:** heritage subject, 3:4 format, exact title and accessible hero source.
2. **Layout:** one R1–R4 master selected, visually inspected when possible, plus its text blueprint.
3. **Attachment ledger:** each image index labeled `layout-only`, `hero identity`, or `support source`; crop and destination named.
4. **Region lock:** title zone, local-title rail, hero territory, secondary territories, main direction and z-order copied from the selected master/blueprint. Do not average layouts.
5. **Content whitelist:** exact visible copy, chosen sources, palette, seal/ornament and construction devices. Anything not listed is excluded.
6. **Material split:** hero stays realistic; every auxiliary image receives a conspicuous individual print treatment; at least one large auxiliary mass has visible halftone dots.
7. **Collage rhythm:** choose two or three local variations only—tear contour, crop, modest angle, partial overlap, dot scale, ink dropout or registration shift.
8. **Outgoing prompt audit:** the actual prompt contains attachment roles, layout invariants, exact copy, hero dominance, per-layer treatments, local variations and the task-specific avoid list.
9. **Impact gate:** at 10% size, the hero has a singular readable silhouette, the darkest dark or strongest color contrast belongs to it, and one deliberate scale breach connects it to the title. If hero, background and support collapse into one flat plane, `READY NO`.
10. **Subject-lift gate:** the realistic hero is a discrete depth-bearing object or passage placed over flatter processed material. It must not remain physically continuous with an untreated facade/background photo.

Record internally: `REFERENCE / ATTACHMENTS / EXACT COPY / REGION LOCKS / HERO / SELECTED + UNUSED SOURCES / LAYER TREATMENTS / ACCENTS / LOCAL VARIATIONS / FORBIDDEN / READY YES|NO`.

Missing optional content is omitted. Missing hero or unresolved layout means `READY NO`.

## Composition invariants

Lock macro composition; vary local collage behavior.

- Match the chosen master's title side, line count, cap-height ratio, alignment, rail width, hero entry, main directional mass, secondary territories and negative-space channels.
- Use an upright heavy condensed sans/grotesk display face. Giant English title is an architectural mass, not a caption. Chinese rail uses high-contrast Song/Ming serif forms and follows the blueprint's vertical reading order.
- The hero must dominate at thumbnail size. Enlarge and crop it; allow it to cover a limited edge or interior portion of title and support material while preserving title recognition. Do not shrink the hero to show every source.
- Overlap is intentional and shallow across zone boundaries. Do not isolate all fragments with white moats, but do not let a secondary fragment invade a neighboring major zone.
- Mix one or two structural straight edges with irregular torn or cut silhouettes. Avoid card grids, equal gutters, repeated identical tears and evenly distributed stickers.
- Keep one strong dark anchor and one quieter neutral paper channel so the hierarchy remains legible.

## Impact gate

Reference accuracy is necessary but not sufficient. Before generation, define these four items explicitly:

- **Hero silhouette:** isolate the subject's most recognizable contour or void. Do not use an uncropped facade when a portal, face, animal or tower can become a stronger cutout.
- **Scale breach:** one hero edge enters the title or exits the canvas. The breach must be visible at thumbnail size while leaving the title recognizable.
- **Depth event:** choose one real source-supported depth cue—black tunnel, extreme foreground edge, receding axis, face crop or diagonal wall. Protect it from supporting collage.
- **Value separation:** reserve the deepest dark, lightest light or sole saturated photographic color for the hero. Convert adjacent support material into flatter, narrower-value print planes.
- **Subject lift:** identify the volumetric part of the source—face, body, arch thickness, open doors, tunnel, tower edge or projecting relief—and cut it away from its surrounding photographic plane. Convert the surrounding wall/facade/context to support print or omit it. A meaningful portion of the hero perimeter must meet paper or processed ink, so it visibly sits in front.

Use a three-scale hierarchy: one monumental hero, one giant title system, and small-to-medium support fragments. Do not let several medium-sized images compete. Symmetrical subjects may keep their axis, but create tension through crop, depth separation, overlap and asymmetric auxiliary contours rather than tilting the subject arbitrarily.

For frontal or planar architecture, do not keep the entire elevation photographic. Split it: the facade becomes halftone/rubbing support; the source-supported arch rim, reveal, door leaves and receding passage remain one realistic foreground hero. Do not fake impossible perspective or invent missing sides.

Use the normalized measurements and z-order in `references/layout-blueprints.md`; they are ranges for the selected master, not a universal freeform grid.

## Material and image treatment

Hero:

- Preserve source silhouette, proportions, masonry/carving details and real surface character.
- Allow cutout, monumental crop, restrained tonal correction and foreground overlap.
- Keep halftone, invented engraving, pattern skin and ornamental overprint off the hero.

Auxiliary layers:

- Assign each selected fragment a distinct treatment: coarse monochrome halftone, two/three-ink screenprint, rubbing, woodcut contrast, partial inversion, silhouette or cropped linework.
- Flatten highlights and shadows; visible dots must form tone, not sit as a global grain overlay.
- Process every auxiliary photograph, including plaques and architectural details. Preserve readable source inscriptions or crop them out deliberately.
- One substantial support mass must clearly show halftone at ordinary viewing size.

Ornament may be source-derived or user-authorized compatible geometric/floral pattern. Register its origin and role, flatten it to one ink, crop it inside an existing background patch, partially hide it, and keep it off hero and type. No automatic sun, birds, scenery or map.

## Prompt compilation

Read `references/prompt-template.md` before every call. Compile one coherent prompt, not a pasted rulebook:

1. task, format and numbered attachment roles;
2. chosen R-layout and its macro region/z-order invariants;
3. exact visible strings and typography slots;
4. hero source fidelity, scale and allowed foreground overlap;
5. every auxiliary source mapped to territory and print treatment;
6. approved seal/ornament, two or three named local variations, avoid list and final priorities.

Delete empty fields and unchosen alternatives. The first attachment is the bundled layout master and must be described as composition-only. Never attach all four layouts. Save the exact outgoing prompt beside the generated project asset.

## Review, failure and retry

Inspect the result at thumbnail, reading and detail scale.

Hard failure if: the hero is not first; the result is flat at thumbnail size; hero and support remain parts of one continuous untreated photograph; a planar facade surrounds the hero on the same material plane; no visible scale breach, subject lift or depth event exists; the title/rail skeleton does not match the chosen blueprint; major zones drift; the result becomes a neat card grid; auxiliary photos remain realistic; halftone is absent; subject identity or source inscriptions are invented; unsupported factual copy appears; or ornament contaminates hero/type.

For a local failure, make one targeted edit and preserve all approved invariants. For structural drift, weak hero scale or corrupted material, regenerate from the original layout master and original photography. Allow at most two focused retries, then report the unresolved limitation. Packaging validation does not prove visual quality.

## Supporting files

- `references/reference-manifest.yaml`: bundled master paths, roles and selection cues.
- `references/layout-blueprints.md`: standalone region maps, hierarchy and z-order for R1–R4.
- `references/prompt-template.md`: prompt compiler and preflight record.
- `examples/ming-xiaoling-prompt.md`: resolved example; adapt its method, not its subject.
