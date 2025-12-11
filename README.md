# cse598-002 — Conditional Diffusion Insulin Control (Offline RL)
CSE 598-002: AI for Science — Fall 2025

This project implements a **conditional diffusion model** for safe insulin dosing in Type 1 diabetes using offline reinforcement learning. The model is trained on expert trajectories and evaluated on virtual patients from the SimGlucose / UVA–Padova environment.

## Baselines
We compare our diffusion policy against several standard controllers:
- **PID Controller**
- **Tabular Q-Learning**
- **TD3-BC**
- **Clinical Controller** (benchmark)

Our diffusion model learns a distribution over safe bolus doses conditioned on the patient state and shows strong performance, particularly on adult virtual patients over 24h, 3-day, and 7-day horizons.

## Running the Code
- The full pipeline is implemented in a Colab notebook and is self-contained.
- Install the **SimGlucose** package for environment imports.
- The diffusion model and all baselines run with standard Python packages.
- Update the `wandb` login key if using Weights & Biases.

## Notes
- Only bolus insulin actions are modeled, so the action dimension must remain **1**.
- Key hyperparameters can be adjusted at the top of the notebook.

## Authors
**Sathvika Ayyappa Prabhu**  
**Matthew Manion**  
University of Michigan — Fall 2025
