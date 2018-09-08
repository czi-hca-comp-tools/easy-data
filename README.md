# easy-data

Easy access to a small collection of benchmark datasets for methods development.


<p align="center">
	<a href="benchmarks.md">Why do we need data benchmarks?</a>&nbsp;&nbsp;&nbsp;
	<a href="CONTRIBUTING.md">Contribution guide</a>&nbsp;&nbsp;&nbsp;
</p>

## Contents

- [Imaging](#imaging)
- [Multiomics](#multiomics)
- [RNA-Seq](#rna-seq)


## Datasets

Instructions for downloading and loading each dataset are in text files in the `datasets` folder.

### RNA-Seq

- [Loyale Developing mouse retina](datasets/developing_mouse_retina.md) - 10x single cell RNA-seq data from the developing mouse retina. [Code repo](https://github.com/gofflab/developing_mouse_retina_scRNASeq) | [Download instructions](datasets/developing_mouse_retina.md) #retina #mouse #umi #10x #droplet
- [Tabula Muris](datasets/tabula_muris.md) - 20 different mouse organs, both full transcript (SmartSeq2) and UMI-based droplet counting (10x Genomics). [Code repo](https://github.com/czbiohub/tabula-muris) | [Vignette repo](https://github.com/czbiohub/tabula-muris-vignettes) | [Interactive website](http://tabula-muris.ds.czbiohub.org/) | [Download instructions](datasets/tabula_muris.md) #mouse #aorta #bladder #brain #diaphragm #fat #heart #kidney #large_intestine #muscle #liver #lung #mammary_gland #marrow #pancreas #skin #spleen #thymus #tongue #rnaseq #smartseq2 #10x #umi #droplet
- [Human cortex development](datasets/ucsc_human_cortex.md) - 4000 SmartSeq2 cells from different locations of the developing human fetus.
- [Conquer](datasets/conquer.md) - [38 datasets](http://imlspenticton.uzh.ch:3838/conquer/) summarized to a count level available as `R` `MultiAssayExperiment` objects.
- [CellBench pilot data set](https://github.com/LuyiTian/CellBench_data/blob/master/cellbench.md) - mixture data set from 3 human lung adenocarcinoma cell lines (HCC827, H1975 and H2228) across different platforms. #benchmark #celseq2 #dropseq #10x #cellline
- [HCA preview dataset gene counting matrix](datasets/HCA_preview_scPipe.md) - HCA preview data gene counting matrix. The gene counting matrix was generated from fastq by [scPipe](https://bioconductor.org/packages/release/bioc/html/scPipe.html). #hca #scPipe

### Imaging


- [Example dataset](datasets/example.md) - 1-2 sentence summary of dataset. [Code Repo](https://github.com/) | [Vignette Repo](https://github.com/) | [Interactive Website](https://github.com/) | [Download instructions](datasets/example.md) #mouse


### Multiomics

- [Example dataset](datasets/example.md) - 1-2 sentence summary of dataset. [Code Repo](https://github.com/) | [Vignette Repo](https://github.com/) | [Interactive Website](https://github.com/) | [Download instructions](datasets/example.md) #mouse
