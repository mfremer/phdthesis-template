LaTeX template for a PhD thesis at Université de Lorraine (uses thesul package for frontpage).

# Structure
- preamble.sty: add packages here
- frontpage/: uses the thesul class to generate the frontpage of the thesis
- chapters/chx/: chapter #x folder, chx.tex is the main file, should be self-contained

Use ch1.tex as a template for chapter templates, chx.tex files should not contain any \usepackage{} and use documentclass subfiles.

# Compilation
## Frontpage
```
cd frontpage
latexmk -pdf frontpage
```

## Thesis
```
latexmk -pdf main
```

## Individual chapter
```
cd chapters/chx
latexmk -pdf chx
```
