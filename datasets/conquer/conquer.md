## `conquer`
 
Mark Robinson and Charlotte Soneson have created the great [`conquer`](http://imlspenticton.uzh.ch:3838/conquer/) dataset, which contains `MultiAssayExperiments` R objects for about 38 single cell experiments with count level and consistently normalized data plus QC reports. Here is a [gist](https://gist.github.com/ivirshup/131a56175503a2408f814874925c19f9) which contains a python script (and conda requirements file) to pull down all those datasets.
 
This data was aggregated for use in: [Bias, robustness and scalability in single-cell differential expression analysis](https://www.nature.com/articles/nmeth.4612).
 
Once you've downloaded the datasets, you can easily load them into R:

```r
library(MultiAssayExperiment)
library(SummarizedExperiment)
data <- loadRDS("{dataset}.rds")
```

For a more extensive example, see the tutorial section on the [`conquer`](http://imlspenticton.uzh.ch:3838/conquer/) site.
