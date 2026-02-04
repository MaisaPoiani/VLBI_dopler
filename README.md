# Radio Science Studies with TudatPy

This repository contains a progressive set of Jupyter Notebooks dedicated to studying radio science applications using TudatPy, with emphasis on techniques related to PRIDE (Planetary Radio Interferometry and Doppler Experiment).

The notebooks were developed sequentially. Each notebook extends and consolidates concepts introduced in the previous ones, progressively building a complete simulation and analysis pipeline for spacecraft tracking and radio interferometry scenarios.

## Environment Setup
This repository contains only the notebooks.
Before running them, you must install the Tudat environment.

Use the following commands:
        conda env create -f environment.yaml
        conda activate tudat-space
        
Make sure the environment is correctly activated before executing any notebook.

## Notebook Overview

### 01_environment_and_basic_orbit_propagation.ipynb

This notebook introduces the fundamental setup of the simulation environment using TudatPy. It covers:

- Loading SPICE kernels
- Creating celestial bodies and custom spacecraft
- Defining spacecraft physical properties
- Setting up force models (gravitational and non-gravitational)
- Performing basic orbit propagation

This notebook establishes the baseline dynamical model used throughout the repository.

### 02_observables_modeling.ipynb

This notebook expands the simulation by introducing radio science observables. It includes:

- Modeling tracking observables relevant to radio interferometry
- Simulation of Doppler and angular position measurements
- Configuration of ground station networks
- Light-time and signal propagation modeling

The notebook focuses on how spacecraft states are converted into measurable quantities used in radio science.

### 03_parameter_estimation.ipynb

This notebook introduces orbit determination and parameter estimation techniques. It explores:

- Construction of estimation parameter sets
- Least-squares orbit determination
- Residual analysis and convergence behavior

This stage demonstrates how simulated observations can be used to recover spacecraft dynamical parameters.

### 04_Sensitivity_Analysis.ipynb

This notebook focuses on statistical and sensitivity analysis of the estimation process. It includes:

- Covariance analysis
- Error propagation studies
- Simulation of noisy observational data
- Evaluation of parameter correlations
- Performance comparison across different simulation scenarios

The goal is to quantify the reliability and robustness of the estimation pipeline.

### 05_RadioScienceApplications.ipynb

This notebook explores advanced radio science applications inspired by PRIDE methodologies. Topics include:

- Multi-station radio interferometry scenarios
- Assessment of observational geometry effects
- Evaluation of tracking precision improvements
- Investigation of observational network configurations

This stage connects the technical framework to realistic radio science mission scenarios.

### 06_Occultation_Spacecraft.ipynb

This notebook introduces a predictive analysis of spacecraft visibility. It presents:

- Development of a function that predicts spacecraft occultations
- Determination of time intervals where the spacecraft becomes unobservable by radio interferometry
- Geometrical and dynamical interpretation of occultation events
- Acessible return of scientific data

This application is particularly relevant for mission planning and data availability forecasting.

## Research Scope

Throughout this repository, the study progressively explores:

- Creation of custom spacecraft dynamical models
- Orbit propagation under realistic perturbations
- Modeling of radio interferometric observables
- Statistical and covariance-based analysis
- Predictive modeling of observational limitations

# Ongoing Development

New studies, simulations, and extensions related to radio science and spacecraft tracking are continuously being developed and added to this repository.
