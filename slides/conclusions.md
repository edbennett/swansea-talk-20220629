# Conclusions and next steps

-

## Conclusions

* LFT has been at the forefront of many aspects of open science
  * Some areas suffer from first-mover disadvantage
* Opportunities remain to do more
  * Some low-hanging fruit
    * Specify software
    * Share existing code
  * Some require more effort
    * e.g. Automating analyses and presentation of data

-

## Thoughts for everyone: data

* If you produce data, publish it!
  * Get a persistent ID
  * _Cite_ the data in the paper
  * Journals can host small amounts of data
* Share data at various stages
  * Keep raw data raw
  * Make data easy to read
  * Include final results too
* If you're not sure where to start, talk to me

-

## Thoughts for lattice: data

* Compromise between data volume and compute capability
* Input files: in principle reproducible; requires huge compute
* Configurations:
  * Saves huge amount of HPC time; still requires some HPC
  * Can be used for other purposes
  * Requires huge storage
  * Persistent IDs an unsolved problem
* Measurement outputs (logs, correlators, flow histories, etc.):
  * Can usually be analysed on a workstation
  * Usually requires less storage than configurations
  * Reduced flexibility

-

## Thoughts for everyone: code

* If you're doing things manually, can you automate them?
  * Remembering Croucher's law
  * Every manual step removed reduces an opportunity for human error
* If you're automating things, can you publish the workflow?
  * Even if it's 5 lines of Mathematica!
    * The less there is, the easier it is to publish
  * Get a persistent ID
  * _Cite_ the workflow in the paper
  * It's _fine_ if your code is ugly
* If you're not sure where to start, talk to me

-

## Thoughts for lattice: code

* Workflow management (currently) needs work:
  * Data flow between disparate tools
  * Managing dependencies
  * Order of execution
  * Parallelisation
  * Working on developing tools/recommendations for this

-

## Next steps

* Produce a manifesto of good practice in open science in lattice
* Develop tooling to better enable automated analysis and presentation
  * Aspiration: "easier to use than not to"
* [Survey of reproducible and open science practices](lattice-survey)
  * [bit.ly/lattice-survey-2022](lattice-survey)
  * Initial results to be presented at Lattice 2022


[lattice-survey]: https://bit.ly/lattice-survey-2022
