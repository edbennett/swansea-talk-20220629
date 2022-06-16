# Examples/Case studies

-

## [CalLat Collaboration, 2104.05226](https://arxiv.org/abs/2104.05226)

* Performs measurements on configurations
  * Specifies software used
* Data and analysis workflow both on [GitHub](https://github.com/callat-qcd/project_fh_vs_3pt)
  * Not tagged; not obvious which commit generated paper
  * Pure Python
* README indicates how each plot in paper generated
* All 20 figures automatically generated
* Tables not obviously generated

-

## [Scott Lawrence, 2111.13007](https://arxiv.org/abs/2111.13007)

* Performs a conformal bootstrap analysis
  * Does not perform measurements on field configurations
* All 5 plots generated programmatically
* Code available on [GitLab](https://gitlab.com/s.lawrence/bootstrap)
  * Primarily reusable components
  * Majority Python
* Full set of plots can be generated from one `Makefile`

-

## [EB et al, 2202.05516](https://arxiv.org/abs/2202.05516)

* Gauge configurations not shared
  * Modified [HiRep](https://github.com/sa2c/HiRep); code, parameters shared
* Measurement outputs available on [Zenodo](https://doi.org/10.5281/zenodo.6472270)
* Almost all 20 plots and 6 tables generated programmatically
  * Remainder are schematic, not numerical
  * Table contents available in [Zenodo data release](https://doi.org/10.5281/zenodo.6472270)
* Code available on [GitHub](https://github.com/edbennett/sp2n-multirep-202203) and [Zenodo](https://doi.org/10.5281/zenodo.6472232)
  * Mix of Python and Mathematica
* Not perfect!
  * Code has no automated tests
  * Automated _a posteriori_
  * Some code and data duplication
