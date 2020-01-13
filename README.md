
# thesis_template


LaTeX layout used for my [doctoral thesis](https://doi.org/10.4233/uuid:517f8597-9c24-4d01-83ed-0f430353e905) at the Delft University of Technology.

The thesis layout is demonstrated for both the book and the propositions.

## thesis.sty

LaTeX2e book style for the PhD thesis layout

### Usage

`\usepackage[screen]{thesis}`

### Options

Shortcuts:
 
	screen            enables options : booklet
	print             enables options : booklet scaled, cmyk, bindingoffset


All options:

	booklet           papersize 17x24cm
	bookletscaled     papersize 17x24cm on a regular a4paper with crop marks
	bindingoffset     set 6.5mm binding offset
	cmyk              force (tikz) cmyk colours
	newfonts          use new modern fonts garamondx and newtxmath
	norulers          remove header rulers
	italic            put header chapter and section in italic
	thumbs            enable chapter thumbs
	debug             enable geometry showframe and showcrop

## Doctoral thesis (thesis.tex)

Core LaTeX file the includes all chapters. Each chapter has its own folder named `ch-...` containing the text `main.tex` and a folder `figs` containing all figures. Long chapters can be split similarly for sections. 

## Propositions (propositions.tex)

The layout of the doctoral thesis (thesis.sty) is used for the propositions. An example is given in both English and Dutch, with a reference to a specific chapter of the doctoral thesis.


## LaTex and TexLive

For MacTex users, don't install the full package but download the smaller [BasicTeX]: https://tug.org/mactex/morepackages.html

Once TexLive is installed you can add all missing packages using the TexLive Manager `tlmg`.

### Install LaTeX packages using tlmg

Set default ctan repository location.
```
sudo tlmgr option location http://mirror.ctan.org/systems/texlive/tlnet
```

Install latexmk (essential for sublime users).
```
sudo tlmgr install latexmk
```

### Install all missing packages automatically

Install on the fly package installation tool.
```
sudo tlmgr install texliveonfly
```

Run once texliveonfly to install all missing packages.
```
sudo texliveonfly thesis.tex
```
