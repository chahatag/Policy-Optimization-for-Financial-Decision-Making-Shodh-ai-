# Credit Risk Optimization: Deep Learning & Offline RL

## Project Overview
This repository contains the complete implementation of an end-to-end pipeline to optimize loan approval decisions. It combines **Exploratory Data Analysis**, a **Supervised Deep Learning Model** for risk prediction, and an **Offline Reinforcement Learning (DQN)** agent for profit maximization.

All code is consolidated into a single Jupyter Notebook to ensure easy reproducibility of the linear pipeline.

## Files Description
* **`Policy Optimization for Financial Decision-Making.ipynb`**: The main notebook containing:
    1.  **Data Preprocessing:** Cleaning, scaling, and handling class imbalance.
    2.  **Supervised Learning:** Training a PyTorch DL model (AUC/F1 metrics).
    3.  **Reinforcement Learning:** Training a DQN agent on offline data.
    4.  **Evaluation:** Comparative analysis of the DL model vs. RL Agent vs. Baseline.
* **`requirements.txt`**: List of Python dependencies required to run the notebook.

## Results Summary
| Strategy | Goal | Key Metric | Result |
| :--- | :--- | :--- | :--- |
| **Deep Learning** | Minimize Default Risk | F1-Score (Defaulters) | 0.44 |
| **RL Agent** | Maximize Portfolio Value | Avg Profit per Loan | $401.41 |
| **Baseline** | Standard Operations | Avg Profit per Loan | $401.87 |

**Key Findings:**
The Deep Learning model prioritized precision/recall (risk aversion), while the RL agent prioritized volume (profit maximization). Due to the dataset's high profitability ratio, the RL agent converged to a strategy similar to the baseline, highlighting the need for future reward shaping.

## How to Run
1. **Clone the repository:**
   ```bash
   git clone https://github.com/chahatag/Policy-Optimization-for-Financial-Decision-Making-Shodh-ai-.git
