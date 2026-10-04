# ECB Translation Methodology

## 1. Translation base
The primary translation base for the New Testament is the **Sahidic Coptic text**. Every translated passage must identify the Coptic edition or witness used.

Greek, Bohairic, and other witnesses are comparative controls. They must not silently replace or normalize the Sahidic reading.

## 2. Preserve the difference between text and reconstruction
A preserved Sahidic reading, a damaged passage, and a reconstructed/parallel reading are three different editorial states.

Use these states consistently:

- `preserved`: sufficient Sahidic text survives for direct translation.
- `partial`: part of the Sahidic verse is missing or unreadable.
- `lacuna`: the Sahidic text used by ECB does not preserve enough text for a direct translation.
- `variant`: the Sahidic wording is preserved but has a significant variant against another major witness.
- `editorial`: the displayed wording contains an explicitly identified editorial supplement.

Never fill a Sahidic lacuna from Greek, Bohairic, English, or an existing Arabic Bible without marking that material as a separate comparative reconstruction.

## 3. Linguistic analysis before idiomatic Arabic
Before approving an Arabic verse, review:

- Coptic segmentation and syntax
- verbal forms and particles
- lexical meaning
- Greek loanwords in Coptic
- proper names and place names
- repeated Markan terminology
- possible ambiguity

The approved Arabic may be idiomatic, but it must remain traceable to the Sahidic wording.

## 4. Arabic style
Use clear Modern Standard Arabic with a dignified biblical register.

Prefer direct wording over archaic phrasing when meaning is unchanged. Preserve deliberate repetition and the rapid narrative movement of Mark, including repeated equivalents of “immediately” where present.

## 5. Controlled terminology
Recurring theological and narrative terms are governed by the project glossary in `docs/glossary.md`.

Examples:

- ⲛⲟⲩⲧⲉ → الله / إله بحسب السياق
- ⲡϫⲟⲉⲓⲥ → الرب
- ⲉⲩⲁⲅⲅⲉⲗⲓⲟⲛ → الإنجيل
- ⲡϣⲏⲣⲉ ⲙⲡⲣⲱⲙⲉ → ابن الإنسان
- ϣⲗⲏⲗ → الصلاة / يصلّي
- ⲛⲏⲥⲧⲓⲁ → الصوم

Changes to an established equivalent require an editorial note in version history.

## 6. Translation and commentary are separate layers
Store and display separately:

1. Sahidic base text
2. Arabic translation
3. literal/lexical gloss
4. textual-critical note
5. comparative readings

A reader must be able to read the Arabic Bible text without being forced through the critical apparatus.

## 7. Textual-critical notation
ECB uses:

- `[ ]` for an explicitly editorial or textually uncertain element
- `…` for a lacuna or unreadable material in the Sahidic source
- `†` for a significant textual note

Witness abbreviations:

- **Sah** — Sahidic
- **Boh** — Bohairic
- **Gk** — Greek

## 8. No silent harmonization
Do not harmonize Mark with Matthew, Luke, John, a liturgical lectionary, or a familiar Arabic translation.

If the Sahidic witness says something unexpected, translate it first and explain it second.

## 9. Revision status
Each verse should eventually carry one of:

- `draft`
- `linguistic_review`
- `textual_review`
- `approved`

Material changes must be traceable through Git history with a short reason.

## 10. Publication rule
A digital scholarly resource may be used for checking and analysis according to its license, but the project must separately verify republication rights for any Coptic base text that will be reproduced verbatim in a commercial or print edition.

## Current Mark review
Mark is currently **v0.2 — in review**. The first critical corrections and lacuna register are stored in `data/mark-critical-apparatus-v0.2.json`.
