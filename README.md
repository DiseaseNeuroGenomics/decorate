
# decorate: Differential Epigenetic Correlation Test

![alt text](https://hoffmg01.u.hpc.mssm.edu/software/decorate/workflow.png)

# Install
```r
library(devtools)

# first install sLED
install_github("lingxuez/sLED")

# Install decorate
# 	first, check for Bioconductor
if (!requireNamespace("BiocManager", quietly = TRUE)){
	cat("Please install Bioconductor before continuing:\n")
	cat("see http://bioconductor.org/install/\n\n")
}else{
	install_github('GabrielHoffman/decorate', repos=BiocManager::repositories())
}   
```

# Dependencies
Depending on your system, you may need to install these dependencies first: 
- udunits 
- proj
- gdal 
- geos

###### Mac OS X
```brew install udunits proj gdal geos```

###### Ubuntu
```sudo apt-get install libudunits2-dev libproj-dev proj-data proj-bin libgeos-dev libgeos-c1v5 libgdal-dev```

###### CentOS
You will need to install these same dependencies, but I don't have experience with the CentOS package manager.

###### Windows
Although I have not tried to install these dependencies on Windows, decorate should install on Windows with no issues.

## [Vignette: run example analysis](https://hoffmg01.u.hpc.mssm.edu/software/decorate/decorate_example.html)

## [Simulations and properties of methods](https://hoffmg01.u.hpc.mssm.edu/software/decorate/simulations.html)

## Data analysis from manuscript
 - [DNA methylation from kidney renal clear cell carcinoma](https://hoffmg01.u.hpc.mssm.edu/software/decorate/KIRC.html)
 - [DNA methylation from schizophrenia brains](https://hoffmg01.u.hpc.mssm.edu/software/decorate/methyl_scz_decorate.html)
 - [ATAC-seq from schizophrenia brains](https://hoffmg01.u.hpc.mssm.edu/software/decorate/atac_local_corr.html)
 - [Histone modification ChIP-seq from human brain](https://hoffmg01.u.hpc.mssm.edu/software/decorate/EpiMap.html)

  [Results files](https://www.synapse.org/#!Synapse:syn20742092)

  [Analysis code](https://github.com/GabrielHoffman/decorate_analysis)
