# README
This repository contains the scripts (in jupyter notebooks) to generate the figure in the manuscript **"[Pangenome mining of the Streptomyces genus redefines their biosynthetic potential](https://doi.org/10.1101/2024.02.20.581055)"**.

# USAGE
## 1. Clone this repository
```bash
git clone https://github.com/NBChub/Streptomyces_pangenome_ms.git 
```

## 2. Set up BGCFlow
```bash
# create and activate new conda environment
conda create -n bgcflow pip -y
conda activate bgcflow

# install BGCFlow wrapper
pip install git+https://github.com/NBChub/bgcflow_wrapper.git

# clone BGCFlow to "bgcflow" folder
bgcflow clone bgcflow
```

## 2. Set configurations
```bash
# edit the location of the bgcflow dir to the right directory with dataset
nano config.yaml
```

## 3. Setting up Conda Environments
Install these conda environments:
```bash
mamba env create -f python_notebook.yaml
mamba env create -f r_notebook.yaml
```

## 4. Run the notebooks
- There are two kind of notebooks, R (*.R.ipynb) and python (*.python.ipynb)
- Run the notebook using the corresponding conda environment: `python_notebook` or `r_notebook`
- Start jupyter session
```bash
# for python
conda activate python_notebook
jupyter lab
```
```bash
# for R
conda activate r_notebook
jupyter lab
```
- Run the notebooks in order

# Citation
> Mohite et al. (2024). Pangenome mining of the Streptomyces genus redefines their biosynthetic potential. bioRxiv 2023.06.14.545018; doi: [https://doi.org/10.1101/2024.02.20.581055](https://doi.org/10.1101/2024.02.20.581055)
