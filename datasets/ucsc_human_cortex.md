# Developing human cortex data

This dataset contains ~4200 cells from the developing human cortex sequenced with Fluidigm C1, with relatively high coverage reads.

Paper: [Nowakowski et al 2018)](http://science.sciencemag.org/content/358/6368/1318.long)

Contact point in HCA: Max Haeussler, Jim Kent (UCSC), data produced/analyzed by Tom Nowakowski, Aparna Bhaduri (UCSF)

Data includes

1. Count matrix of log'ed counts from HiSat2.

2. Metadata csv includes clustername, age, patient ID.

```{bash}
    wget http://cells.ucsc.edu/aparna/geneMatrix.tsv.gz
    wget http://cells.ucsc.edu/aparna/meta.tsv
```

The original FASTQ files are in [dbGAP](https://www.ncbi.nlm.nih.gov/projects/gap/cgi-bin/study.cgi?study_id=phs000989.v3.p1&phv=253214&phd=&pha=&pht=5022&phvf=&phdf=&phaf=&phtf=&dssp=1&consent=&temp=1)

Browser: http://cells.ucsc.edu
