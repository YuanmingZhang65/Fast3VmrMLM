A fast, efficient, big-data and small memory software to detect significantly and suggested associated markers (QTNs).

Within R environment on the Linux server, the Fast3VmrMLM software can be installed by the following R codes:

First, install the dependency packages by:
install.packages(c("Rcpp", "RcppArmadillo", "RcppParallel", "Matrix", "BH", "data.table", "openxlsx", "dplyr", "MASS", "lars", "SKAT", "KScorrect", "BEDMatrix"))

Second, install the Fast3VmrMLM package from local files by:
install.packages("E:/Fast3VmrMLM_1.0.zip",repos=NULL,type="win.binary")

The Fast3VmrMLM method combines multiple statistical and computational techniques with the 3VmrMLM method to significantly optimize computation speed and memory consumption. Large-scale genetic analysis can be performed on small servers. This study develops a novel method to large-scale gene mining and breeding by design for polygenic traits, including human diseases and crop yield. Both simulation studies and real-data analysis demonstrated that 3VmrMLM and Fast3VmrMLM outperform most GWAS methods in terms of statistical power and false-positive rate.

Most types of genetic population can be used in the Fast3VmrMLM software for GWAS, including homozygous cultivars, hybrid F1 cultivars, heterogeneous accessions with heterozygous marker genotypes, NAM and MAGIC, and parents and their hybrids in the NC II design (requiring only a parental marker genotypic dataset; marker genotypes of the hybrid F1 offspring can be inferred from their parents even if the parents contain heterozygous genotypes in weeds and fruit trees).

The types of markers include SNPs, bin haplotypes, gene haplotypes, lncRNA types and structural variations.

Reference
Wang J, Chen Y, Shu G, Zhao M, Zheng A, Chang X, Li G, Wang Y, Zhang YM. Fast3VmrMLM: A fast algorithm that integrates genome-wide scanning with machine learning to accelerate gene mining and breeding by design for polygenic traits in large-scale GWAS datasets. Plant Communications 2025, 101385 (https://www.cell.com/plant-communications/fulltext/S2590-3462(25)00147-6).
