LaTeX template for a PhD thesis.

# Folder structure
- frontpage/: uses the thesul class to generate the frontpage of the thesis
- chapters/chx/: chapter no.x folder, chx.tex is the main file, should be self-contained

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
