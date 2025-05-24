A fast, efficient, big-data and small memory software to detect significantly and suggested associated markers (QTNs).

Within R environment on the Linux server, the Fast3VmrMLM software can be installed by the following R codes:

First, install the dependency packages by:
install.packages(c("Rcpp", "RcppArmadillo", "RcppParallel", "Matrix", "BH", "data.table", "openxlsx", "dplyr", "MASS", "lars", "SKAT", "KScorrect", "BEDMatrix"))

Second, install the Fast3VmrMLM package from local files by:
install.packages("E:/Fast3VmrMLM_1.0.zip",repos=NULL,type="win.binary")

Reference

Wang J, Chen Y, Shu G, Zhao M, Zheng A, Chang X, Li G, Wang Y, Zhang YM. Fast3VmrMLM: A fast algorithm that integrates genome-wide scanning with machine learning to accelerate gene mining and breeding by design for polygenic traits in large-scale GWAS datasets. Plant Communications 2025, 101385 (https://www.cell.com/plant-communications/fulltext/S2590-3462(25)00147-6).
