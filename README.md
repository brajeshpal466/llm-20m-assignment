# 20M LLM Training Assignment (Session 13)

**Short caption:** Training a 20M‑parameter language model on 50 M tokens with reversible optimizers – Colab notebooks and results.

## Overview
This repository contains notebooks and scripts to train a ~20 M‑parameter GPT‑style language model on synthetic data (≈50 M tokens) using Google Colab. The workflow includes:
1. Baseline training with the largest batch size that fits the GPU.
2. Training with reversible optimizers (mid‑point, symplectic Euler, etc.) – reporting which variant works.
3. Training with the chosen reversible optimizer while pushing batch size to its maximum.

The notebooks log final loss, throughput (tokens / s), peak memory usage, and observations.

## Repository Structure
- `01_prepare_data.ipynb` – generate synthetic token stream.
- `02_train_baseline.ipynb` – baseline training script.
- `03_train_reversible.ipynb` – reversible optimizer experiments.
- `04_train_reversible_max_batch.ipynb` – max‑batch reversible training.
- `utils.py` – helper functions for logging, memory profiling, and token throughput.
- `requirements.txt` – Python dependencies.

## How to Use
1. Open any notebook in Google Colab (or locally).
2. Install the dependencies:
```bash
pip install -r requirements.txt
```
3. Run the cells sequentially.

## Results (to be filled after experiments)
- Final loss: ...
- Throughput: ... tokens/s
- Peak memory: ... GB
- Best reversible variant: ...

---
*Repository for Session 13 assignment.*
