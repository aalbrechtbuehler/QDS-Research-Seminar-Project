# QDS Research Seminar Project

This repository contains the analysis pipeline for investigating the structure of cichlid postural behaviour, including preprocessing, statistical analysis, and Markov modelling.

## Repository Structure

To run the full pipeline, organize your working directory as follows:

```
project_folder/
├── PrettyDat.csv
├── preprocessing.ipynb
├── SamplingAndSims.ipynb
├── rAnalysis.rmd
```

## Usage Guide

### 1. Preprocessing

Run `preprocessing.ipynb` to generate species-specific corpora from the raw dataset.

* **Input:** `PrettyDat.csv`
* **Output:** `.txt` files containing postural sequences for each species

### 2. Summary Statistics & Eigenvalue Analysis

Statistical summaries and eigenvalue decay analyses are implemented in:

```
rAnalysis.rmd
```

This script produces:

* Summary statistics of sequence data
* Eigenvalue decay diagnostics
* Marginal state distribution temporal dynamics

### 3. Markov Modelling & Simulations

Higher-order Markov models and synthetic simulations are implemented in:

```
SamplingAndSims.ipynb
```

This notebook includes:

* k-order Lagged vs. Collapsed Context Model fitting
* Simulation evaluations of model performance

