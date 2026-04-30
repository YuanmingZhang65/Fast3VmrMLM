A fast, efficient, big-data and small memory software to detect QTNs and QTN-by-environment interactions. The software packages (x86 and arm architectures of Linux system) were updated on April 30 2026.

When the population size is less than 1,000, the probability threshold in the first stage should be set to 0.01 or 0.05. As the population size increases, this threshold in the first stage may be set to a value below 0.01 (for example, svpal = 0.05 or 0.01 for a population size of less than 4,000, and svpal = 1e–5 for a population size of more than 20,000).

Within the Linux system, the Fast3VmrMLM software can be installed by the following four steps:

1) To download and install Miniconda3 at https://repo.anaconda.com/miniconda/, in which the recommended installer file is Miniconda3-py38_23.11.0-2-Linux-x86_64.

2) To create a new conda environment named Fast3VmrMLM and install R version 4.3 by the following code.

 •	create a new conda environment named Fast3VmrMLM and install R v4.3:
 
      conda create -n "Fast3VmrMLM" r-essentials r-base=4.3
      conda activate Fast3VmrMLM

3) To install the dependency packages.

  •	Install dependency packages by following codes in Linux environment (or by install.packages in R environment):

      conda install -c conda-forge r-Rcpp=1.1.0 r-RcppArmadillo=15.0.2_1 r-data.table=1.15.2 r-RcppParallel=5.1.9 r-MASS=7.3_60.0.1 r-openxlsx=4.2.8 r-BH=1.87.0_1

4) Downloading Fast3VmrMLM from Github and installing it:

  •   Downloading via R code in R environment (R version 4.3):
  
      download.file("https://github.com/YuanmingZhang65/Fast3VmrMLM/archive/refs/heads/main.zip", destfile = "Fast3VmrMLM-main.zip",mode = "wb")

 •   Installing Fast3VmrMLM in R environment (R version 4.3):

      unzip("Fast3VmrMLM-main.zip")
      unzip("Fast3VmrMLM-main/Fast3VmrMLM_Linux_2.0.zip")
      install.packages("Fast3VmrMLM", repos = NULL)

The above installation may take some time, please be patient and wait. Once the software Fast3VmrMLM is installed, users may run it using two commands:

      library("Fast3VmrMLM")
      Fast3VmrMLM(***)	(please see the example in Instruction 2.0.pdf)

The Fast3VmrMLM method combines multiple statistical and computational techniques with the 3VmrMLM method to significantly optimize computation speed and memory consumption. Large-scale genetic analysis can be performed on small servers. This study develops a novel method tolarge-scale gene mining and breeding by design for polygenic traits, including human diseases and crop yield. Both simulation studies and real-data analysis demonstrated that 3VmrMLM and Fast3VmrMLM outperform most GWAS methods in terms of statistical power and false-positive rate.

Most types of genetic population can be used in the Fast3VmrMLM software for GWAS, including homozygous cultivars, hybrid F1 cultivars, heterogeneous accessions with heterozygous marker genotypes, NAM and MAGIC, and parents and their hybrids in the NC II design (requiring only a parental marker genotypic dataset; marker genotypes of the hybrid F1 offspring can be inferred from their parents even if the parents contain heterozygous genotypes in weeds and fruit trees).

The types of markers include SNPs, bin haplotypes, gene haplotypes, lncRNA types and structural variations.

References

Wang JT#, Chen Y#, Shu GP#, Zhao MM#, Zheng A, Chang XY, Li GQ, Wang YB, Zhang YM*. Fast3VmrMLM: A fast algorithm that integrates genome-wide scanning with machine learning to accelerate gene mining and breeding by design for polygenic traits in large-scale GWAS datasets. Plant Communications 2025; 6(7): 101385 (https://doi.org/10.1016/j.xplc.2025.101385).

Wang JT#, Han XL#, Zhao MM, Zhang HQ, Chen Y, Jiang QY and Zhang YM*. A fast method for breeding by design via G×E interactions detected in large-scale climatic, phenomic and genomic data. National Science Review 2026, 13, nwag095, online (https://doi.org/10.1093/nsr/nwag095).
