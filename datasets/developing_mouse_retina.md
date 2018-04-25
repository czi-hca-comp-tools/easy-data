# Single cell RNA-Seq atlas of the developing murine retina

10x single cell RNA-seq data from the developing mouse retina

<img src="https://github.com/gofflab/developing_mouse_retina_scRNASeq/blob/master/img/Age.gif" width="300"/>
<img src="https://github.com/gofflab/developing_mouse_retina_scRNASeq/blob/master/img/CellType.gif" width="400"/>

## Use agreement
Although these data are being made publicly available as part of the [CZI Computational Tools](meetings.czi.technology/human-cell-atlas/) working group, the producers consider these data as unpublished and expect that the data will be used in accord with standard scientific etiquette and practices concerning unpublished data. Researchers are encouraged to use these data exclusively for the development of novel methods to analyze scRNA-Seq related to cell-cell variation, trajectory analysis and cell type identification/characterization. Use of these data for other purposes requires the explicit consent of the creators prior to an embargo date of July 1st, 2018.

## Stats

### Sample/Batches
| Age        | Replicate Number           | Cells  |
| ------------- |:-------------:|:-----:|
E11 | 1 | 8301
E12 | 1 |1503
E14 | 2 |24206
E16 | 1 | 4763
E18 | 2 |20578
P0  | 1 | 8873
P2  | 2 |15582
P5  | 1 | 5366
P8  | 2 |10200
P14 | 1 | 7680

## Count Matrix
The count matrix is provided in .mtx format and can be downloaded here:
[10x_mouse_retina_development.mtx](https://www.dropbox.com/s/6d76z4grcnaxgcg/10x_mouse_retina_development.mtx?dl=0)

## Cellular Phenotype Data
[10x_mouse_retina_development_phenoData.csv](https://www.dropbox.com/s/q0m4co24soo50ma/10x_mouse_retina_development_phenoData.csv?dl=0)

|                       |barcode                |sample |age | Size_Factor| num_genes_expressed| Total_mRNAs|CellType       | raw_cluster| umap_cluster| umap_coord1| umap_coord2| umap_coord3|umap_CellType |used_for_pseudotime |
|:----------------------|:----------------------|:------|:---|-----------:|-------------------:|-----------:|:--------------|-----------:|------------:|-----------:|-----------:|-----------:|:-------------|:-------------------|
|E11.AAACCTGAGATGTAAC.1 |E11.AAACCTGAGATGTAAC-1 |E11    |E11 |    1.733370|                1549|        2794|RPCs           |          32|          130|    3.581455|   -4.245770|   -3.752502|Early RPCs    |FALSE               |
|E11.AAACCTGAGGCAATTA.1 |E11.AAACCTGAGGCAATTA-1 |E11    |E11 |    2.201144|                1848|        3548|RPCs           |           9|          103|    2.634151|   -5.016845|   -3.926956|Early RPCs    |FALSE               |
|E11.AAACCTGAGTAGCGGT.1 |E11.AAACCTGAGTAGCGGT-1 |E11    |E11 |    2.381057|                1935|        3838|RPCs           |          24|          130|    3.268848|   -3.967177|   -3.942664|Early RPCs    |FALSE               |
|E11.AAACCTGAGTGGAGTC.1 |E11.AAACCTGAGTGGAGTC-1 |E11    |E11 |    2.861238|                2139|        4612|RPCs           |           9|          115|    3.737625|   -4.926516|   -4.012058|Early RPCs    |TRUE                |
|E11.AAACCTGCAAGTTGTC.1 |E11.AAACCTGCAAGTTGTC-1 |E11    |E11 |    2.044805|                1723|        3296|Lens Epithelia |          74|           77|    3.857854|   -4.027292|   -2.717437|Early RPCs    |FALSE               |
|E11.AAACCTGCACCCATTC.1 |E11.AAACCTGCACCCATTC-1 |E11    |E11 |    2.280553|                1806|        3676|RPCs           |          32|          109|    3.386985|   -3.678844|   -2.939268|Early RPCs    |TRUE                |

## Feature Data 
[10x_mouse_retina_development_featureData.csv](https://www.dropbox.com/s/5nv0u34h8ej70qo/10x_mouse_retina_development_featureData.csv?dl=0)

|                   |id                 |gene_short_name | num_cells_expressed| mean_expr|    sd_exprs|         bcv| percent_detection|
|:------------------|:------------------|:---------------|-------------------:|---------:|-----------:|-----------:|-----------------:|
|ENSMUSG00000051951 |ENSMUSG00000051951 |Xkr4            |                 253| 0.0021191| 0.046522355|   481.95455|         0.2094302|
|ENSMUSG00000089699 |ENSMUSG00000089699 |Gm1992          |                   4| 0.0000331| 0.005754187| 30200.24999|         0.0033111|
|ENSMUSG00000102343 |ENSMUSG00000102343 |Gm37381         |                  58| 0.0004801| 0.021906392|  2081.84482|         0.0480117|
|ENSMUSG00000025900 |ENSMUSG00000025900 |Rp1             |               11816| 0.1694811| 0.635347014|    14.05333|         9.7811331|
|ENSMUSG00000109048 |ENSMUSG00000109048 |Rp1             |                   0| 0.0000000| 0.000000000|         NaN|         0.0000000|
|ENSMUSG00000025902 |ENSMUSG00000025902 |Sox17           |                 108| 0.0016225| 0.077612551|  2288.30757|         0.0894010|
