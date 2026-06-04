# Style Guide

## Purpose

This guide keeps the prose consistent across chapters. It is especially important because the book makes technical and controversial claims for readers who may not know Greek.

## Tone

Default tone:

- rigorous,
- patient,
- direct,
- fair to mainstream readings,
- assertive where the system reaches a conclusion.

Avoid:

- sarcasm toward commentators or translators,
- vague suspicion of "experts,"
- repeated hedging on conclusions already established by the system,
- overstating points that are still only leads.

## Certainty Language

Use different language for different levels of claim.

For grammatical possibility:

- "Greek grammar permits..."
- "The phrase can grammatically mean..."
- "This is a possible reading..."

For documented mainstream practice:

- "Many translations render..."
- "A common commentary reading is..."
- "The representative sources in this study tend to..."

For system-governed conclusions:

- "The system excludes..."
- "The structure requires..."
- "The chiastic pair supplies..."
- "On this analysis..."

For claims still needing verification:

- "This remains to be checked..."
- "The current source lead points to..."
- "This should not yet be cited as evidence..."

## Greek And Transliteration

Working default:

- Give Greek at first technical discussion.
- Give transliteration immediately after the Greek when the reader needs to recognize the term later.
- Use italicized transliteration in prose.
- Use code style in planning files only.

Example manuscript pattern:

```latex
The opening word is \textgreek{ἀποκάλυψις} (\textit{apokalypsis}), a noun that must be tested for verbal force before it is treated as a static title.
```

The LaTeX preamble defines `\textgreek{...}` and loads `textalpha`/`alphabeta` for lightweight Greek support under pdfLaTeX.

## English Rendering Of Key Terms

Working defaults:

| Greek / Term | Working English | Warning |
| --- | --- | --- |
| `apokalypsis` | disclosure | Do not settle the final translation before Chapter 9. |
| `semaino` / `esemanen` | signify / signified | Do not flatten to "made known" when the distinction matters. |
| `deixai` | show | Keep distinct from signify. |
| `doulos` | servant | Do not assume "all Christians" without argument. |
| `en tachei` | in speed / speedily, depending on context | Do not default to "soon" in argument prose. |
| `logos tou theou` | word of God | Analyze rather than ornament. |
| `martyria iesou christou` | testimony of Jesus Christ | Do not decide the genitive by shortcut. |

## Handling Mainstream Interpretations

Preferred sequence:

1. State the mainstream reading.
2. Explain why it is plausible.
3. Identify what it supplies, assumes, or leaves unconstrained.
4. Show how the system decides differently.
5. State what is excluded and why.

This order keeps the critique serious and prevents the book from sounding like it is rejecting consensus before understanding it.

## Footnotes

Use footnotes for:

- named source claims,
- grammar and lexicon support,
- textual variants,
- side debates that would slow the main argument.

Do not use footnotes to hide essential steps in the argument. If a step is necessary for the reader to follow the conclusion, it belongs in the main text.

## Diagrams

Use diagrams when:

- the argument depends on sequence,
- the argument depends on symmetry,
- the argument compares surface and expanded forms,
- the reader must see supplied constituents.

Preferred labels:

- A, B, C, C', B', A' for the chiastic nucleus.
- "surface form" and "expanded form" for the reduced/reconstructed contrast.
- "transmission" and "reception" for the larger model.

## Terms To Use Carefully

### "Revelation"

Avoid using "Revelation" ambiguously. Use:

- "the book of Revelation" for the canonical work;
- "`apokalypsis`" for the Greek term;
- "disclosure" as the provisional rendering;
- "the entity often called the revelation" when discussing the book/entity distinction.

### "Experts"

Use sparingly. Prefer more specific terms:

- commentators,
- translators,
- grammarians,
- lexicographers,
- pastors and teachers,
- scholars.

### "Arbitrary"

Use only when the argument has shown that a choice lacks a governing system. Often "underdetermined" is more precise before the system is introduced.

## Chapter Rhythm

For technical chapters:

1. Begin with the interpretive problem.
2. Give the smallest Greek unit needed.
3. Explain the possible readings.
4. Introduce the technical concept.
5. Apply the concept to the verse.
6. State what changes.

For consequence chapters:

1. Recall the structural finding.
2. State the mainstream implication.
3. State the system's conclusion.
4. Show the effect on reading Revelation.
