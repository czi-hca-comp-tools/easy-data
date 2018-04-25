
# benchmark for what?

A discussion of the problems for which benchmark datasets would allow for experimentation.

* cell type annotation and reannotation at various levels of ontological depth
* building and validating cell type classifiers
* manifold alignment and batch-effect-aware analyses
* assessing the variability in gene expression of cell types present in many organs
* measuring sex differences in gene expression
* measuring the variability in biological claims (like which genes are differentially expressed between populations) to be expected between different studies of the same cell types

There are several sources of public datasets.  The question is, what should be the characteristics of a benchmark dataset?
At the most basic level, it should be very easy to access (e.g. free/open, in data formats that people use, easy to access).  Then there are different requirements depending on what is being benchmarked, such as:
* clustering would want to see a mix of easy and difficult to cluster data.
* portals would want a mix of small and large data sets to test development (quick test with small data) and scalability (test with large data)
* for manifold alignment, datasets that have batch effect artifacts
* trajectories would want data that actually contains trajectories e.g. developmental biology data, including time series data
* control perturbations from well known experimental conditions are also helpful for benchmarking

## Benchmarking resources

## Software Packages

- [CellBench](https://github.com/LuyiTian/CellBench_data)
- [IA-SVA](https://github.com/UcarLab/IA-SVA)
