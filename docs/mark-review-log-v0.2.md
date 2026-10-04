# Mark Review Log — v0.2

## Scope
Book: Mark  
Primary base: Sahidic Coptic  
Project: The Egyptian Coptic Bible – Arabic Translation (ECB)

## Review levels
- **DRAFT** — Arabic wording exists but has not completed the Sahidic word-by-word pass.
- **LINGUISTIC REVIEW** — vocabulary, syntax, particles, names, and repeated terminology checked against Sahidic.
- **TEXTUAL REVIEW** — lacunae and meaningful variants checked and recorded.
- **APPROVED** — ready for editorial publication within the project.

## Current status
All 16 chapters remain **DRAFT / IN REVIEW**.

The previous Arabic draft is not to be treated as a final published translation until each verse completes linguistic review.

## Completed first-pass checks

### Source-integrity scan
Completed across Mark 1–16 for explicit lacuna markers in the current Sahidic digital corpus.

Registered issues include:
- Mark 7:16 — lacuna marker
- Mark 8:10 — partial opening lacuna
- Mark 9:10 — lacuna marker
- Mark 9:44 — lacuna marker
- Mark 9:46 — lacuna marker
- Mark 11:26 — damaged/missing text marker
- Mark 15:28 — empty/absent text marker

These are stored structurally in:
`data/mark-critical-apparatus-v0.2.json`

### Confirmed correction
**Mark 9:29**

Previous draft:
> هذا الجنس لا يستطيع أن يخرج إلا بالصلاة.

Corrected Sahidic-based reading:
> **هذا الجنس لا يستطيع أن يخرج إلا بالصلاة والصوم.**

Reason:
The Sahidic text contains both the prayer term **ϣⲗⲏⲗ** and fasting **ⲛⲏⲥⲧⲓⲁ**.

### Editorially retained readings
The current editorial policy retains pending fuller witness review:
- Mark 2:26 — أبياثار رئيس الكهنة
- Mark 5:1 — الجراسيين
- Mark 16:9–20 — retained because present in the Sahidic base used for this stage, with a critical note required

## Terminology control
The controlled glossary is now maintained in:
`docs/glossary.md`

Core rules include:
- ⲡϫⲟⲉⲓⲥ → الرب
- ⲛⲟⲩⲧⲉ → الله / إله
- ⲉⲩⲁⲅⲅⲉⲗⲓⲟⲛ → الإنجيل
- ⲡϣⲏⲣⲉ ⲙⲡⲣⲱⲙⲉ → ابن الإنسان
- ϣⲗⲏⲗ → الصلاة / يصلّي
- ⲛⲏⲥⲧⲓⲁ → الصوم

## Next review pass
The next required pass is verse-by-verse linguistic review:

1. Segment the Sahidic clause.
2. Identify lemma and morphology where relevant.
3. Compare the Arabic draft to the Sahidic syntax and semantics.
4. Record any departure needed for natural Arabic.
5. Mark significant textual uncertainty separately.
6. Promote the verse from DRAFT → LINGUISTIC REVIEW only after the check.

## Publication warning
No verse should be labelled “approved translation from Sahidic” merely because an Arabic draft exists.

The core rule remains:

> **Translate what the Coptic witness actually preserves; do not silently supply what we expect the verse to say.**
