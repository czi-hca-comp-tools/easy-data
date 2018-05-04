# MCA (mouse cell atlas)

[MCA](http://tabula-muris.ds.czbiohub.org/) contains about 300,000 cells from major mouse organs sequenced using the microwell-seq platform.

The study is published [here](https://www.cell.com/cell/abstract/S0092-8674(18)30116-8).

Below are instructions for getting four files: metadata (including annotations) and count data for each dataset.

## Metadata

You can download the metadata file from here (thanks to Guo's lab):
[MCA-cell-ann.csv](https://github.com/czi-hca-comp-tools/easy-data/blob/MCA/datasets/mouse-cell-atlas/MCA-cell-ann.csv)

## Count files for R

As a courtesy of [Satija lab](http://satijalab.org/seurat/mca.html) you can download complete count files as a sparse matrice in `.rds` format for easy loading into `R`. 

Unzip [MCA.zip](https://www.dropbox.com/s/8d8t4od38oojs6i/MCA.zip?dl=1) and copy the `MCA-cell-ann.csv` into the folder. Either move the entire folder to your working directory in R or make sure to point R to right place and then run:

```R
library(Matrix)
library(Seurat)

microwell.matrix = readRDS(here("MCA", "MCA_merged_mat.rds"))
microwell.metadata = read_csv(here("MCA", "cell-ann.csv"))

microwell.matrix <- microwell.matrix[,colnames(microwell.matrix) %in% microwell.metadata$Cell.name]
microwell.metadata <- microwell.metadata[microwell.metadata$Cell.name %in% colnames(microwell.matrix),]
```
