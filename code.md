# Code

This page highlights selected research code and reproducible analysis projects related to my work in causal AI.

## Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions

This repository contains the code and data for the paper *Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions: Evidence from the UK COVID-19 Policies*. The project compares four econometric methods and eleven causal structure-learning algorithms on a UK COVID-19 time-series dataset, with a focus on policy-relevant inference and decision support.

The repository includes raw data, supporting documentation, and analysis scripts for the full workflow, including missing-data imputation, discretisation for dynamic Bayesian network parameterisation, model averaging across econometric graphs, and causal-effect estimation using the do-operator. Expected outputs include graph files for multiple methods, a VAR lag-selection plot, and a pairwise SHD comparison figure.

- [GitHub repository](https://github.com/br1pa/econometric-vs-causal-time-series)
- Related paper: *Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions: Evidence from the UK COVID-19 Policies*

### Repository contents

- `data/` — input data used in the analysis
- `docs/` — codebook and reproducibility notes
- `scripts/` — analysis scripts for the project

### Methods and tools

This project brings together econometric modelling, causal structure learning, graph comparison, and intervention-focused analysis. The repository is written in R and uses packages for time-series modelling, Bayesian network learning, graph analysis, causal effect estimation, and visualisation.

## GitHub

- [GitHub profile](https://github.com/br1pa)
- [Econometric vs. Causal Time-Series repository](https://github.com/br1pa/econometric-vs-causal-time-series)
