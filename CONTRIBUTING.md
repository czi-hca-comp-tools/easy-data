Contributions should be made through pull requests. Each PR should consist of
a markdown file containing

1. a description of the dataset including a link to the appropriate publication or
reference.
2. direct links to download the count matrix (in the form of an easy-to-load file, like .csv or .tsv files, or `rds` file containing an sparse matrix for R and an [AnnData](https://github.com/theislab/anndata) `hdf5` file or
  a `mtx` file for python). The most generic file format is .csv/.tsv.
3. direct links to download the metadata (in a `csv` with rows indexed by cell names).
4. bonus: sample loading code for R and python.

An example is [datasets/tabula_muris.md](datasets/tabula_muris.md)

__How easy can you make it for someone to get started?__
