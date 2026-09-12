# Plastic Scintillator–SiPM Detector Module for PET Imaging

Geant4 Monte Carlo simulation and optimization of a plastic scintillator–SiPM based detector module for Positron Emission Tomography (PET) imaging.

## Overview

This project investigates the feasibility of using plastic scintillators as a lower-cost alternative to conventional inorganic scintillators in PET detector systems.

The detector is modeled and studied using the **Geant4 Monte Carlo simulation toolkit**, with emphasis on gamma-ray interactions, energy deposition, scintillation light production, optical photon transport, SiPM detection, and spatial resolution.

The project also investigates the effect of optical coupling and light-guide thickness on detector performance.

## Research Objectives

- Design a plastic scintillator–SiPM detector module using Geant4.
- Simulate gamma-ray interactions and energy deposition in the scintillator.
- Model scintillation and optical photon transport.
- Investigate reflective coating effects using ESR.
- Study optical coupling between the scintillator, light guide, and SiPM.
- Optimize light-guide thickness.
- Analyze detector spatial response and intrinsic spatial resolution.
- Evaluate detector performance using ROOT-based data analysis.

## Detector Concept

The simulated detector consists of:

**Plastic Scintillator → Optical Coupling → Light Guide → SiPM**

The scintillator surfaces are modeled with a reflective ESR coating to improve optical photon collection.

## Simulation Framework

### Software

- **Geant4** — Monte Carlo particle transport simulation
- **C++** — Detector construction and simulation
- **ROOT** — Data analysis and visualization
- **Python** — Scientific computing and analysis
- **LaTeX** — Scientific documentation

### Physics Processes

The simulation includes the study of:

- Gamma-ray interactions
- Compton scattering
- Energy deposition
- Scintillation
- Optical photon transport
- Optical reflection
- SiPM photon detection
- Coincidence detection
- Spatial response

## Detector Optimization

The study investigates the influence of optical and detector parameters including:

- ESR reflectivity
- Light-guide thickness
- Optical coupling
- Detector geometry
- SiPM response

Different detector configurations are simulated and compared to determine their influence on spatial resolution and photon collection.

## Data Analysis

Simulation output is analyzed using ROOT.

The analysis includes:

- Energy spectra
- Energy deposition distributions
- Spatial distributions
- Histograms
- Gaussian fitting
- Standard deviation analysis
- FWHM calculation
- Comparison of detector configurations

Spatial resolution is evaluated using:

\[
\mathrm{FWHM} = 2.355\sigma
\]

where \( \sigma \) is the standard deviation obtained from the spatial response distribution.

## Results

The simulations show that the measured spatial response depends on the optical configuration of the detector.

In the studied configurations, increasing the light-guide thickness generally increases the measured spatial spread. The best spatial-resolution result in the current study was obtained for the configuration without a light guide, using the plastic-scintillator Compton response.

Further analysis and optimization are ongoing.

## Repository Structure

```text
plastic-scintillator-sipm-pet-geant4/
│
├── README.md
├── LICENSE
├── .gitignore
│
├── src/
│   └── Geant4 source files
│
├── include/
│   └── Geant4 header files
│
├── macros/
│   └── Geant4 macro files
│
├── analysis/
│   ├── ROOT/
│   └── Python/
│
├── geometry/
│   └── Detector geometry and configuration files
│
├── results/
│   ├── energy_spectra/
│   ├── spatial_resolution/
│   └── figures/
│
└── docs/
    ├── detector_design/
    └── methodology/
