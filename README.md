# PlasmaMutationDetectorForLilab
Tumor Mutation Detection in Plasma For Li lab (in linux)

release 1.7.2 For Lilab: version for ZhiGuang Li lab developed by ywliao from Yves's version. Mainly changed:
               1. vcf file from NCBI can be used as input (ftp://ftp.ncbi.nlm.nih.gov/snp/organisms/human_9606/VCF/), hg38 version should be used
               2. Add some message to report input
               3. ntrim default to 2
               4. remove positions which mutation reads haven't been read, or only one read support mutation
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
From the command line and in the directory where FindPeek github was cloned.
```R CMD INSTALL PlasmaMutationDetectorForLilab ```

### Usage
```?MutHeatmap```to access the documentation pages for function MutHeatmap
