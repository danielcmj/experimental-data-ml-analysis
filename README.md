# Simulation & Experimental Signal Analysis  
**Physics-based modeling of magnetic particle detection in microfluidic sensors**

## Overview
This repository contains a physics-driven analysis pipeline for studying how superparamagnetic particles are detected by magnetoresistive sensors in a microfluidic cytometer.

The project combines:
- experimental signal processing,
- analytical physical modeling,
- parameter estimation via curve fitting,

to extract physically meaningful quantities from raw voltage signals measured during particle flow experiments.

The emphasis is on interpretable models rather than black-box machine learning.

---

## What problem does this solve?
In magnetic cytometry, particles flowing over a sensor produce voltage peaks whose shape and amplitude depend on multiple coupled effects:
- particle velocity,
- particle height in the microfluidic channel,
- magnetic moment orientation,
- possible overlap of multiple particles.

This project provides a structured approach to:
- convert time-domain signals into spatial coordinates,
- model the magnetic and electrical response of the sensor,
- fit experimental peaks using physics-based equations,
- objectively compare single-particle and multi-particle events.

---

## Project structure
```text
.
├── data/
│   ├── *.txt            # raw experimental cytometer data
│   └── *.pkl            # cached dataframes for faster loading
│
├── figures/             # generated plots (optional)
├── Simulation_Experimental_Signal_Analysis.ipynb
├── requirements.txt
└── README.md
