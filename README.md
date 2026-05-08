# Coherence limitations of a Fourier-engineered cos(2φ) transmon qubit

The paper that this repository pertains to can be found here: [https://arxiv.org/abs/2605.06372].

## Files in this repository

This repository includes all scripts and notebooks used for simulation, analysis, and visualization.

Two notebooks are dedicated to data fitting and calibration:

`Fitting_transitions.ipynb`
This notebook is used to fit the simulated qubit spectrum to experimental measurements. It enables extraction of key system parameters by aligning theoretical transition frequencies with measured data.

`Crosstalk_calibration.ipynb`
This notebook performs cross-talk calibration based on raw experimental measurements. It computes a rotation matrix used to compensate for unwanted cross-talk.

## General Workflow for the files

The other notebooks in the repository are generating the figures for the paper and follow the workflow below:

### Definition of constants and calibration parameters
Experimental constants, device parameters, and calibration values are initialized.

### Data loading and preprocessing
Input data files are imported, cleaned, formatted, and transformed into structures suitable for numerical analysis.

### Model(Hamiltonian) construction
The physical model describing the system is constructed using the defined parameters.

### Calculation of the corresponding physical quantities or functions
Relevant quantities are calculated from the defined model and parameters. Depending on the specific file, this may include:
 - transition frequencies,
 - resonator shift,
 - matrix elements,
 - spectral properties,
  or other derived observables.

### Visualization and plotting
Custom plotting functions generate publication-quality figures for analysis and comparison.

### Parameter fitting and optimization
Experimental and simulated results can be compared through fitting procedures to extract effective model parameters.

## Input Requirements
The notebook is working with external data and parameter files. In general, users should provide:
 - calibrated system parameters,
 - experimental measurement data,
 - device-specific constants,
 - and optional fitting constraints.

## Output
Typical outputs include:
 - processed datasets, 
 - fitted model parameters,
 - and publication-ready plots.

## Author & Contact
Nataliia Zhurbina \
nkzhurbina@gmail.com
