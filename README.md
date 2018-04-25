# easy-data

Easy access to a small collection of benchmark datasets for methods development, focused on supporting projects at the hca-comp-tools workshop. Add your benchmarking desiderata and your datasets below.

## benchmark for what?

A discussion of the problems for which benchmark datasets would allow for experimentation.

* cell type annotation and reannotation at various levels of ontological depth
* building and validating cell type classifiers
* manifold alignment and batch-effect-aware analyses
* assessing the variability in gene expression of cell types present in many organs
* measuring sex differences in gene expression
* measuring the variability in biological claims (like which genes are differentially expressed between populations) to be expected between different studies of the same cell types

## There are several sources of public datasets.  The question is, what should be the characteristics of a benchmark dataset?
At the most basic level, it should be very easy to access (e.g. free/open, in data formats that people use, easy to access).  Then there are different requirements depending on what is being benchmarked, such as:
* clustering would want to see a mix of easy and difficult to cluster data.
* portals would want a mix of small and large data sets to test development (quick test with small data) and scalability (test with large data)
* for manifold alignment, datasets that have batch effect artifacts
* trajectories would want data that actually contains trajectories e.g. developmental biology data, including time series data
* control perturbations from well known experimental conditions are also helpful for benchmarking

# datasets

To add a dataset, just create a section with a description and links to download it.

How easy can you make it for someone to get started?

## `tabula muris`

[Tabula Muris](http://tabula-muris.ds.czbiohub.org/) contains about 100,000 cells from 20 organs and tissues in mouse. The study is sex-balanced, with four male and four female mice. The organs included are skin, fat, mammary gland, heart, bladder, brain, thymus, spleen, kidney, limb muscle, tongue, marrow, trachea, pancreas, lung, large intestine, and liver. Many of these organs were processed using two methods: SMART-seq2 on FACS-sorted cells and microfluidic droplets from 10X Genomics.

Below are instructions for getting four files: metadata (including annotations) and count data for each dataset.

### metadata

Version-controlled metadata are available on  [github](https://github.com/czbiohub/tabula-muris-vignettes/tree/master/data).

[TM_droplet_metadata.csv](https://github.com/czbiohub/tabula-muris-vignettes/blob/master/data/TM_droplet_metadata.csv?raw=true)

[TM_facs_metadata.csv](https://github.com/czbiohub/tabula-muris-vignettes/blob/master/data/TM_facs_metadata.csv?raw=true)

### count files for R

You can download complete count files as sparse matrices in `.rds` format for easy loading into `R`. Unzip [TabulaMuris.zip](https://s3.amazonaws.com/czbiohub-tabula-muris/TabulaMuris.zip). Load:

```R
tm.droplet.matrix = readRDS(here("data", "TM_droplet_mat.rds"))
tm.droplet.metadata = read_csv(here("data", "TM_droplet_metadata.csv"))
```

### count files for Python

You can download complete count files as sparse matrices in [AnnData](http://anndata.readthedocs.io/en/latest/)-formatted h5ad files for use in Python [here](https://s3.amazonaws.com/czbiohub-tabula-muris/TabulaMuris.h5ad.zip). You can load them using the [Scanpy](http://scanpy.readthedocs.io/en/latest/index.html) library:

```python
import pandas
import scanpy

tm_facs_metadata = pd.read_csv('data/TM_facs_metadata.csv')
tm_facs_data = scanpy.anndata.read_h5ad('data/TM_facs_mat.h5ad')
```
### CSV and MTX files

The original data release is on [FigShare](https://figshare.com/projects/Tabula_Muris_Transcriptomic_characterization_of_20_organs_and_tissues_from_Mus_musculus_at_single_cell_resolution/27733).


## Software Packages

- [CellBench](https://github.com/LuyiTian/CellBench_data)
