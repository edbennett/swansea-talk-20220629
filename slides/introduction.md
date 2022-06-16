# Definitions

-

## Reproducibility

Same data 
<span class="fragment fade-in" data-fragment-index="1">$+$ same analysis</span>
<span class="fragment fade-in" data-fragment-index="2">$\rightarrow$ Same results</span>

* Related concepts: <!-- .element: class="fragment fade-in" data-fragment-index="3" -->
  * Replicability: New data $+$ same analysis $\rightarrow$ same results <!-- .element: class="fragment fade-in" data-fragment-index="4" -->
  * Robustness: Same data $+$ new analysis $\rightarrow$ same results <!-- .element: class="fragment fade-in" data-fragment-index="5" -->

-

## Open science

The movement to make all research accessible to all levels of society.

Including, but not limited to:

* Publications
* Physical samples
* Data
* Software

-

## FAIR

Research data (and software) should be:

* **F**indable
* **A**ccessible
* **I**nteroperable
* **R**eusable

_Orthogonal to data being open_

-

## Persistent identifier

A reference for a digital object that will not change.

E.g. a Digital Object Identifier (DOI)

CERN runs [Zenodo](https://www.zenodo.org), which gives DOIs to data

---

# Motivation

-

## Why open science?

* The ideal scientific process
* Public funding $\Rightarrow$ Public results <!-- .element: class="fragment fade-in" data-fragment-index="2" -->
* Our funders say so <!-- .element: class="fragment fade-in" data-fragment-index="3" -->

_"Data resulting from publicly funded research should be made publicly available... unless there are specific reasons (e.g. legislation, ethical, privacy and security) why this should not happen"_ &mdash;[STFC Scientific Data Policy](https://www.dcc.ac.uk/guidance/policy/funders-data-policies/stfc)
<!-- .element: class="fragment fade-in" data-fragment-index="3" -->

-

## Open science accelerates progress

[The war over supercooled water (DOI:10.1063/PT.6.1.20180822a)](https://physicstoday.scitation.org/do/10.1063/pt.6.1.20180822a/full/)

* Discrepancy discovered in 2011
* Student hired to revisit computations in 2012
* Code requested in 2013
* Code promised "available on request" in 2016
* Code eventually provided after involvement of Nature editors
* Discrepancy caused by a poor choice of initialisation function
* Findings published in 2017

Was that the best use of 6 years of arguments?

-

## Articles as advertisements

_An article about computational science in a scientific publication is
**not** the scholarship itself, it is merely **advertising** of the
scholarship. The actual scholarship is the complete software development
environment and the complete set of instructions which generated the
figures._

&mdash;[attributed to Jon Claerbout, around 1995](https://statweb.stanford.edu/~wavelab/Wavelab_850/wavelab.pdf)

-

## Why automated reproducibility?

* Communication with words is imprecise
* Papers have limited space
* Human error is inevitable
  * [Croucher's law](https://mikecroucher.github.io/MLPM_talk/):
    I am an idiot and will make mistakes
* Computers are pretty good at doing the same thing every time

-

## Why persistent identifiers?

* Universities restructure their websites
* Software hosting services come and go
* People change usernames
* People move institutions

[![Image of a tweet reading "Another reminder: reviewers and editors need to insist that software be placed in a permanent repository. Not author's web site. Not GitHub.", quoting a second reading "Anyone know where to find the xenograft read detecting software Xenome? Link on the paper is dead."](images/code_archive_tweet.png) <!-- .element:  width="600px" -->](https://twitter.com/michaelhoffman/status/796103749068529667)
