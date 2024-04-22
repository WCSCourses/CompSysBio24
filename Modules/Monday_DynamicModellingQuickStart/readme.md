# Getting started with dynamic modelling

This repository contains materials for getting started with executable models.

This is an arbitrary example - and is not meant to necessarly represent a "gold standard" in how this type of modelling is performed. 
This exercise is instead meant to serve as an introduction to possible workflows and analysis, so that when they are covered in detail at a later stage, you have a better idea of how each type of analysis fits into a possible workflow.


In this exercise we will be analysing data from: 
"Differential RNA-seq analysis comparing APC-defective and APC-restored SW480 colorectal cancer cells" https://doi.org/10.1016/j.gdata.2016.02.001

In this study, authors have taken a colorectal cancer cell line that is mutant (defective) for the gene APC - a known tumor driver and restored the functional APC. RNAseq has been collected for the WT cell line, the APC restored cell line, and a vector control (a cell line given the mutation vector but without the mutation). 

In this exercise we will:

- Perform differential expression analysis of the RNAseq data
- Identify pathways and genes associated with the mutation
- Build a signalling map of the network of these genes
- Convert this map into a series of logical models using different modelling tools
- Perform analysis and generate biological insights based on these models

To get started, work with the notebook: "APC_mutation.ipynb"

Before opening the notebook, download all dependencies with conda using

```
conda env create -f environment.yml
conda activate quickstart
curl https://sh.rustup.rs -sSf | sh -s -- -y
export PATH="$PATH:$HOME/.cargo/bin"
pip install gseapy casq
```
