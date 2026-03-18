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

## Observations
Here is your text translated into clear, technical English suitable for a thesis:

---

The evolution of modern power systems is strongly influenced by the increasing integration of non-dispatchable renewable energy sources, such as photovoltaic generation, which introduce variability and reduce the overall system inertia. In this context, frequency stability becomes a central issue, since the instantaneous balance between generated power and consumed power must be maintained to ensure proper system operation. In this work, a simplified dynamic model has been developed in the MATLAB/Simulink environment, aimed at describing the frequency behavior of a power system composed of three types of generation units: a nuclear unit, representing base-load generation, a steam thermal unit with regulating function, and a photovoltaic renewable source characterized by variability and lack of inertia.

The model is based on the dynamic frequency equation, in which the time variation of the frequency deviation is proportional to the power imbalance between generation and load, taking into account a damping term and the equivalent inertia of the system. In particular, the dynamics are expressed as a relationship between the derivative of the frequency deviation, the inertia parameter, and the difference between generated and absorbed power. This formulation makes it possible to describe the transient behavior of the system following disturbances, highlighting the role of the different components in stabilizing the grid.

The system is initialized in an equilibrium condition by imposing equality between total generated power and total load demand. Under this configuration, the frequency remains constant at its nominal value, and the frequency deviation is zero. The nuclear generation is modeled as a quasi-constant source, with very slow dynamics and limited regulation capability, reflecting its real role as base-load generation. The thermal unit is instead equipped with a proportional control based on frequency deviation, capable of increasing or decreasing its output power in response to frequency variations, representing primary frequency control. The photovoltaic source is modeled as a variable, non-controllable input subject to external disturbances.

The simulations carried out allow the analysis of several operating scenarios. In the case of a sudden reduction in photovoltaic power, an immediate decrease in total generation is observed, resulting in a negative power imbalance and thus a drop in frequency. The system response is characterized by the intervention of the thermal unit, which gradually increases its output power, contributing to reducing the imbalance. However, in the absence of secondary control, the frequency does not return to its nominal value but stabilizes at a lower level, highlighting the intrinsic limitation of primary regulation.

A similar behavior is observed in the case of a load increase, where the rise in demand generates a power deficit that causes a frequency drop. Also in this case, the regulating unit intervenes to compensate for the imbalance, but it is not able to fully eliminate it. When both disturbances—reduction in renewable generation and increase in load—are applied simultaneously, the system exhibits a more critical response, with a larger frequency deviation and greater stress on the regulating units, which may approach their operational limits.

A particularly relevant aspect emerging from the simulations is the role of system inertia. By reducing the inertia parameter, which represents the kinetic energy stored in the rotating masses of synchronous generators, a faster but less stable response is observed, with deeper frequency drops and shorter variation times. This behavior accurately reflects what occurs in modern power systems with high renewable penetration, where the replacement of synchronous machines with power-electronic-based sources leads to a significant reduction in inertia. Conversely, high inertia contributes to damping frequency variations, making the system more robust but less responsive.

Further analyses highlight the importance of the control parameter of the thermal unit. A high control gain enables a faster response and better compensation of the imbalance but may introduce overshoot phenomena and increase sensitivity to oscillations. On the other hand, a low gain results in a slower response and larger frequency deviations. Therefore, an optimal trade-off between responsiveness and system stability is required.

Finally, increasing the penetration of renewable sources, simulated by raising the share of photovoltaic power, shows how the system becomes progressively more sensitive to disturbances. Under these conditions, even relatively small variations in generation can produce significant frequency deviations, due to reduced inertia and limited immediate regulation capability.

Overall, the developed model is able to qualitatively reproduce the main phenomena related to frequency stability in modern power systems. The results clearly highlight how the massive integration of renewables requires the introduction of new control and stability-support tools, such as energy storage systems, secondary control, and synthetic inertia resources. This work therefore represents a solid foundation for further developments, which could include more detailed component modeling, multi-node network structures, and the analysis of advanced control strategies.



