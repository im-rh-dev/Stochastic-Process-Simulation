# Stochastic-Process-Simulation
## Introduction
This repository contains the implementation of simulations for various stochastic processes, including Homogeneous Poisson Process (HPP), Inhomogeneous Poisson Process (NHPP), and Renewal Processes, as part of a project in Statistics and Econometrics for Actuarial Science. The project, authored by Imene Rahal and Asma Beghoura, focuses on simulating these processes and applying them to real-world datasets, such as hospital admission data and insurance claim data, to analyze patterns and predict outcomes.

The code is written in Python and includes detailed simulations, visualizations, and analyses. The accompanying Jupyter Notebooks provides additional interpretations and interactive visualizations.

## Features
- **Simulation of Stochastic Processes**:
  - **Homogeneous Poisson Process (HPP)**: Simulates events with a constant rate (λ) and compares empirical vs. theoretical means.
  - **Inhomogeneous Poisson Process (NHPP)**: Models time-varying rates using direct simulation (Bernoulli trials) and the thinning method.
  - **Renewal Process**: Simulates events with various inter-arrival time distributions (e.g., exponential, uniform, normal, gamma, Weibull) using direct sampling and Acceptance-Rejection Sampling for complex distributions.
- **Exploratory Data Analysis (EDA)**:
  - Visualizes event paths, inter-arrival time histograms, raster plots, and joyplots for process trajectories.
  - Compares empirical and theoretical metrics (e.g., mean event counts, inter-arrival times).
- **Real-World Applications**:
  - Analyzes hospital admission data (2018) to model patient arrivals using HPP and NHPP.
  - Analyzes insurance claim data to model inter-arrival times using a fitted exponential distribution.
- **Validation**: Verifies simulation results against theoretical expectations (e.g., Strong Law of Large Numbers, exponential distribution for inter-arrival times).
- **Visualization**: Uses Matplotlib, Seaborn, and Plotly for histograms, step functions, raster plots, joyplots, and empirical vs. theoretical comparisons.

## Datasets
1. **Hospital Admission Data (2018)**:
   - Contains weekly admission counts for 2018.
   - Used to simulate and compare HPP and NHPP models against actual admission patterns.
   - Objective: Determine if admissions follow a homogeneous or non-homogeneous process and predict resource utilization.

2. **Insurance Claim Data**:
   - Contains policy bind dates to calculate inter-arrival times between claims.
   - Objective: Fit distributions (e.g., exponential, Weibull, Gamma) to inter-arrival times and simulate synthetic claims for comparison with real data.

*Note*: The datasets are not included in the repository due to their proprietary nature. Users must provide their own data files (`hospital_admissions_2018.csv` and `insurance_claims.csv`) or adapt the code to their datasets.

## Installation
To run the simulations, install the required Python dependencies. The code uses standard Python libraries and does not require external packages beyond those listed.

### Prerequisites
- Python 3.8+
- Required libraries:
  ```bash
  pip install numpy pandas matplotlib seaborn plotly scipy
