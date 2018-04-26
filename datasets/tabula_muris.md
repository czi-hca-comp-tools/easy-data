# Tabula Muris

[Tabula Muris](http://tabula-muris.ds.czbiohub.org/) contains about 100,000 cells from 20 organs and tissues in mouse. The study is sex-balanced, with four male and four female mice. The organs included are skin, fat, mammary gland, heart, bladder, brain, thymus, spleen, kidney, limb muscle, tongue, marrow, trachea, pancreas, lung, large intestine, and liver. Many of these organs were processed using two methods: SMART-seq2 on FACS-sorted cells and microfluidic droplets from 10X Genomics.

Below are instructions for getting four files: metadata (including annotations) and count data for each dataset.

## Metadata

Version-controlled metadata are available on  [github](https://github.com/czbiohub/tabula-muris-vignettes/tree/master/data).

[TM_droplet_metadata.csv](https://github.com/czbiohub/tabula-muris-vignettes/blob/master/data/TM_droplet_metadata.csv?raw=true)

[TM_facs_metadata.csv](https://github.com/czbiohub/tabula-muris-vignettes/blob/master/data/TM_facs_metadata.csv?raw=true)

## Count files for R

You can download complete count files as sparse matrices in `.rds` format for easy loading into `R`. Unzip [TabulaMuris.zip](https://s3.amazonaws.com/czbiohub-tabula-muris/TabulaMuris.zip). Load:

```R
library(tidyverse)

tm.droplet.matrix = readRDS("TM_droplet_mat.rds")
tm.droplet.metadata = read_csv("TM_droplet_metadata.csv")
```

## Count files for Python

You can download complete count files as sparse matrices in [AnnData](http://anndata.readthedocs.io/en/latest/)-formatted h5ad files for use in Python [here](https://s3.amazonaws.com/czbiohub-tabula-muris/TabulaMuris.h5ad.zip). You can load them using the [Scanpy](http://scanpy.readthedocs.io/en/latest/index.html) library:

```python
import pandas
import scanpy

tm_facs_metadata = pd.read_csv('data/TM_facs_metadata.csv')
tm_facs_data = scanpy.anndata.read_h5ad('data/TM_facs_mat.h5ad').transpose()
```
## CSV and MTX files

The original data release is on [FigShare](https://figshare.com/projects/Tabula_Muris_Transcriptomic_characterization_of_20_organs_and_tissues_from_Mus_musculus_at_single_cell_resolution/27733).
