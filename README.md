# GNN Final Project: Host Risk Forecasting on LANL Cyber-1

This repo contains my final project on the LANL Cyber-1 authentication logs. The main goal is to study host-level risk over time using the authentication stream, starting with exploratory analysis and simple baselines, and then moving to a temporal graph-based model in PyTorch.

## Notebooks

`lanl_cyber1_eda.ipynb`  
Explores the LANL authentication data and motivates the modeling setup

`baselines.ipynb`  
Builds non-graph baselines for the same host-level prediction task

`lanl_temporal_host_risk.ipynb`  
Main modeling notebook. Contains the temporal pipeline, host-memory updates, event replay, attention over recent events, training, evaluation, and metrics.

## Data

Place the LANL Cyber-1 files in `../project/data/` so the notebooks can find them:

- `../project/data/auth.txt.gz`
- `../project/data/redteam.txt.gz`

## Environment

You will need a recent Python 3 environment with the usual data and ML packages, including:

- `numpy`
- `pandas`
- `matplotlib`
- `scikit-learn`
- `torch`
- `tqdm`
- `jupyter`
