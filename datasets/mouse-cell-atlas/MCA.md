# MCA (mouse cell atlas)

[MCA](http://tabula-muris.ds.czbiohub.org/) contains about 300,000 cells from major mouse organs sequenced using the microwell-seq platform.

The study is published [here](https://www.cell.com/cell/abstract/S0092-8674(18)30116-8).

Below are instructions for getting four files: metadata (including annotations) and count data for each dataset.

## Metadata

You can download the metadata file from here (thanks to Guo's lab):
[MCA-cell-ann.csv](https://github.com/czi-hca-comp-tools/easy-data/blob/MCA/datasets/mouse-cell-atlas/MCA-cell-ann.csv)

## Count files for R

As a courtesy of [Satija lab](http://satijalab.org/seurat/mca.html) you can download complete count files as a sparse matrice in `.rds` format for easy loading into `R`. Unzip [MCA.zip](https://www.dropbox.com/s/8d8t4od38oojs6i/MCA.zip?dl=1) and load:

```R
library(Matrix)
library(Seurat)

mca.matrix <- readRDS(file = "~/Downloads/MCA/MCA_merged_mat.rds")
mca.metadata <- read.csv("~/Downloads/MCA/MCA_All-batch-removed-assignments.csv", row.names = 1)
```
