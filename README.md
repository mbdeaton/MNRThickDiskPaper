# Matter-Neutrino Resonance Around Thick Disks
Deaton et al. 2016

### Overview
We are studying the Matter-Neutrino Resonance (MNR) in neutron star merger
environments. In this paper, we're extending Malkus et al.'s (2012,2013,2014)
analytic thin disk model to account for geometric thickness. We want to know if
the two distinct MNR behaviors---symmetric and standard---still occur when we
move our model a few steps forward in realism.

__Questions__.
How does the MNR affect neutrino flavor evolution around a disk if ...

1. ... it's geometrically thick?
2. ... the emission and scattering neutrino-surfaces are distinct?
3. ... the neutrino-surfaces are energy-dependent?

__Audience__.
Neutrino oscillation modelers. People pursuing the question: "Is
neutrino-transformation likely to be relevant to nucleosynthesis in neutron star
mergers?" (These are people familiar with MNR so we can breeze over the
introduction.)

__Structure__.
The paper could flow like this:

* quick overview of MNR (particularly Malkus's conclusions) and the physical
  scenarios that could produce it
* present new, improved disks: a family of parameterized, hierarchical
  models
* defend the new models by comparing to hydro simulations (from Foucart and
  Fernandez)
* give formulation for calculating neutrino self-interaction potential via ray
  tracing (instead of analytically as in Malkus's work)
* present results from each model

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
