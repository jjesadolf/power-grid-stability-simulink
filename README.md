# Power Grid Frequency Stability - MATLAB/Simulink

This project presents a dynamic model of a power grid developed in MATLAB/Simulink to analyze frequency stability under different operating conditions.

## Model Description

The system includes:
- Nuclear unit (base-load generation)
- Steam unit with primary frequency control
- Photovoltaic (PV) generation
- Load model with disturbances

The frequency dynamics is modeled using the power balance equation:

ΔP = P_gen - P_load

## Simulated Scenarios

- Reduction of renewable generation (PV drop)
- Increase of load demand
- Combined disturbances
- Variation of system inertia (M)
- Different control gains of the steam unit

## Key Results

- Higher renewable penetration increases frequency sensitivity
- Lower inertia leads to faster and deeper frequency drops
- Steam unit is essential for primary frequency regulation
- Nuclear unit provides system stability but reacts slowly

## Tools

- MATLAB
- Simulink

Jesus Adolfo Rossi



