# cdd2021
Repository for the subject CDD


## Requirements
You will need rdkit (and potentionaly with postgres database), but Conda, Jupyter and Git are also very useful. 

### git
Linux
```bash
sudo apt install git
```

Windows and Apple
Download and install from [git](https://git-scm.com/downloads)

### conda
Linux
```bash
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
# you will need probably to run:
# chmod u+x Miniconda3-latest-Linux-x86_64.sh to run this script
./Miniconda3-latest-Linux-x86_64.sh
```

Windows
Download and install [miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/windows.html)

Apple
Download and install [miniconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/macos.html)


## Get started with rdkit with jupyter
Should work in all consoles
```bash
git clone https://github.com/lich-uct/cdd2021.git
# create environment with rdkit, preferably updated version
# cdd is name of the environment
conda create -n cdd -c rdkit -c conda-forge rdkit=2019 jupyterlab 
conda activate cdd
jupyter lab # if you want to run it locally
jupyter lab --ip 0.0.0.0 --port XXXX # ip 0s to see jupyter on the Internet, port XXXX as maybe you don't want to run it on default 8888 port
# jupyter notebook --ip 0.0.0.0 --port XXXX alternative if you want only notebooks
```

## What to do
 On your part, please try to apply the workflows onto your particular set, and adapt them for your particular cases.$

 The example jupyter notebooks with the workflows will be uploaded into the /exercises folder of the repository. I w$

 Make your own folders in the root of the repository; e.g. 'vorsilam'. Place your own data and notebooks and all oth$

## Current exercises
 - [exercises/1_getting_started](exercises/1_getting_started.ipynb): How to parse structures into RDKit, visualize t$


## What expect to pass the exercises
You will work on your projects, or 'zapoctovy projekt', projects will involve roughly the following:
 - Picking a set of known biologically active structures, load and process it using RDkit
 - Performing a basic analysis of the set, descriptors, scaffolds, fingerprints, similarities, etc.
 - Comparing the properties of your picked set with other sets
 - Trying out some standard cheminformatic methods on the sets
 - Preparing set visualizations
 - Making a basic classifier related to your picked and prepared dataset

 The extent and exact form of all above points will be determined ad-hoc, depending on time, situation, progress, etc. We will periodically upload jupyter notebooks that describe the steps of the next task, the reasoning behind them, and their demonstration on an example set.

## Resources
 - [Getting started with RDKit in Python](http://www.rdkit.org/docs/GettingStartedInPython.html)
 - [RDKit documentation](https://www.rdkit.org/docs/)
