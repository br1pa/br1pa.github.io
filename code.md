# Code

This page highlights selected research code and reproducible analysis projects related to my work in causal AI.

## Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions

This repository contains the code and data for the paper *Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions: Evidence from the UK COVID-19 Policies*. The project compares four econometric methods and eleven causal structure-learning algorithms on a UK COVID-19 time-series dataset, with a focus on policy-relevant inference and decision support.

The repository includes raw data, supporting documentation, and analysis scripts for the full workflow, including missing-data imputation, discretisation for dynamic Bayesian network parameterisation, model averaging across econometric graphs, and causal-effect estimation using the do-operator. Expected outputs include graph files for multiple methods, a VAR lag-selection plot, and a pairwise SHD comparison figure.

- [GitHub repository](https://github.com/br1pa/econometric-vs-causal-time-series)
- Related paper: [*Econometric vs. Causal Structure-Learning for Time-Series Policy Decisions: Evidence from the UK COVID-19 Policies*](https://arxiv.org/abs/2603.00041)

### Repository contents

- `data/` — input data used in the analysis
- `docs/` — codebook and reproducibility notes
- `scripts/` — analysis scripts for the project

### Methods and tools

This project brings together econometric modelling, causal structure learning, graph comparison, and intervention-focused analysis. The repository is written in R and uses packages for time-series modelling, Bayesian network learning, graph analysis, causal effect estimation, and visualisation.

## Variable-Lag Tabu Search for Time-Series Causal Discovery

This repository contains the code for the paper *Time Series Causal Discovery with Variable Lags*. The project introduces a Tabu-based structure-learning algorithm for multivariate time-series causal discovery, allowing each directed edge to have its own lag within a user-specified maximum lag.

The method learns temporally ordered causal graphs in which edges point from past to future values, making the corresponding time-unrolled graph acyclic. It uses a decomposable BIC-based score with node-specific effective sample sizes and an explicit lag-length penalty, encouraging parsimonious delay assignments while retaining longer lags when they improve model fit.

The repository includes the main sequential implementation, a parallel implementation for improved scalability, synthetic simulation scripts, analysis utilities, and a real-world UK COVID-19 policy application.

- [GitHub repository](https://github.com/br1pa/variable-lag-tabu)
- Related paper: [*Time Series Causal Discovery with Variable Lags*](https://arxiv.org/abs/2605.04081)

### Repository contents

- `src/variable_lag_tabu.py` — main sequential implementation
- `src/variable_lag_tabu_parallel.py` — parallel implementation
- `src/sweep_variable_lag_bn.py` — synthetic simulation sweeps
- `src/real_world_application.py` — real-world UK COVID-19 policy application
- `src/analysis.py` — analysis helper script

### Methods and tools

This project focuses on score-based causal discovery for time-series data. It combines Tabu search, edge-specific lag optimisation, decomposable BIC-style scoring, lag regularisation, mixed continuous and binary local models, and parallel neighbourhood evaluation.

## GitHub

- [GitHub profile](https://github.com/br1pa)
- [Variable-Lag Tabu repository](https://github.com/br1pa/variable-lag-tabu)
- [Econometric vs. Causal Time-Series repository](https://github.com/br1pa/econometric-vs-causal-time-series)
