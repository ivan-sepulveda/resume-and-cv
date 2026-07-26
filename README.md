# resume-and-cv

LaTeX source for Iván Sepúlveda's resume and CV.

## Structure

- `one-page-resume/` — one-page resume (`document.tex`)
- `curriculum-vitae/` — full CV, includes a publications list via `publications.tex` and `own-bib.bib` (biblatex/biber)

Each folder builds independently and produces its own `document.pdf`.

## Build

Requires a LaTeX distribution with `biber` (e.g. TeX Live).

```bash
cd one-page-resume   # or curriculum-vitae
pdflatex document.tex
biber document
pdflatex document.tex
pdflatex document.tex
```

## TODO

- [ ] Optimize both CV and resume for Applicant Tracking Systems (ATS): use standard section headers, avoid multi-column/graphics-heavy layouts that don't parse well, ensure text extracts cleanly from PDF, and align keywords with target job descriptions.
