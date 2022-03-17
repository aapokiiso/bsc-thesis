Bachelor's thesis
=====

The build instructions currently assume you are using a Debian-based Linux
distro.

Dependencies
-----

To install required Texlive packages, run

```shell
$ apt update
$ apt install \
    texlive \
    texlive-latex-extra \
    texlive-fonts-extra \
    texlive-bibtex-extra \
    texlive-extra-utils \
    texlive-lang-european \
    biber
```

To install optional packages, run

```shell
$ apt install \
    chktex \
    latexmk
```

Next, download required files from the [Aalto Thesis LaTeX Template](https://wiki.aalto.fi/display/Aaltothesis/Aalto+Thesis+LaTeX+Template).

The required files are
- [`aaltothesis.cls`](https://wiki.aalto.fi/download/attachments/69900685/aaltothesis.cls?version=1&modificationDate=1537563039300&api=v2)
- [`aaltologo.sty`](https://version.aalto.fi/gitlab/latex/aaltologo/-/raw/master/aaltologo.sty?inline=false)

Place the downloaded files into `~/texmf/tex/latex/local`.

Build
-----

To build the document as a PDF, run

```shell
$ pdflatex thesis.tex
```
