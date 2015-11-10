# Neutrino Oscillations in Neutron Star Mergers
Deaton et al. 2016

### Overview
We are studying neutrino flavor transformations in neutron star mergers. The aims
of this paper are 1) to educate ourselves and the merger modeling community about
the toolbox of neutrino oscillations possible in environments with dense matter
and large neutrino fluxes, and 2) to paint a qualitative picture for the
astrophysics community (mainly nucleosynthesis folks) of where and when different
types of oscillations may occur. If we fulfill our second aim, we will have a
good start on the next stage of this project: figuring out how neutrino
absorptions may effect the formation of heavy elements from merger outflows.

The principle statements of the paper are:

1. Here's a toy model for the relevant terms in the oscillations Hamiltonian.
2. Here's how well it fits more nuanced models (ray tracing on Foucart's disks,
   and wind profiles from Fernandez's disks).
3. The different types of mergers produce different oscillations: here are the
   categories.

### Build Instructions
Compile the paper with the usual pdflatex sequence:
```
pdflatex paper.tex
bibtex paper
pdflatex paper.tex
pdflatex paper.tex
```
The `bibtex` and subsequent `pdflatex` calls are redundant if no new references
have been added between compiles.

### Text Guidelines
These guidelines establish conventions to improve the text of the article.
"Prefer to..." below means break the rule if it makes sense to.

* Prefer to write things in words not letters throughout: e.g. avoid "NSBH" or
  "MNR".
* Prefer to use abbreviations like "Eqn." and "Fig." in the text.

### LaTeX Guidelines
These guidelines establish conventions to make it easier to read and write
the raw LaTeX in paper.tex.

* __Object labels__.
  Use four letters or fewer for the class (e.g. `sec`, `ssec`, `fig`, etc.),
  followed by a colon,
  followed by a shortish underscore separated name (e.g. `nu_energy_spectrum`).
  Example: `\label{fig:nu_energy_spectrum}`.
* __BibTeX keys__.
  The key format in references.bib is `<surname><year>-<unique>` where
  `<surname>` is the 1st four (or fewer) letters of the 1st author's surname,
  `<date>` is the four-digit year of publication, and
  `<unique>` is a unique specifier from the title journal or whatever.
  Example: `deat2013-leakage`.
