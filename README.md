# PlasmaMutationDetectorForLilab
Tumor Mutation Detection in Plasma For Li lab (in linux)

#### Description: 
Aims at detecting single nucleotide variation
    (SNV) and insertion/deletion (INDEL) in circulating tumor DNA (ctDNA), used
    as a surrogate marker for tumor, at each base position of an Next Generation
    Sequencing (NGS) analysis. Mutations are assessed by comparing the minor-allele
    frequency at each position to the measured PER in control samples.
#### Imports: 
S4Vectors (>= 0.16.0), Rsamtools (>= 1.30.0), rtracklayer (>=
        1.38.0), robustbase (>= 0.92-8), SummarizedExperiment (>=
        1.8.0), data.table (>= 1.10.4)
#### Depends: 
R (>= 3.4.0), ggplot2 (>= 2.2.0), grid (>= 3.4.0),
        GenomicRanges (>= 1.30.0), data.table (>= 1.10.4), VariantAnnotation (>= 1.24.0)


#### release 1.7.2 For Lilab
version for ZhiGuang Li lab developed by ywliao from Yves's version. Mainly changed:
 1. vcf file from NCBI can be used as input (ftp://ftp.ncbi.nlm.nih.gov/snp/organisms/human_9606/VCF/), hg38 version should be used
 2. Add some message to report input
 3. The ntrim default to 2
 4. Remove positions which mutation reads haven't been read, or only one read support mutation
 5. Correct frequency  in revert position

## installation
#### Option 1(Recommended)
Using devtools
```
install.packages("devtools")
library(devtools)
install_github("DMU-lilab/PlasmaMutationDetectorForLilab")
```
### Option 2
Manual installation
#### Checkout the latest release of PlasmaMutationDetectorForLilab from GitHub
```git clone https://github.com/DMU-lilab/PlasmaMutationDetectorForLilab.git```

#### Install the FindPeek package
From the command line and in the directory where PlasmaMutationDetectorForLilab github was cloned.
```R CMD INSTALL PlasmaMutationDetectorForLilab ```

### Usage
Please refer to the original version of manual.
https://cran.r-project.org/web/packages/PlasmaMutationDetector/index.html
