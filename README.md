# R/SGCCA 

#### Author : Etienne CAMENEN

#### Key-words: 
omics, CCA, multi-block, multi-modal

#### EDAM operation
analysis, correlation, visualisation

#### Contact
etienne.camenen@gmail.com

#### Short description
Performs multi-variate analysis (PCA, CCA, PLS, R/SGCCA, etc.) and produces textual and graphical outputs (e.g. variables and individuals plots).

---

## Description
A user-friendly multi-blocks analysis (Regularized Generalized Canonical Correlation Analysis, RGCCA) with all default settings predefined. The software produces figures to explore the analysis' results: individuals and variables projected on two components of the multi-block analysis, list of top variables and explained variance in the model.
 
More information about:

* [RGCCA](https://cran.r-project.org/web/packages/RGCCA/vignettes/vignette_RGCCA.pdf)
* [input / output formats](https://github.com/BrainAndSpineInstitute/rgcca_ui#input-files)


## Usage instruction

### Installation
```
conda create -n rgcca -c icm-iconics r-rgcca=3.0.2
```

### Execution (with Russet data)
```
conda activate rgcca && \
cd ${CONDA_PREFIX} && \
wget https://github.com/BrainAndSpineInstitute/rgcca_ui/blob/master/inst/extdata/agriculture.tsv && \
Rscript inst/launcher.R -d agriculture.tsv
 ```
 
 More information about the command-line parameters [here](https://github.com/BrainAndSpineInstitute/rgcca_ui#command-line).