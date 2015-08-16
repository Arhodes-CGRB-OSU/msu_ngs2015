# DE analysis module for Week3


For RNA-seq data, the strategy taken is to count the number of reads that fall into annotated genes and to perform statistical analysis on the table of counts to discover quantitative changes in expression levels between experimental groups. Easy, right? Not, exactly.

1. We have integer counts and not continous measurements. Data is not normally distributed, so statistical methods we applied to microarray data don't work here. 

2. Replication levels in designed RNA-Seq experiments tend to be modest, often not much more than two or three. As a result, there is a need for statistical methods that perform well in small-sample situations. The low levels of replication rule out, for all practical purposes, distribution-free rank or permutation-based methods.  

3. The Poisson model doesn't work either -- it is a single parameter model with mean == variance and real data has more variance than Poisson can explain (which we will look at in our dataset).

**Solution:** Employing methods which assess the mean-variance relationship to help with the problem of estimating biological variability for experiments with small number of replicates. 

In this module, learners will use [R Statistical Software](https://www.r-project.org/) to walk-through activities designed to compare the performance of different tools (edgeR, DESeq2, limma-voom) for differential expression analysis of RNA-Seq data, and how the mean-variance relationship is addressed in datasets with increasing number of replicates.



> ## Learning Objectives 
>
> * 
> * 
> * 