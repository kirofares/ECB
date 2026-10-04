# ECB Reader Data Model

The reader stores text separately from presentation.

## Navigation hierarchy

`Testament → Book → Chapter → Verse`

## Verse model

Each verse has two token arrays:

- `coptic[]`
- `arabic[]`

Every token has:

- `id`: globally unique within the loaded dataset
- `text`: the displayed word/token
- `align[]`: IDs of corresponding token(s) in the opposite language
- `gloss` (optional): short lexical or editorial gloss
- future fields can include lemma, morphology, Strong-like internal IDs, notes, manuscript witness, confidence, revision metadata

## Alignment rules

The model supports:

- one Coptic word → one Arabic word
- one Coptic word → several Arabic words
- several Coptic words → one Arabic word
- unaligned editorial particles/tokens when necessary

The UI creates a real anchor link for each token and also highlights every aligned counterpart.

## Editorial rule

Alignment expresses translation correspondence, not necessarily strict lexical identity. Interpretive notes and textual variants should remain separate from the base alignment layer.
