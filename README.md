# Smart Grid Fault Detection — PhD Research

**Institution:** University of the Witwatersrand (Wits), Johannesburg  
**Researcher:** Eng. Mhlanga (C. Eng.)  
**Programme:** Electrical Engineering  
**Status:** Active — Phase 1: Dataset Generation  

---

## Research Title

> *AI-Based Fault Detection and Classification in Smart Power Grids Using Hybrid Machine Learning and Physics-Informed Neural Network Frameworks*

---

## Objective

To develop and validate a hybrid AI framework for real-time fault detection and multi-class classification in Smart Power Grids — combining Physics-Informed Neural Networks (PINNs) with LSTM, CNN, and XGBoost architectures, trained on a simulation-generated dataset from the IEEE 39-bus benchmark network.

---

## Framework Architecture

PowerWorld Simulator (IEEE 39-bus)  
>  
Transient Stability Simulation  
>  
Fault Injection (SLG / LL / LLG / 3-Phase)  
>  
Time-Series CSV Export (V, I, f, RoCoF)  
>  
Feature Engineering (RMS, Wavelets, Sequences)  
>  
PINN-LSTM-CNN-XGBoost Hybrid Model  
>  
Fault Detection + Classification + Location  
>  
IEC 61850 GOOSE Deployment Feasibility

---

## Fault Scenarios

| Parameter | Range |
|---|---|
| Fault Types | SLG, LL, LLG, 3-Phase |
| Network | IEEE 39-bus (New England) |
| IBR Penetration | 0%, 30%, 50%, 70% |
| Fault Impedance | 00, 50, 200, 500 |
| Loading Levels | 50%, 75%, 100%, 115% |
| Target Dataset Size | ~25,000–40,000 labelled events |

---

## Tech Stack

| Layer | Tools |
|---|---|
| Simulation | PowerWorld Simulator v23 |
| Data Processing | Python, NumPy, Pandas, SciPy |
| Feature Engineering | PyWavelets, Scikit-learn |
| Deep Learning | PyTorch, TensorFlow/Keras |
| Ensemble ML | XGBoost, Scikit-learn |
| Experiment Tracking | MLflow, Optuna |
| Version Control | Git, GitHub |

---

## Repository Structure

smart-grid-fault-detection/
+-- powerworld_cases/       # .pwb simulation case files
+-- data/
¦   +-- raw/                # Exported CSVs from PowerWorld
¦   +-- processed/          # Cleaned, windowed, labelled datasets
¦   +-- external/           # PMU validation datasets
+-- src/
¦   +-- simulation/         # Dataset generation scripts
¦   +-- features/           # Feature extraction pipeline
¦   +-- models/             # Baseline, LSTM, CNN, PINN, Hybrid
¦   +-- utils/              # Loaders, evaluation, visualisation
+-- notebooks/              # Jupyter exploration and results
+-- results/
¦   +-- plots/              # Figures for report and publication
¦   +-- metrics/            # Accuracy, F1, AUC, latency CSVs
¦   +-- models/             # Saved model weights
+-- report/
¦   +-- figures/            # Publication-quality figures
¦   +-- chapters/           # Report chapter drafts
+-- requirements.txt
+-- README.md

---

## Progress Log

| Phase | Description | Status |
|---|---|---|
| Phase 1 | Literature review + proposal | >> Complete |
| Phase 2 | IEEE 39-bus model setup + fault injection | >> In Progress |
| Phase 3 | PINN architecture development | >> Pending |
| Phase 4 | Hybrid model training + optimisation | >> Pending |
| Phase 5 | Benchmarking + IEC 61850 validation | >> Pending |

---

## Publications (Planned)

- [ ] Systematic literature review — *IEEE Transactions on Power Delivery*
- [ ] Dataset methodology + baseline results — *IEEE PES General Meeting*
- [ ] PINN-hybrid framework — *IEEE Transactions on Neural Networks and Learning Systems*
- [ ] Deployment feasibility — *IEEE Transactions on Smart Grid*

---

## License

MIT License — see [LICENSE](LICENSE)

---

> *"The grid of tomorrow cannot be protected by the relays of yesterday."*
