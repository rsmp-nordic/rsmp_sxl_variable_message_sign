# RSMP Signal Exchange List (SXL) for Variable Message Signs
This repository contains the official RSMP SXL for variable message signs
and is also used to coordinate the development of the SXL.
The repository is maintained by [RSMP Nordic](https://rsmp-nordic.org)

## SXL

There is no official release yet, but work is underway. You are welcome
to contribute.

## Generating the specification from source

Requirements:

- Sphinx: https://www.sphinx-doc.org
- LaTeX (and pdflatex, and various LaTeX packages)

On Ubuntu:

```
# apt-get install python-sphinx texlive texlive-latex-extra \
  texlive-humanities latexmk sphinx python-sphinx-rtd-theme
```

On Arch:

```
# pacman -S python-sphinx texlive-most texlive-latexextra texlive-humanities \
  python-sphinx_rtd_theme
```

Then:

```
$ make latexpdf # For generating pdf
$ make html # For generating a hierarchy of html pages
$ make singlehtml # For generating a single html page
```

