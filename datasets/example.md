# Example dataset

Long-form description of the data, the organs and species collected, any perturbations of the data. May link to the appropriate publication or reference

This dataset contains 100,000 cells from the mouse *organ*.

## How to download the metadata

[Here](example.com) is a direct link to the metadata as a `csv`, where rows are indexed by cell names.

## How to download the counts data

You can download complete count files as sparse matrices in `.rds` format for easy loading into `R`. Download [this](example.com) file and unzip.

## Example code

Here are some code snippets for loading the data

### Python

Here is a code snippet for loading the data in Python:

```python
import pandas as pd
from anndata import read_h5ad

metadata = pd.read_csv('data/metadata.csv')
data = read_h5ad('data/matrix.h5ad').T
```

### R

```R
library(tidyverse)

matrix = readRDS("TM_droplet_mat.rds")
metadata = read_csv("TM_droplet_metadata.csv")
```
