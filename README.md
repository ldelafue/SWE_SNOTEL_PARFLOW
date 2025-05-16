# SWE_SNOTEL_PARFLOW
 
By using the code, you agree to cite:

> *De la Fuente et al 2024. Improving Basin-Scale Estimation of Snow Water Equivalent via Process-Model-Based Augmentation of Observational Data, Preprint*
 
## Getting started
To run the code, you must first set up the conda environment. You must use the following lines to clone the repo and create the environment (the last step may take some time):
```
git clone git@github.com:ldelafue/SNOW_SNOTEL_PARFLOW.git
cd your_local_github_repository/SNOW_SNOTEL_PARFLOW
conda env create -f environment.yml
```

## Data
Two sources of data are needed to run the notebook. The first one is the raw data, which can be found at https://hf-hydrodata.readthedocs.io/en/latest/gen_conus1_baseline_mod.html. SNOTEL and PARFLOW-CLM simulations can be retrieved from this project. 
The experiment results done in the paper must be downloaded from the link https://drive.google.com/file/d/1io7SYwBgPqlOVi4hrAby7m7-9bv8OY6_/view?usp=share_link and placed in the git folder.
The UA-SWE data for the comparison done in the supplement information requires downloading the WY2006 UA-SWE data from this link https://daacdata.apps.nsidc.org/pub/DATASETS/nsidc0719_SWE_Snow_Depth_v1/

## Analysis folder
This folder has the Jupyter notebook (the only file that must be run by the user) and the files used to create each of the figures presented in the paper. All the figures are contained in the Jupyter notebook Figures_paper.ipynb.

## exp1 and exp2 folder
This folder only contains the summary results of the experiments, given that saving each of the grid files from each run at the CONUS scale has a size of 10 GB. The Jupyter notebook uses the files contained in it, so they are not intended to be clearly understandable for the user.
The files "conus1_2005_preprocessed.zarr" and "conus1_2006_preprocessed.zarr" used in the Jupyter notebook correspond to the ParFlow-CLM simulations that can be accessed through HydroFrame©.

## Training code
The folder code inside the folders exp1 and exp2 has the main Python code used to train and evaluate the models. However, these files are not intended to run the code by any user, given that many of the functions and libraries are part of the HydroFrame© project, and they are not freely available. Therefore, the codes provided only give an overall understanding of the Python code used.   
