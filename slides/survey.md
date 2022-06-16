# Survey of _hep-lat_ in 2021

-

## Survey scope

* Every hep-lat arXiv submission from 2021
  * Including cross-lists
  * Skim-read plus keyword searches
* Series of questions: yes/no, categorisation, and free text
  * Answers based solely on text of paper
* Data and analysis code are available on [Zenodo](https://doi.org/10.5281/zenodo.6584001)

-

## What computations does an LFT paper do?

A very reductive view:

1. Generate field configurations
2. Measures observables on configurations
3. Analyses, plots, tabulates measured observables

Less focus on emerging techniques, e.g.

* tensor networks
* quantum simulation

-

## High level numbers

Out of 1,229 arXiv submissions in 2021:

![Bar charts breaking down arXiv submissions](plots/all_numerical.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

* Use of preprints is already decades ahead of many disciplines! <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

-

## Why cite software?

Citing software:
* Gives credit to those who built it
  * Avoids paper-centric metrics
  * Justifies funding maintenance
* More precisely specifies what was done
  * Implementations vary in subtle details
  * Referring to an algorithm is not sufficient

-

## Setting the scene: Acknowledging HPC

![Bar chart breaking down arXiv submissions by whether they acknowledge HPC resources. The majority of hep-lat submissions worldwide and the vast majority in the UK do. Most crosslists do not.](plots/acknowledges_compute_resources.svg)

-

## How many submissions specify _any_ software?

![Bar chart breaking down arXiv submissions by whether they acknowledge software. The majortity do not. A slight majority in the UK do.](plots/specifies_any_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1300px" -->

-

## How is software acknowledged?

![Bar chart breaking down submissions specifying software by the method of psecification. Citation to a paper is most common.](plots/how_specifies_any_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1400px" -->

-

## Where does software live?

![Bar chart breaking down the locations used for software in use. GitHub is the most popular, followed by Zenodo.](plots/all_software_locations.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1000px" -->

* Zenodo is a data repository, gives DOIs
* GitHub is a code collaboration/hosting service; does not

---

## Generating field configurations

* Usually using Monte Carlo methods to sample from some action
* Usually extremely expensive
  * Hard to test automated workflows end-to-end
  * Hard for others to reproduce (wait for Moore's law?)
  * Open sharing of configurations is good
    * Needs infrastructure (more later)
* Reproducibility efforts include:
  * Seedable RNG, RNG checkpoints
  * Include run parameters in output, configurations files
  * Include code version/commit ID within output
* Around 44% of publications do this

-

## Do authors specify how configurations are generated?

![Bar chart breaking down whether publications specify what software was used for generating configurations. Internationally the majority do not; in the UK a slight majority do.](plots/specifies_configuration_generation_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

The UK is significantly better than average here. <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

-

## What software is used to generate configurations?

![Bar chart showing the top ten software packages used for configuration generation. Out of 100 papers, 14 use openQCD, 9 CL2QCD, and 7 each MILC, HiRep, FGrid, Chroma, BQCD](plots/configuration_generation_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

* 11 indicate unreleased modifications <!-- .element: class="fragment fade-in" data-fragment-index="2" -->
* More only name toolkits (e.g. Grid, Chroma) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

---

## What about work that doesn't generate configurations?

![Bar chart breaking down whether publications use existing field configurations; around 39% do. The majority of worldwide papers don't, but a slight majority of UK papers do.](plots/uses_existing_configurations.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1200px" -->

-

## How are existing configurations acknowledged?

![Bar chart breaking down how existing ensembles are acknowledged or cited. The overwhelming majority are citations to papers.](plots/how_specify_ensembles.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1200px"""-->

-

## Lattice Data Grids

* International Lattice Data Grid
  * Defines protocols and standards
  * Local deployments in US, UK, Europe, Japan, Australia
* FAIR before FAIR
* Early-ish example of open science

-

## How many papers acknowledge an LDG?

![Bar chart breaking down whether papers acknowledge a lattice data grid. Less than 5% do; 0% within the UK.](plots/acknowledges_data_grid.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1200px" -->

-

## Which LDGs are acknowledged?

![Bar chart showing which lattice data grids are acknowledged. 14 of 14 use the JLDG; 10 also acknowledge ILDG.](plots/which_data_grids.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="700px"-->

* Japan has the most active(ly cited) LDG <!-- .element: class="fragment fade-in" data-fragment-index="2" -->
* Either the others aren't used, or aren't cited <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

-

## Ongoing work on ILDG

* Perceived issues with ILDG:
  * DOIs, citability
  * Grid certificates
  * Rigidity of metadata
* ILDG committees recently resumed activity
  * Significant German government funding
  * Dedicated staff to address these problems

-

## Performing measurements

![Bar chart breaking down whether publications specify what software was used for measurement. A significant majority internationally and a small majority in the UK do not](plots/specifies_measurement_software.svg) <!-- .element width="1200px" -->

-

## What measurement codes are in use?

![Bar chart showing the top ten measurement codes. Chroma has 45 uses, QUDA 22, MILC and Grid 16.](plots/measurement_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

* 27 indicate unreleased modifications <!-- .element: class="fragment fade-in" data-fragment-index="2" width="700px" -->
* More only name toolkits (e.g. Grid, Chroma) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

---

## Use of open data

(Excluding field configurations)

![Bar chart breaking down how publications acknowledge data they have used; the overwhelming majority are citations to papers](plots/how_acknowledges_other_data.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

* Acknowledgements to individuals <!-- .element: class="fragment fade-in" data-fragment-index="2" -->
* Not FAIR <!-- .element: class="fragment fade-in" data-fragment-index="2" -->

-

## Do authors publish data?

![Bar chart breaking down how whether publications publish data. The overwhelming majority do not.](plots/publish_any_data.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1300px" -->

-

## Where are data published?

![Bar chart showing where data are published. Out of 38 submissions, 12 publish data directly on the arXiv, 5 on GitLab, 3 each on Unibi and Zenodo.](plots/used_data_repositories.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="800px" -->

---

## Data analysis

* Experimental research:
  * Does not generate configurations
  * Does not perform computationally reproducible "measurements"
  * Still has a substantial reproducibility effort
  * $\Rightarrow$ Data analysis of measurement results is the key reproducibility question

-

## Do authors specify _any_ software is used for analysis?

![Bar graph breaking down whether software used for data analysis is specified. The vast majority of publications do not specify any software.](plots/specifies_analysis_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1300px" -->

-

## What software is specified?

![Bar graph showing the top 10 software packages acknowledged by hep-lat publications and crosslists. The top 5 in hep-lat are Mathematica, gvar, numpy, matplotlib, and lsqfit.](plots/acknowledged_analysis_software.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1300px" -->

-

## Do authors publish a full analysis workflow?

![Bar graph breaking down whether authors publish a full or partial analysis workflow. The overwhelming majority do not; only single digit numbers out of a thousand publish in full.](plots/publish_analysis_workflow.svg) <!-- .element: class="fragment fade-in" data-fragment-index="2" width="1300px" -->
