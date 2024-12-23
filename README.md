# SWE_SNOTEL_PARFLOW
 
By using the Code you agree to cite:

> *De la Fuente et al 2024. Improving Basin-Scale Estimation of Snow Water Equivalent via Process-Model-Based Augmentation of Observational Data, Preprint*
 
## Getting started
To run the code you must set up the conda environment first. You must use the follow lines to clone the repo and create the environment (the last step may take some time):
```
git clone git@github.com:ldelafue/SNOW_SNOTEL_PARFLOW.git
cd your_local_github_repository/SNOW_SNOTEL_PARFLOW
conda env create -f environment.yml
```

## Data
There are two sources of data needed to run all the notebooks. The first one is the raw data that can be found at https://hf-hydrodata.readthedocs.io/en/latest/gen_conus1_baseline_mod.html. SNOTEL and PARFLOW-CLM simulations can be retrival from this project. 
The experiment results done in the paper must be downloanded from the link XXX and placed in the git folder.

## Analysis folder
This folder has the jupyter notebook and the files used to create each of the figures presented in the paper. All the figures are contained in the jupyter notebook Figures_paper.ipynb.

## exp1 and exp2 folder
This folder has some of the results of the experiment done across the paper.