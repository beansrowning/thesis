# Thesis Paper

## Depends :
  - XeLaTeX
  - bibTeX
  - TiKZ
  - pgfplots
  - subfiles
  - ragged2e

#### A standard LaTeX build of [TeX Live](http://www.tug.org/texlive) or [MiKTeX](http://www.miktex.org) should be sufficient.

## Build instructions :
  - Building the PDF requires three passes of XeLaTeX (pdftex should work, also), and one of Bibtex.
  - TiKZ images and pgfplots will render as seprate TeX jobs to avoid memory issues.
  - Create a `/figures` directory if not already present.
  - Synctex is optional

```shell
  xelatex -shell-escape -synctex=1 Paper
  bibtex Paper
  xelatex -shell-escape -synctex=1 Paper
  xelatex -shell-escape -synctex=1 Paper
```
