# paper-notes

Visual, skimmable highlights of research papers. Each paper gets one page with a TL;DR, diagrams, key findings, and critique. The goal is to get the important points of a paper in minutes without reading the full text.

## Papers

| Date read | Paper | Topic | TL;DR |
|---|---|---|---|
<!-- New rows go at the top. Format: | YYYY-MM-DD | [Title](papers/<dir>/) | tags | one line | -->

## How each note is structured

Every note follows [`TEMPLATE.md`](TEMPLATE.md) and is layered, so you can stop reading at any layer:

1. **TL;DR**: 4 bullets, about 30 seconds.
2. **The one diagram**: the core idea in a single Mermaid figure.
3. **Key findings**: a table that cites the paper's evidence.
4. **How it works**: architecture and method diagrams.
5. **Numbers worth remembering**.
6. **Critique, takeaways, open questions, glossary, related work.**

Diagrams are written in [Mermaid](https://mermaid.js.org/), which GitHub renders inline. Nothing needs to be built.

## Layout

```
papers/
  <arxiv-id>-<short-slug>/
    README.md        # the note
    *.md             # optional deep-dive pages for long papers
TEMPLATE.md
```

PDFs are not stored here. Each note links to the source instead.

## Workflow

One paper per PR:

1. `git checkout -b feature/paper-<arxiv-id>-<slug>`
2. `cp TEMPLATE.md papers/<arxiv-id>-<slug>/README.md` and fill it in.
3. Add a row to the **Papers** table above.
4. Open a PR, review the rendered diagrams on GitHub, then merge.
