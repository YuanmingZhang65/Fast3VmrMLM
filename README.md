A fast, efficient, big-data and small memory software to detect significantly and suggested associated markers (QTNs).

Within the Linux system, the Fast3VmrMLM software can be installed by the following four steps:

1) To download and install Anaconda at https://repo.anaconda.com/archive/, in which the recommended installer file is Anaconda3-2021.05-Linux-x86_64.sh.

2) To create a new conda environment named Fast3VmrMLM by the following code:

   •
   
       conda create -n "Fast3VmrMLM" r-essentials r-base=4.3
   
3) To install the dependency packages.
   
  •	Install mamba for fast installation by:
  
      conda install -c conda-forge mamba
      
  •	Install dependency packages by following codes in Linux environment (or by install.packages in R environment; the below “mamba” can be replaced by “conda” if it doesn’t work):
  
      mamba install -c conda-forge r-Rcpp
      
      mamba install -c conda-forge r-RcppArmadillo
      
      mamba install -c conda-forge r-RcppParallel
      
      mamba install -c conda-forge r-data.table
      
      mamba install -c conda-forge r-MASS
      
      mamba install -c conda-forge r-openxlsx
      
      mamba install -c conda-forge r-BH  
     
     
  •	Install dependency packages “boost” by the following code in Linux environment:
  
      conda install -c conda-forge boost
      
4) To decompress Fast3VmrMLM.zip with the following bash code and install it with R code by:
   
   unzip '/user/Fast3VmrMLM_Linux.zip' -d '/user/'

   R

   install.packages("/home/user/Fast3VmrMLM", repos = NULL)


The above installation may take some time, please be patient and wait.

The Fast3VmrMLM method combines multiple statistical and computational techniques with the 3VmrMLM method to significantly optimize computation speed and memory consumption. Large-scale genetic analysis can be performed on small servers. This study develops a novel method to large-scale gene mining and breeding by design for polygenic traits, including human diseases and crop yield. Both simulation studies and real-data analysis demonstrated that 3VmrMLM and Fast3VmrMLM outperform most GWAS methods in terms of statistical power and false-positive rate.

Most types of genetic population can be used in the Fast3VmrMLM software for GWAS, including homozygous cultivars, hybrid F1 cultivars, heterogeneous accessions with heterozygous marker genotypes, NAM and MAGIC, and parents and their hybrids in the NC II design (requiring only a parental marker genotypic dataset; marker genotypes of the hybrid F1 offspring can be inferred from their parents even if the parents contain heterozygous genotypes in weeds and fruit trees).

The types of markers include SNPs, bin haplotypes, gene haplotypes, lncRNA types and structural variations.

Reference

Wang J, Chen Y, Shu G, Zhao M, Zheng A, Chang X, Li G, Wang Y, Zhang YM. Fast3VmrMLM: A fast algorithm that integrates genome-wide scanning with machine learning to accelerate gene mining and breeding by design for polygenic traits in large-scale GWAS datasets. Plant Communications 2025, 101385 (https://www.cell.com/plant-communications/fulltext/S2590-3462(25)00147-6).
