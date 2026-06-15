# Physics-guided Quantile Probabilistic Precipitation Forecasting

This repository contains the code for a physics-guided quantile probabilistic forecasting framework for short-term precipitation prediction. The study focuses on cross-regional transfer learning from the UK source domain to the Ireland target domain using ERA5 reanalysis data.

## Overview

The proposed framework combines:

- Quantile regression for probabilistic precipitation forecasting
- Physics-guided gate mechanism using surface pressure and total cloud cover
- Transfer learning from the UK to Ireland
- Extreme precipitation weighting for heavy rainfall samples
- Evaluation across different forecast lead times

## Forecast Lead Times

The experiments include three forecast lead times:

- t+1
- t+6
- t+12

## Main Models

The repository includes implementations of:

- Deterministic LSTM baseline
- Quantile LSTM
- Physics-guided Quantile LSTM
- Quantile Transformer
- Physics-guided Quantile Transformer
- Fine-tuning and zero-shot transfer experiments
- Ablation studies

## Evaluation Metrics

The models are evaluated using:

- RMSE
- R²
- Prediction interval coverage
- Critical Success Index (CSI)
- False Alarm Rate (FAR)

## Repository Structure

```text
.
├── t_1/          # Experiments for t+1 lead time
├── t_6_12/       # Experiments for t+6 and t+12 lead times
├── figures/      # Generated figures
└── README.md
