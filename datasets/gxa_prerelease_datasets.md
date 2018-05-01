# Pre-release datasets from the EBI Single-Cell Expression Atlas

The following are 6 Smart-seq2 datasets analysed as part of the Single-Cell Expression Atlas project due for its first release later in the year. They form an example of processed matrices suitable for downstream analysis.

## Data

In the following data the columns are:

* ENA: link to the European nucleotide archive record for the experiment
* Experiment metadata: file in [IDF format](https://www.ebi.ac.uk/arrayexpress/help/creating_an_idf.html)
* Cell metadata: comma-separated file with cell-wise metadata
* Filtered quantification files: expression matrices containing TPMs, in .mtx format, with matrices, column info and row info in separate files
* Clusters: SC3-derived clusters 

| Experiment | ENA | Experiment metadata | Cell metadata | Filtered quantification files | Clusters |
| --- | --- | --- | --- | --- | --- |
| Single-cell RNA-seq analysis of 1,522 cells of the small intestinal epithelium | [SRP095033](https://www.ebi.ac.uk/ena/data/view/PRJNA357261) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-13/E-ENAD-13.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-13/ExpDesign-E-ENAD-13.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-13/E-ENAD-13-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-13/E-ENAD-13.clusters.tsv) |
| Single-cell RNA-seq analysis of 389 cells of the small intestinal epithelium in response to Salmonella enterica and to the parasitic helminth Heligmosomoides polygyrus | [SRP095033](https://www.ebi.ac.uk/ena/data/view/PRJNA357261) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-14/E-ENAD-14.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-14/ExpDesign-E-ENAD-14.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-14/E-ENAD-14-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-ENAD-14/E-ENAD-14.clusters.tsv) |
| Single-cell transcriptome analysis of precursors of human CD4+ cytotoxic T lymphocytes | [SRP124157](https://www.ebi.ac.uk/ena/data/view/PRJNA417191) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-106540/E-GEOD-106540.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-106540/ExpDesign-E-GEOD-106540.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-106540/E-GEOD-106540-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-106540/E-GEOD-106540.clusters.tsv) |
| Single cell RNA-sequencing of human tonsil Innate lymphoid cells (ILCs) | [SRP060416](https://www.ebi.ac.uk/ena/data/view/PRJNA289086) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-70580/E-GEOD-70580.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-70580/ExpDesign-E-GEOD-70580.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-70580/E-GEOD-70580-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-70580/E-GEOD-70580.clusters.tsv) |
| Single cell transcriptome analysis of human pancreas | [SRP075496](https://www.ebi.ac.uk/ena/data/view/PRJNA322355) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-81547/E-GEOD-81547.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-81547/ExpDesign-E-GEOD-81547.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-81547/E-GEOD-81547-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-81547/E-GEOD-81547.clusters.tsv) |
| Single-Cell RNAseq analysis of diffuse neoplastic infiltrating cells at the migrating front of human glioblastoma | [SRP079058](https://www.ebi.ac.uk/ena/data/view/PRJNA330719) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-84465/E-GEOD-84465.idf.txt) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-84465/ExpDesign-E-GEOD-84465.csv) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-84465/E-GEOD-84465-quantification-filtered-files.zip) | [link](http://ftp.ebi.ac.uk/pub/databases/arrayexpress/data/atlas/example_single_cell/E-GEOD-84465/E-GEOD-84465.clusters.tsv) |


## Analysis methods

The following tools were used in the processing of these data. 

| Analysis | Software | Version | Citation |
| --- | --- | --- | --- |
| QC | FASTQC | 0.11.7 | http://www.bioinformatics.babraham.ac.uk/projects/fastqc/ |
| Filtering and trimming | FASTX | 0.0.13 | http://hannonlab.cshl.edu/fastx_toolkit/ |
| Pipeline | IRAP | 1.0.0b | Nuno A. Fonseca, Robert Petryszak, John Marioni, Alvis Brazma. iRAP - an integrated RNA-seq Analysis Pipeline. bioRxiv 2014. doi: http://dx.doi.org/10.1101/005991 |
| Clustering/Gene markers | SC3 | 1.7.7 | Kiselev, Vladimir Yu, Kristina Kirschner, Michael T. Schaub, Tallulah Andrews, Andrew Yiu, Tamir Chandra, Kedar N. Natarajan et al. SC3: consensus clustering of single-cell RNA-seq data. Nature methods 14, no. 5 (2017): 483. |
| Reads alignment | bowtie2 | 2.3.2 | Langmead, Ben, and Steven L. Salzberg. Fast gapped-read alignment with Bowtie 2. Nature methods 9, no. 4 (2012): 357-359. |
| QC | fastq_utils | 0.14.7 | https://github.com/nunofonseca/fastq_utils |
| Gene/transcript quantification | kallisto | 0.44.0 | Nicolas L Bray, Harold Pimentel, Páll Melsted, Lior Pachter. Near-optimal probabilistic RNA-seq quantification. Nature Biotechnology (2016). |
