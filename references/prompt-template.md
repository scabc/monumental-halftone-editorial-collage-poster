# Actual prompt compiler

Resolve every bracket before calling. Omit unused clauses and unchosen alternatives.

```text
Use case: ads-marketing
Asset: one 3:4 historical-cultural-heritage editorial poster

ATTACHMENT ROLES
Image 1 = bundled layout master [R#], composition-only. Copy its spatial grammar and typography hierarchy; do not copy its subject, literal wording or decorative objects.
Image 2 = hero identity source: [source and crop].
Image 3... = support sources: [source -> role].

MACRO COMPOSITION — LOCKED
Use [R#] exactly as described in the bundled master and layout blueprint:
[title zone, line split, local-title rail, hero territory/entry, secondary territories, dominant direction, quiet paper channels].
Z-order back to front: [ordered layers].
Allow only [named shallow crossings]. Keep every other major region contained.

EXACT VISIBLE COPY
Display title, line 1: "[text]"
Display title, line 2: "[text]"
Local title: "[characters]" arranged [reading order].
[Other supplied/approved strings and slots.]
Use upright heavy condensed sans/grotesk for the English title and high-contrast Song/Ming serif forms for Chinese. Match the chosen master's relative type scale; do not reduce the title to fit imagery.

HERO — FIRST FIXATION
Use Image 2 as the realistic dominant hero. Preserve [defining structure, material, damage and identity]. Enlarge/crop it to [territory and entry]. It may cover [specific title/support edge] while the title remains recognizable. Keep print dots, ornamental patterns and invented detail off the hero.

IMPACT LOCK
Hero silhouette/void: [single recognizable contour or negative shape].
Scale breach: [specific hero edge crossing title or canvas].
Depth event: [source-supported tunnel, foreground edge, receding axis, face crop or diagonal].
Value separation: [hero-owned darkest dark/lightest light/saturated color]; flatten adjacent support into [narrower print range].
Subject lift: [volumetric portion kept photographic] separated from [surrounding plane converted to print/omitted]; [hero edges] meet paper or processed ink rather than one continuous photograph.
Keep one monumental hero, one giant title system, and small-to-medium support fragments; no competing medium images.

AUXILIARY LAYERS — ALL PROCESSED
[Image/crop -> selected R# territory -> treatment -> visual job.]
[Repeat for every support layer.]
At least one large support field uses unmistakable halftone dots that build tone. Flatten highlights and shadows; remove photographic gloss. No auxiliary photo remains untreated and no single global filter substitutes for individual treatment.

ACCENTS AND LOCAL VARIATION
[Exact red seal or resolved ornament -> origin -> one-ink treatment -> existing background patch; subordinate, partly hidden, off hero/type.]
Use only these local variations: [two or three named contour/crop/angle/overlap/print changes]. Maintain macro regions, dominant direction and reading hierarchy.

AVOID
[Unsupported factual copy; fake glyphs; copied objects from the layout master; card grid; equal gutters; white moat around every fragment; weak hero scale; unprocessed support photos; global grain-only effect; invented hero texture; watermarks/UI.]

FINAL PRIORITIES
1. [R#] composition and typography skeleton.
2. Real source hero as unmistakable first visual center through silhouette, scale breach, depth and value separation.
3. Every auxiliary layer visibly processed, with substantial halftone.
4. Controlled overlap and slightly irregular local collage rhythm.
5. Exact approved copy and subordinate accents.
```

## Preflight record

```text
REFERENCE: R# / path / inspected yes|no / blueprint read yes|no
ATTACHMENTS: index -> role -> crop -> destination
EXACT COPY: string -> slot -> mode
REGION LOCKS: title / rail / hero / secondary / paper / direction / z-order
HERO: source truth / crop / scale / allowed overlap
IMPACT: silhouette / scale breach / depth event / value separation
SUBJECT LIFT: photographic volume / surrounding plane treatment / contact edges
SELECTED SOURCES: source -> job
UNUSED SOURCES: source -> reason
LAYER TREATMENTS: every auxiliary layer
ACCENTS: origin / treatment / territory
LOCAL VARIATIONS: 2–3 named changes
FORBIDDEN: task-specific list
READY: YES|NO
```

If `READY` is not `YES`, do not call generation.
