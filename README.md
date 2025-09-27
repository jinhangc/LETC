# LETC: Localized-Exploration-then-Commit Algorithm In Linear Contextual Pricing

Paper: Localized Exploration in Contextual Dynamic Pricing Achieves Dimension-Free Regret

## Introduction
This repo contains scripts of simulation and real data analysis for our paper.
This README file provides instructions to reproduce the result in the numerical studies section of our paper. 
- `LinearDP.ipynb` includes the simulation results, i.e., regret curves for our algorithm vs offline policy.
- `LinearDP_data_exp1.ipynb` includes the first real-data experiment, i.e., revenue improvements across different products.
- `LinearDP_data_exp2.ipynb` includes the second real-data experiment, i.e., regret curves for two randomly-chosen products.
For the product 'Misc School Supplies SKU 17', set `selected=0` at the beginning, then run the entire code file; for 'Classification Folders SKU 11', set `selected=1`.


The demand model has the following linear form:
$D_t=x_t^T {\alpha}^\star+p_t({x}_t^T {\beta}^\star)+\epsilon_t$


The regret is defined as
$\mathcal{R}(T):=\sum_{t=1}^T p^\star(x_t)\left(x_t^T {\alpha}^\star+p^\star(x_t){x}_t^T {\beta}^\star\right)- p_t\left(x_t^T {\alpha}^\star+p_t{x}_t^T {\beta}^\star\right)$

Our paper achieves first dimension-free and also minimax optimal regret rate.

