# ECB — Canon & Source Status

## Canon scope

ECB currently catalogs the Coptic Orthodox biblical canon as:

- Old Testament: 46 books
- New Testament: 27 books
- Total: 73 books

Editorial supplements tracked separately:
- Additions to Esther
- Additions to Daniel
- Psalm 151
- Prayer of Manasseh

## Source policy

### New Testament
Primary translation base: **Sahidic Coptic**.

ECB uses the Sahidica New Testament tradition where available:

**Sahidica - A New Edition of the New Testament in Sahidic Coptic**  
**Copyright (c)2000-2006 by J Warren Wells. All rights reserved.**

The Sahidica-specific license permits use in **free electronic editions of the New Testament** when the full source title and copyright information are included and credited. Print use requires separate written permission.

ECB therefore records NT publication status separately from editorial review:
- electronic source use: `free_electronic_attributed`
- translation/review state: draft / linguistic review / textual review / approved
- print publication: permission required

Coptic SCRIPTORIUM is used as the digital corpus and linguistic/annotation layer; each displayed chapter should retain its document URN.

### Old Testament
CoptOT / Coptic SCRIPTORIUM provides Sahidic Old Testament material for a growing set of books and chapters. The Sahidic OT corpus is distributed under **CC BY-SA 4.0**, but textual availability and preservation still vary by book and chapter.

Each OT book must therefore record:
- source project / manuscript or edition,
- license,
- versification scheme,
- whether the text is preserved, partial, lacunose, reconstructed, or editorially supplied.

## Reader publication states

- `catalogued` — book/chapter navigation exists
- `source_identified` — usable Coptic source identified
- `source_linked` — source record/URN linked in ECB
- `translation_draft` — Arabic draft exists
- `linguistic_review` — Coptic/Arabic linguistic review underway
- `textual_review` — textual variants and witnesses reviewed
- `approved` — approved for public reading
- `free_electronic_attributed` — source may be reproduced in the free electronic ECB edition with the required attribution

## Rule

A book can exist in the ECB reader before its full text is published. The UI must clearly distinguish catalogued structure from reviewed text, and must never silently substitute a Greek, Bohairic, English, or existing Arabic Bible text for missing Sahidic material.
