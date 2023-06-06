LaTeX source files for my PhD thesis.

# Basic info
Title (french): Problèmes d'agencement pour le design génératif et la modélisation d'objets
Title (english): Layout problems and generative design for shape modeling
Author: Marco Freire
Supervisor: Sylvain Lefebvre
Laboratory: Université de Lorraine

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
