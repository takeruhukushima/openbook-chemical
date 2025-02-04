[前の章: 08 Relativistic Effects in Heavy Elements](08_Relativistic_Effects_in_Heavy_Elements.md) - [次の章: 10 Summary and Future Perspectives](10_Summary_and_Future_Perspectives.md)

# Advanced Thermodynamics for Chemistry

This chapter advances the principles of thermodynamics to address complex chemical systems and phenomena. Building upon the foundational concepts introduced in Chapter 4, we explore advanced topics such as statistical thermodynamics, non-equilibrium thermodynamics, and applications of thermodynamics in chemical kinetics and materials science. This chapter aims to provide a deeper understanding of thermodynamic principles and their broad applicability in chemistry.

## 9.1 Statistical Thermodynamics

Statistical thermodynamics provides a bridge between the microscopic properties of individual molecules and the macroscopic thermodynamic properties of bulk systems. It uses statistical mechanics to derive thermodynamic quantities from molecular properties and energy distributions.

### 9.1.1 Microstates and Macrostates

- **Microstate**: A specific microscopic configuration of a system, specifying the quantum state of each molecule in the system.
- **Macrostate**: A macroscopic state of a system defined by macroscopic properties such as temperature, pressure, volume, and energy, which can be realized by many different microstates.

### 9.1.2 Boltzmann Distribution

The Boltzmann distribution describes the probability of finding a molecule in a particular energy state at a given temperature in a system at thermal equilibrium.

- **Probability of Energy State**: The probability $P_i$ of a molecule being in an energy state $E_i$ is given by $P_i = \frac{g_i e^{-E_i/kT}}{Q}$, where $g_i$ is the degeneracy of the energy level, $k$ is the Boltzmann constant, $T$ is the temperature, and $Q$ is the partition function.
- **Partition Function**: The partition function $Q = \sum_i g_i e^{-E_i/kT}$ is a measure of the number of thermally accessible states at a given temperature and is central to statistical thermodynamics.

### 9.1.3 Thermodynamic Functions from Partition Functions

Statistical thermodynamics allows us to calculate thermodynamic functions from the partition function.

- **Internal Energy**: $U = kT^2 \left(\frac{\partial \ln Q}{\partial T}\right)_V$
- **Entropy**: $S = k \ln Q + kT \left(\frac{\partial \ln Q}{\partial T}\right)_V = \frac{U}{T} + k \ln Q$
- **Helmholtz Free Energy**: $A = -kT \ln Q$
- **Gibbs Free Energy**: $G = -kT \ln Q + PV = -kT \ln Q + kT V \left(\frac{\partial \ln Q}{\partial V}\right)_T$
- **Pressure**: $P = kT \left(\frac{\partial \ln Q}{\partial V}\right)_T$

### 9.1.4 Molecular Partition Functions

The total partition function of a system can be approximated as a product of molecular partition functions for independent degrees of freedom (translational, rotational, vibrational, electronic).

- **Translational Partition Function**: $q_{trans} = \left(\frac{2\pi mkT}{h^2}\right)^{3/2} V$
- **Rotational Partition Function**: For linear molecules, $q_{rot} = \frac{T}{\sigma \Theta_{rot}}$, and for nonlinear molecules, $q_{rot} = \frac{\pi^{1/2}}{\sigma} \left(\frac{T^3}{\Theta_{rot,x} \Theta_{rot,y} \Theta_{rot,z}}\right)^{1/2}$, where $\sigma$ is the symmetry number and $\Theta_{rot}$ are rotational temperatures.
- **Vibrational Partition Function**: $q_{vib} = \frac{1}{1 - e^{-\Theta_{vib}/T}}$, where $\Theta_{vib} = \frac{h\nu}{k}$ is the vibrational temperature.
- **Electronic Partition Function**: $q_{elec} = \sum_i g_{elec,i} e^{-E_{elec,i}/kT} \approx g_{elec,0}$ at typical temperatures, where $g_{elec,0}$ is the degeneracy of the electronic ground state.

## 9.2 Non-Equilibrium Thermodynamics

Non-equilibrium thermodynamics deals with systems that are not in thermodynamic equilibrium and involve irreversible processes. It extends classical thermodynamics to describe transport phenomena and systems with fluxes of energy and matter.

### 9.2.1 Fluxes and Forces

Non-equilibrium thermodynamics describes systems in terms of fluxes ($J_i$) and thermodynamic forces ($X_i$).

- **Fluxes**: Rates of transport processes, such as heat flux, mass flux, and electric current.
- **Forces**: Gradients of thermodynamic variables that drive fluxes, such as temperature gradient, concentration gradient, and electric potential gradient.

### 9.2.2 Linear Phenomenological Laws

For systems close to equilibrium, fluxes are linearly related to thermodynamic forces through phenomenological coefficients ($L_{ij}$).

- **General Linear Law**: $J_i = \sum_j L_{ij} X_j$
- **Onsager Reciprocal Relations**: $L_{ij} = L_{ji}$, which relate cross-phenomenological coefficients and are a consequence of microscopic reversibility.

### 9.2.3 Examples of Transport Phenomena

- **Heat Conduction**: Heat flux ($J_q$) is driven by temperature gradient ($X_q = -\nabla T$), $J_q = -L_{qq} \nabla T = -\kappa \nabla T$, where $\kappa$ is thermal conductivity.
- **Diffusion**: Mass flux ($J_m$) is driven by concentration gradient ($X_m = -\nabla \mu$), $J_m = -L_{mm} \nabla \mu = -D \nabla C$, where $D$ is diffusion coefficient and $C$ is concentration.
- **Viscosity**: Momentum flux (stress) is driven by velocity gradient (shear rate).
- **Electrical Conduction**: Electric current ($J_e$) is driven by electric potential gradient ($X_e = -\nabla \phi$), $J_e = -L_{ee} \nabla \phi = -\sigma \nabla \phi$, where $\sigma$ is electrical conductivity.
- **Thermoelectric Effects**: Coupling between heat flux and electric current, such as Seebeck effect and Peltier effect.

### 9.2.4 Entropy Production in Irreversible Processes

Irreversible processes in non-equilibrium thermodynamics are associated with entropy production ($\sigma$).

- **Entropy Production Rate**: $\frac{dS}{dt} = \sum_i J_i X_i = \sigma \geq 0$
- **Local Equilibrium Hypothesis**: Non-equilibrium thermodynamics often assumes local equilibrium, where small subsystems are in local thermodynamic equilibrium even if the system as a whole is not in equilibrium.

## 9.3 Thermodynamics in Chemical Kinetics

Thermodynamics plays a crucial role in understanding and predicting the rates and equilibrium of chemical reactions.

### 9.3.1 Transition State Theory (TST)

Transition State Theory (TST) combines thermodynamics and kinetics to estimate reaction rates by considering the properties of the transition state.

- **Activated Complex**: The transition state is an activated complex at the highest energy point along the reaction coordinate.
- **Eyring Equation**: The rate constant $k$ in TST is given by $k = \frac{kT}{h} e^{-\Delta G^\ddagger/RT} = \frac{kT}{h} K^\ddagger$, where $\Delta G^\ddagger$ is the Gibbs free energy of activation, $K^\ddagger = e^{-\Delta G^\ddagger/RT}$ is the equilibrium constant for forming the activated complex, and $\frac{kT}{h}$ is the frequency factor.
- **Thermodynamic Interpretation of Activation Parameters**: $\Delta G^\ddagger = \Delta H^\ddagger - T\Delta S^\ddagger$, where $\Delta H^\ddagger$ is the enthalpy of activation and $\Delta S^\ddagger$ is the entropy of activation.

### 9.3.2 Reaction Rates and Equilibrium Constants

Thermodynamics relates reaction rates to equilibrium constants and provides insights into reaction mechanisms.

- **Relationship between $K$, $k_f$, and $k_r$**: The equilibrium constant $K$ for a reversible reaction $A \rightleftharpoons B$ is related to the forward rate constant $k_f$ and reverse rate constant $k_r$ by $K = \frac{k_f}{k_r} = e^{-\Delta G^\circ/RT}$, where $\Delta G^\circ$ is the standard Gibbs free energy change of reaction.
- **Temperature Dependence of Rate Constants**: The Arrhenius equation $k = A e^{-E_a/RT}$ and the Eyring equation show the temperature dependence of rate constants, which is related to activation energy and Gibbs free energy of activation, respectively.

### 9.3.3 Kinetic Isotope Effects

Kinetic isotope effects (KIEs) are changes in reaction rates when one atom in a reactant is replaced by its isotope. They provide mechanistic information about rate-determining steps.

- **Primary KIE**: Isotopic substitution at a bond that is broken or formed in the rate-determining step.
- **Secondary KIE**: Isotopic substitution at a bond adjacent to the reacting center.
- **Thermodynamic Origin of KIEs**: KIEs arise from changes in vibrational frequencies and zero-point energies upon isotopic substitution, which affect activation energies and reaction rates.

## 9.4 Thermodynamics in Materials Science

Thermodynamic principles are essential in materials science for understanding phase equilibria, phase transformations, and material properties.

### 9.4.1 Phase Equilibria and Phase Diagrams

Phase diagrams are graphical representations of the thermodynamic conditions (temperature, pressure, composition) under which different phases of a substance are stable in equilibrium.

- **Gibbs Phase Rule**: $F = C - P + 2$, where $F$ is the degrees of freedom, $C$ is the number of components, and $P$ is the number of phases in equilibrium.
- **Clausius-Clapeyron Equation**: $\frac{dP}{dT} = \frac{\Delta H_{phase}}{T\Delta V_{phase}}$, describes the temperature dependence of phase boundaries in a P-T phase diagram.
- **Lever Rule**: Used to determine the relative amounts of phases in a two-phase region of a phase diagram.

### 9.4.2 Phase Transformations

Phase transformations involve changes in the physical state of a material, driven by changes in thermodynamic conditions.

- **First-Order Phase Transitions**: Involve discontinuous changes in first derivatives of Gibbs free energy (e.g., volume, entropy), such as melting, boiling, and sublimation.
- **Second-Order Phase Transitions**: Involve discontinuous changes in second derivatives of Gibbs free energy (e.g., heat capacity, compressibility), such as order-disorder transitions and ferromagnetic transitions.
- **Nucleation and Growth**: Phase transformations often proceed via nucleation (formation of small nuclei of the new phase) and growth (increase in size of nuclei).

### 9.4.3 Thermodynamics of Solutions and Mixtures

Thermodynamics of solutions and mixtures describes the behavior of multicomponent systems.

- **Ideal Solutions**: Solutions that obey Raoult's law and have ideal mixing properties.
- **Non-Ideal Solutions**: Solutions that deviate from ideal behavior due to intermolecular interactions. Described by activity coefficients and excess thermodynamic functions.
- **Chemical Potential in Mixtures**: $\mu_i = \mu_i^\circ + RT \ln a_i = \mu_i^\circ + RT \ln (\gamma_i x_i)$, where $a_i$ is activity, $\gamma_i$ is activity coefficient, and $x_i$ is mole fraction of component $i$.

### 9.4.4 Applications in Materials Design

Thermodynamic principles guide the design and processing of materials with desired properties.

- **Alloy Design**: Phase diagrams and thermodynamic calculations are used to design alloys with specific phase compositions and properties.
- **Ceramic Processing**: Thermodynamics controls sintering, grain growth, and phase stability in ceramic materials.
- **Polymer Science**: Thermodynamics governs polymer solubility, phase separation, and thermal transitions in polymers.

In summary, advanced thermodynamics provides powerful tools for understanding and predicting the behavior of complex chemical systems. Statistical thermodynamics connects microscopic and macroscopic properties, non-equilibrium thermodynamics describes transport phenomena, and thermodynamics in kinetics and materials science provides frameworks for studying reaction rates, phase equilibria, and material properties. This chapter has highlighted some of the advanced applications of thermodynamics in chemistry, demonstrating its central role in modern chemical science and engineering.

## Exercises

[Exercises(.md)](exercises/ch09_exercises.md)
[Exercises(.ipynb)](exercises/ch09_exercises.ipynb)

## References

[References](references/reference_list.md)
