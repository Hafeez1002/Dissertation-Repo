This is the repository for all the code, packages, and methodology used for my dissertation. The dissertation itself is an attempt to build a 1D CNN in order to classify which type of chaos dominates a given time series. Built from scratch, data generation in Julia, CNN architecture and training in Python, structured as a series of self-contained notebooks. This is so that it is easy to track my thought process along the way, as well as give me any advice you can along the way. I love criticism, so any tips will be greatly appreciated.

Hopefully along the way I can add a quantifier of the amount of chaos I have, rather than it just being a discrete process. For now, Project 0 talks about the importance of the project and the architecture that I intend to build for the entire process.

## Project Structure

| # | File | Language | Description |
|---|------|----------|-------------|
| **00** | `00_project_overview.ipynb` | Python | Motivation, theoretical background, and architecture plan |
| **01** | `01_deterministic_systems.jl` | Julia | Generate chaotic time series (Lorenz, Rössler, logistic map, Hénon, Mackey-Glass) |
| **02** | `02_stochastic_processes.jl` | Julia | Generate stochastic time series (white/coloured noise, random walk, ARMA, Ornstein-Uhlenbeck) |
| **03** | `03_dataset_assembly.ipynb` | Python | Load Julia CSVs, window, add noise augmentation, split into train/val/test |
| **04** | `04_cnn_architecture.ipynb` | Python | Define the 1D CNN layer by layer with full explanations |
| **05** | `05_training_pipeline.ipynb` | Python | Train with AdamW, LR scheduling, and early stopping |
| **06** | `06_evaluation.ipynb` | Python | Test set metrics, confusion matrix, ROC curve, confidence analysis |



## Reference

Boaretto, B.R.R. et al. (2021). *Evaluating temporal correlations in time series using permutation entropy, ordinal probabilities and machine learning.* Chaos, 31(6), 063124.
