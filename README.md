
# thesis_template


LaTeX layout used for my [doctoral thesis](https://doi.org/10.4233/uuid:517f8597-9c24-4d01-83ed-0f430353e905) at the Delft University of Technology.
The thesis layout is demonstrated for both the booklet and propositions.

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

## Thesis project (thesis.tex)

## Propositions (propositions.tex)
