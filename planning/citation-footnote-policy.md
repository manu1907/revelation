# Citation And Footnote Policy

## Purpose

This file governs bibliography, footnotes, and footnote references for the manuscript. The goal is to keep the book readable for serious general readers while giving enough documentation for specialists to evaluate the argument.

## LaTeX Setup

The manuscript uses `biblatex-chicago` with note-style citations and `biber`.

Use:

- `\autocite[page]{key}` for ordinary footnote citations.
- `\footcite[page]{key}` when a footnote should contain only the citation.
- `\footnote{... \autocite[page]{key}.}` when the footnote contains explanation plus a citation.
- `\textcite{key}` only when the author's name belongs in the sentence.
- `\printbibliography` for the final bibliography.

Build command:

```sh
latexmk -pdf -interaction=nonstopmode -halt-on-error main.tex
```

## What Must Be Footnoted

Footnote these:

- Claims about what a named commentator, translator, grammar, lexicon, or edition says.
- Claims about Greek grammar that rely on a grammar or linguistic source.
- Claims about lexical range from BDAG, LSJ, Louw-Nida, BrillDAG, or similar sources.
- Claims about Greek textual variants, including the presence or absence of `te`.
- Claims about translation popularity, mainstream reception, or bestseller/use data.
- Direct quotations, even short ones.
- Unusual or contested claims, especially where the book disagrees with mainstream readings.

## What Usually Does Not Need A Footnote

Do not overload the manuscript with notes for:

- The author's own argument once the evidence has already been established.
- Repeated references to the same source in the same paragraph, unless the page changes or the claim changes.
- Basic orientation statements that are immediately shown by the Greek text.
- Common biblical cross-references when the verse reference itself is enough.

## Footnote Style

Footnotes should be useful but not distracting.

Use footnotes for:

- source documentation,
- brief technical expansions,
- noting minority positions,
- explaining why a source is included,
- marking text-critical issues.

Avoid footnotes that become hidden mini-essays. If a note needs more than one short paragraph, it probably belongs in the main text or an appendix.

## Page-Level References

For commentaries, cite exact pages whenever possible:

```latex
\autocite[190--91]{osborne2002revelation}
```

For multi-volume works, include volume if needed:

```latex
\autocite[1:12]{charles1920revelation}
```

For online sources, use `urldate` in `main.bib` and cite the source key. If the online source has stable section headings but no pages, name the section in the footnote text.

Before adding a commentary footnote to a chapter, record the page-specific finding in `planning/page-reference-ledger.md`. The ledger should say whether the passage is verified directly, checked only in a preview, checked only through OCR, or still only a secondary lead.

## Source Tiers

Argument sources:

- Greek editions,
- grammars,
- lexicons,
- technical commentaries,
- peer-reviewed articles,
- scholarly monographs.

Reception sources:

- major translations,
- study Bibles,
- pastoral commentaries,
- widely used public Bible resources.

Orientation sources:

- Bible Gateway,
- BibleHub,
- Wikipedia,
- blogs,
- sermon sites.

Orientation sources may guide lookup, but they should not carry the book's argument.

## Bibliography Workflow

1. Add every serious source to `src/main.bib` before drafting with it.
2. Use stable citation keys: `authorYearShortTitle`.
3. Record page-specific findings in the evidence matrix.
4. Insert footnotes only after the page-specific claim is verified.
5. Keep source paraphrases in planning files and cite exact pages in chapter drafts.

Use this order for commentary evidence:

- `planning/source-access-log.md` records whether we have legitimate access to the source.
- `planning/page-reference-ledger.md` records the page-level finding.
- `planning/commentary-evidence-starter.md` records the interpretive pattern across sources.
- Chapter drafts cite the source only after the ledger entry is strong enough for manuscript use.

## Current Citation Keys

- `aune1997revelation1-5`
- `beale1999revelation`
- `bealeCampbell2015shorter`
- `charles1920revelation`
- `koester2014revelation`
- `mounce1997revelation`
- `osborne2002revelation`
- `osborne2016verseByVerse`
- `swete1911apocalypse`
- `nestleAland2012na28`
- `ubs2014gnt5`
- `tabbTgcRevelation`
- `netBibleRevelation1`

## Warning

The bibliography is not the same as evidence. A source may be listed in `main.bib` because we intend to consult it, but a manuscript claim should cite that source only after the relevant passage has been checked.
