# Pulse Radar Target Detection and Range Estimation

A Python-based simulation of a basic pulse radar system for detecting multiple targets and estimating their ranges from received echo signals.

The project demonstrates the fundamental signal-processing chain of a pulse radar system, including pulse generation, echo simulation, noise addition, correlation-based detection, peak detection, and target range estimation.

## Project Overview

Radar systems determine the distance of a target by transmitting an electromagnetic signal and measuring the time delay of the returned echo.

This project simulates a simplified pulse radar system with multiple targets placed at different delays. The transmitted radar pulse is reflected by the simulated targets, Gaussian noise is added to the received signal, and cross-correlation is used to identify the echo delays.

The detected delays are then converted into target range estimates using the radar range equation:

Range = (c × Δt) / 2

where:

- c = speed of light
- Δt = round-trip signal propagation delay
- Division by 2 accounts for the two-way travel of the radar signal

## Signal Processing Flow

Transmitted Pulse
        ↓
Multiple Target Echo Simulation
        ↓
Gaussian Noise Addition
        ↓
Received Signal
        ↓
Cross-Correlation with Transmitted Pulse
        ↓
Peak Detection
        ↓
Time Delay Estimation
        ↓
Target Range Calculation

## Features

- Generation of a rectangular radar pulse
- Simulation of multiple target echoes
- Addition of Gaussian noise to simulate a noisy received signal
- Visualization of transmitted and received signals
- Cross-correlation-based echo detection
- Automatic peak detection using SciPy
- Estimation of target ranges from detected time delays
- Visualization of correlation output

## Technologies Used

- Python
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook

## Libraries

The following Python libraries are required:

```bash
pip install numpy scipy matplotlib
