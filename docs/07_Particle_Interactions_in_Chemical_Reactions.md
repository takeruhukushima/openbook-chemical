[前の章: 06 Quantum Chemistry Basics](06_Quantum_Chemistry_Basics.md) - [次の章: 08 Relativistic Effects in Heavy Elements](08_Relativistic_Effects_in_Heavy_Elements.md)


# Particle Interactions in Chemical Reactions

This chapter explores the fundamental interactions between particles that drive chemical reactions. Chemical reactions involve the rearrangement of atoms and molecules, which are governed by the interactions between electrons and nuclei. Understanding these interactions at the particle level is crucial for predicting reaction rates, mechanisms, and outcomes. This chapter covers the basic types of particle interactions, potential energy surfaces, and reaction dynamics.

## 7.1 Types of Particle Interactions

Chemical reactions are driven by fundamental interactions between particles, primarily electromagnetic interactions. These interactions can be categorized into several types based on their nature and range.

### 7.1.1 Electromagnetic Interactions

Electromagnetic interactions are responsible for the forces between charged particles (electrons and nuclei). These interactions are long-range and govern the formation of chemical bonds and the dynamics of chemical reactions.

- **Coulomb Interaction**: The electrostatic force between charged particles, described by Coulomb's law. For two charges $q_1$ and $q_2$ separated by a distance $r$, the potential energy is $V(r) = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r}$.
- **Exchange Interaction**: A quantum mechanical effect arising from the Pauli exclusion principle, which affects the energy of electron-electron interactions. Exchange interactions are crucial for chemical bonding and magnetism.
- **Dipole-Dipole Interaction**: Interactions between molecules with permanent dipole moments. These interactions are weaker than Coulomb interactions but play a significant role in intermolecular forces and condensed phases.
- **Dispersion (London) Forces**: Weak, short-range attractive forces arising from instantaneous fluctuations in electron distributions, leading to temporary dipoles. Dispersion forces are important for nonpolar molecules and contribute to van der Waals forces.

### 7.1.2 Strong Nuclear Force

The strong nuclear force is one of the fundamental forces of nature, responsible for binding protons and neutrons together in the atomic nucleus. Although it is the strongest force, it is very short-range and does not directly play a role in chemical reactions under normal conditions. However, in nuclear chemistry and reactions involving nuclear transformations, the strong force is dominant.

### 7.1.3 Weak Nuclear Force

The weak nuclear force is another fundamental force involved in radioactive decay and certain types of particle interactions. Like the strong force, it is short-range and does not directly influence typical chemical reactions. However, it is important in nuclear processes and particle physics.

### 7.1.4 Gravitational Force

Gravitational force is the weakest of the four fundamental forces and is significant only for macroscopic objects with large masses. At the atomic and molecular level, gravitational forces are negligible compared to electromagnetic interactions and do not play a role in chemical reactions.

## 7.2 Potential Energy Surfaces (PES)

Potential Energy Surfaces (PES) are central to understanding chemical reactions. A PES is a mathematical representation of the potential energy of a molecular system as a function of its geometry (nuclear coordinates). It provides a landscape on which chemical reactions occur.

### 7.2.1 Dimensions of PES

For a system with $N$ atoms, the PES is a function of $3N-6$ internal coordinates (or $3N-5$ for linear molecules). These coordinates can be bond lengths, bond angles, and dihedral angles. Visualizing PES is typically done for systems with a few degrees of freedom (e.g., diatomic or triatomic molecules).

### 7.2.2 Features of PES

Key features of a PES include:

- **Reactant Valley**: Regions of the PES corresponding to reactant molecules. These are typically local minima.
- **Product Valley**: Regions of the PES corresponding to product molecules. These are also local minima.
- **Transition State (Saddle Point)**: A point on the PES that is a maximum along the reaction coordinate and a minimum in all other directions. The transition state represents the highest energy point along the minimum energy path from reactants to products.
- **Reaction Path (Minimum Energy Path, MEP)**: The path of lowest energy connecting reactants to products through the transition state.
- **Activation Energy ($E_a$)**: The energy barrier for a reaction, defined as the energy difference between the transition state and the reactants.
- **Intermediates**: Stable or metastable species that exist in local minima along the reaction path between reactants and products.

### 7.2.3 Constructing PES

PES can be constructed using quantum chemical calculations. Methods for calculating PES include:

- **Ab initio methods**: High-level quantum mechanical methods (e.g., Coupled Cluster, Configuration Interaction) that provide accurate PES but are computationally expensive for large systems.
- **Density Functional Theory (DFT)**: A more computationally efficient method that can provide reasonably accurate PES for many systems.
- **Semiempirical methods**: Approximate quantum mechanical methods that use empirical parameters to reduce computational cost.
- **Molecular Mechanics (MM)**: Classical force field methods that are computationally very fast but less accurate and not suitable for describing bond breaking and formation.

## 7.3 Reaction Dynamics

Reaction dynamics studies the motion of nuclei and electrons during a chemical reaction. It aims to understand how reactions occur at the molecular level, including the pathways, rates, and energy flow.

### 7.3.1 Classical Trajectory Calculations

Classical trajectory calculations simulate the motion of nuclei on the PES using classical mechanics. These calculations can provide insights into reaction mechanisms and dynamics, particularly for reactions involving heavy atoms at high temperatures.

- **Equations of Motion**: Nuclei are treated as classical particles moving according to Newton's equations of motion.
- **Initial Conditions**: Initial positions and momenta of reactants are chosen based on statistical distributions (e.g., Boltzmann distribution).
- **Trajectory Propagation**: Equations of motion are integrated numerically to follow the trajectories of reactants as they move towards products.
- **Limitations**: Classical trajectory calculations neglect quantum effects such as tunneling, zero-point energy, and quantum interference.

### 7.3.2 Transition State Theory (TST)

Transition State Theory (TST) is a statistical theory that provides a framework for calculating reaction rates based on the properties of the transition state. TST assumes that:

- **Transition State**: There exists a well-defined transition state along the reaction path.
- **Equilibrium**: Reactants are in equilibrium with the transition state.
- **No Recrossing**: Trajectories that cross the transition state from reactants to products do not recross back to reactants.

The TST rate constant is given by:

$$ k_{TST} = \frac{k_B T}{h} \frac{Q_{TS}}{Q_R} e^{-E_a/k_B T} $$

where $k_B$ is the Boltzmann constant, $T$ is temperature, $h$ is Planck's constant, $Q_{TS}$ and $Q_R$ are partition functions for the transition state and reactants, and $E_a$ is the activation energy.

### 7.3.3 Quantum Reaction Dynamics

Quantum reaction dynamics methods treat nuclear motion quantum mechanically. These methods are necessary for describing reactions involving light atoms (e.g., hydrogen) and low temperatures, where quantum effects are significant.

- **Time-Dependent Quantum Mechanics**: Wave packet propagation methods solve the time-dependent Schrödinger equation to describe the evolution of reactant wave packets as they move towards products.
- **Time-Independent Quantum Mechanics**: Scattering theory methods solve the time-independent Schrödinger equation to calculate scattering matrices and reaction probabilities as a function of energy.
- **Quantum Tunneling**: A quantum mechanical phenomenon where particles can pass through potential energy barriers even if they do not have enough classical energy to overcome the barrier. Tunneling is important for reactions involving light atoms and low temperatures.
- **Zero-Point Energy (ZPE)**: The minimum vibrational energy of a molecule in its ground vibrational state. ZPE can affect activation energies and reaction rates, especially for reactions involving isotopic substitution.

## 7.4 Reactive Intermediates

Reactive intermediates are short-lived, high-energy species formed during chemical reactions. They are not reactants or products but play a crucial role in reaction mechanisms.

### 7.4.1 Types of Reactive Intermediates

Common types of reactive intermediates include:

- **Carbocations**: Positively charged carbon ions (e.g., $CH_3^+$). They are electrophilic and prone to reactions with nucleophiles.
- **Carbanions**: Negatively charged carbon ions (e.g., $CH_3^-$). They are nucleophilic and react with electrophiles.
- **Free Radicals**: Species with unpaired electrons (e.g., $CH_3^\bullet$). They are highly reactive and involved in chain reactions.
- **Carbenes**: Neutral species with divalent carbon atoms and two nonbonding electrons (e.g., $:CH_2$). They are highly versatile intermediates in organic synthesis.
- **Arynes**: Unsaturated cyclic hydrocarbons with a triple bond in the ring (e.g., benzyne). They are highly reactive and undergo cycloaddition reactions.

### 7.4.2 Detection and Characterization of Intermediates

Reactive intermediates are often short-lived and difficult to isolate. Spectroscopic techniques and trapping experiments are used to detect and characterize them.

- **Spectroscopic Methods**: Techniques like UV-Vis spectroscopy, IR spectroscopy, EPR spectroscopy, and NMR spectroscopy can be used to detect and study reactive intermediates in situ, especially in matrix isolation or flash photolysis experiments.
- **Trapping Experiments**: Reactive intermediates can be trapped by reacting them with trapping agents to form stable products that can be identified. For example, free radicals can be trapped by reacting with stable radicals like nitric oxide (NO).

### 7.4.3 Role of Intermediates in Reaction Mechanisms

Reactive intermediates are key components of reaction mechanisms. Understanding the formation, structure, and reactivity of intermediates is essential for elucidating reaction pathways and designing new chemical reactions. Reaction mechanisms often involve a series of elementary steps, each involving one or more reactive intermediates.

## 7.5 Reaction Mechanisms

A reaction mechanism is a step-by-step sequence of elementary reactions that describe the overall chemical transformation. It provides a detailed picture of how reactants are converted into products at the molecular level.

### 7.5.1 Elementary Reactions

Elementary reactions are single-step reactions that occur in one step without any intermediates. Examples include unimolecular reactions (e.g., isomerization, dissociation) and bimolecular reactions (e.g., $S_N2$ reactions, cycloadditions).

### 7.5.2 Types of Reaction Mechanisms

Common types of reaction mechanisms include:

- **Addition Reactions**: Two or more reactants combine to form a single product (e.g., addition of $H_2$ to alkenes).
- **Elimination Reactions**: A molecule loses atoms or groups to form a smaller molecule, often with the formation of multiple bonds (e.g., dehydration of alcohols).
- **Substitution Reactions**: One atom or group in a molecule is replaced by another atom or group (e.g., $S_N1$ and $S_N2$ reactions).
- **Rearrangement Reactions**: Atoms or groups within a molecule are rearranged to form an isomer (e.g., Claisen rearrangement).
- **Redox Reactions**: Reactions involving the transfer of electrons between reactants, resulting in changes in oxidation states (e.g., combustion, electrochemical reactions).
- **Chain Reactions**: Reactions involving a series of steps, including initiation, propagation, and termination steps. Free radical reactions are often chain reactions (e.g., radical polymerization).
- **Catalytic Reactions**: Reactions accelerated by catalysts, which are substances that participate in the reaction mechanism but are regenerated at the end (e.g., enzyme catalysis, heterogeneous catalysis).

### 7.5.3 Determining Reaction Mechanisms

Determining reaction mechanisms involves experimental and computational methods.

- **Experimental Methods**: Kinetic studies, product analysis, stereochemical studies, isotopic labeling, and spectroscopic detection of intermediates are used to probe reaction mechanisms.
- **Computational Methods**: Quantum chemical calculations, PES analysis, and reaction dynamics simulations are used to model reaction mechanisms and predict reaction pathways.

Understanding reaction mechanisms is crucial for controlling chemical reactions, optimizing reaction conditions, and designing new synthetic strategies. It is a central theme in chemistry, bridging fundamental principles with practical applications.

In summary, particle interactions drive chemical reactions, and understanding these interactions, potential energy surfaces, reaction dynamics, reactive intermediates, and reaction mechanisms is essential for comprehending and predicting chemical reactivity. This chapter provides a foundation for further exploration into advanced topics in chemical kinetics and reaction engineering.



# Particle Interactions in Chemical Reactions

This chapter explores the fundamental interactions between particles that drive chemical reactions. Chemical reactions involve the rearrangement of atoms and molecules, which are governed by the interactions between electrons and nuclei. Understanding these interactions at the particle level is crucial for predicting reaction rates, mechanisms, and outcomes. This chapter covers the basic types of particle interactions, potential energy surfaces, and reaction dynamics.

## 7.1 Types of Particle Interactions

Chemical reactions are driven by fundamental interactions between particles, primarily electromagnetic interactions. These interactions can be categorized into several types based on their nature and range.

### 7.1.1 Electromagnetic Interactions

Electromagnetic interactions are responsible for the forces between charged particles (electrons and nuclei). These interactions are long-range and govern the formation of chemical bonds and the dynamics of chemical reactions.

- **Coulomb Interaction**: The electrostatic force between charged particles, described by Coulomb's law. For two charges $q_1$ and $q_2$ separated by a distance $r$, the potential energy is $V(r) = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r}$.
- **Exchange Interaction**: A quantum mechanical effect arising from the Pauli exclusion principle, which affects the energy of electron-electron interactions. Exchange interactions are crucial for chemical bonding and magnetism.
- **Dipole-Dipole Interaction**: Interactions between molecules with permanent dipole moments. These interactions are weaker than Coulomb interactions but play a significant role in intermolecular forces and condensed phases.
- **Dispersion (London) Forces**: Weak, short-range attractive forces arising from instantaneous fluctuations in electron distributions, leading to temporary dipoles. Dispersion forces are important for nonpolar molecules and contribute to van der Waals forces.

### 7.1.2 Strong Nuclear Force

The strong nuclear force is one of the fundamental forces of nature, responsible for binding protons and neutrons together in the atomic nucleus. Although it is the strongest force, it is very short-range and does not directly play a role in chemical reactions under normal conditions. However, in nuclear chemistry and reactions involving nuclear transformations, the strong force is dominant.

### 7.1.3 Weak Nuclear Force

The weak nuclear force is another fundamental force involved in radioactive decay and certain types of particle interactions. Like the strong force, it is short-range and does not directly influence typical chemical reactions. However, it is important in nuclear processes and particle physics.

### 7.1.4 Gravitational Force

Gravitational force is the weakest of the four fundamental forces and is significant only for macroscopic objects with large masses. At the atomic and molecular level, gravitational forces are negligible compared to electromagnetic interactions and do not play a role in chemical reactions.

## 7.2 Potential Energy Surfaces (PES)

Potential Energy Surfaces (PES) are central to understanding chemical reactions. A PES is a mathematical representation of the potential energy of a molecular system as a function of its geometry (nuclear coordinates). It provides a landscape on which chemical reactions occur.

### 7.2.1 Dimensions of PES

For a system with $N$ atoms, the PES is a function of $3N-6$ internal coordinates (or $3N-5$ for linear molecules). These coordinates can be bond lengths, bond angles, and dihedral angles. Visualizing PES is typically done for systems with a few degrees of freedom (e.g., diatomic or triatomic molecules).

### 7.2.2 Features of PES

Key features of a PES include:

- **Reactant Valley**: Regions of the PES corresponding to reactant molecules. These are typically local minima.
- **Product Valley**: Regions of the PES corresponding to product molecules. These are also local minima.
- **Transition State (Saddle Point)**: A point on the PES that is a maximum along the reaction coordinate and a minimum in all other directions. The transition state represents the highest energy point along the minimum energy path from reactants to products.
- **Reaction Path (Minimum Energy Path, MEP)**: The path of lowest energy connecting reactants to products through the transition state.
- **Activation Energy ($E_a$)**: The energy barrier for a reaction, defined as the energy difference between the transition state and the reactants.
- **Intermediates**: Stable or metastable species that exist in local minima along the reaction path between reactants and products.

### 7.2.3 Constructing PES

PES can be constructed using quantum chemical calculations. Methods for calculating PES include:

- **Ab initio methods**: High-level quantum mechanical methods (e.g., Coupled Cluster, Configuration Interaction) that provide accurate PES but are computationally expensive for large systems.
- **Density Functional Theory (DFT)**: A more computationally efficient method that can provide reasonably accurate PES for many systems.
- **Semiempirical methods**: Approximate quantum mechanical methods that use empirical parameters to reduce computational cost.
- **Molecular Mechanics (MM)**: Classical force field methods that are computationally very fast but less accurate and not suitable for describing bond breaking and formation.

## 7.3 Reaction Dynamics

Reaction dynamics studies the motion of nuclei and electrons during a chemical reaction. It aims to understand how reactions occur at the molecular level, including the pathways, rates, and energy flow.

### 7.3.1 Classical Trajectory Calculations

Classical trajectory calculations simulate the motion of nuclei on the PES using classical mechanics. These calculations can provide insights into reaction mechanisms and dynamics, particularly for reactions involving heavy atoms at high temperatures.

- **Equations of Motion**: Nuclei are treated as classical particles moving according to Newton's equations of motion.
- **Initial Conditions**: Initial positions and momenta of reactants are chosen based on statistical distributions (e.g., Boltzmann distribution).
- **Trajectory Propagation**: Equations of motion are integrated numerically to follow the trajectories of reactants as they move towards products.
- **Limitations**: Classical trajectory calculations neglect quantum effects such as tunneling, zero-point energy, and quantum interference.

### 7.3.2 Transition State Theory (TST)

Transition State Theory (TST) is a statistical theory that provides a framework for calculating reaction rates based on the properties of the transition state. TST assumes that:

- **Transition State**: There exists a well-defined transition state along the reaction path.
- **Equilibrium**: Reactants are in equilibrium with the transition state.
- **No Recrossing**: Trajectories that cross the transition state from reactants to products do not recross back to reactants.

The TST rate constant is given by:

$$ k_{TST} = \frac{k_B T}{h} \frac{Q_{TS}}{Q_R} e^{-E_a/k_B T} $$

where $k_B$ is the Boltzmann constant, $T$ is temperature, $h$ is Planck's constant, $Q_{TS}$ and $Q_R$ are partition functions for the transition state and reactants, and $E_a$ is the activation energy.

### 7.3.3 Quantum Reaction Dynamics

Quantum reaction dynamics methods treat nuclear motion quantum mechanically. These methods are necessary for describing reactions involving light atoms (e.g., hydrogen) and low temperatures, where quantum effects are significant.

- **Time-Dependent Quantum Mechanics**: Wave packet propagation methods solve the time-dependent Schrödinger equation to describe the evolution of reactant wave packets as they move towards products.
- **Time-Independent Quantum Mechanics**: Scattering theory methods solve the time-independent Schrödinger equation to calculate scattering matrices and reaction probabilities as a function of energy.
- **Quantum Tunneling**: A quantum mechanical phenomenon where particles can pass through potential energy barriers even if they do not have enough classical energy to overcome the barrier. Tunneling is important for reactions involving light atoms and low temperatures.
- **Zero-Point Energy (ZPE)**: The minimum vibrational energy of a molecule in its ground vibrational state. ZPE can affect activation energies and reaction rates, especially for reactions involving isotopic substitution.

## 7.4 Reactive Intermediates

Reactive intermediates are short-lived, high-energy species formed during chemical reactions. They are not reactants or products but play a crucial role in reaction mechanisms.

### 7.4.1 Types of Reactive Intermediates

Common types of reactive intermediates include:

- **Carbocations**: Positively charged carbon ions (e.g., $CH_3^+$). They are electrophilic and prone to reactions with nucleophiles.
- **Carbanions**: Negatively charged carbon ions (e.g., $CH_3^-$). They are nucleophilic and react with electrophiles.
- **Free Radicals**: Species with unpaired electrons (e.g., $CH_3^\bullet$). They are highly reactive and involved in chain reactions.
- **Carbenes**: Neutral species with divalent carbon atoms and two nonbonding electrons (e.g., $:CH_2$). They are highly versatile intermediates in organic synthesis.
- **Arynes**: Unsaturated cyclic hydrocarbons with a triple bond in the ring (e.g., benzyne). They are highly reactive and undergo cycloaddition reactions.

### 7.4.2 Detection and Characterization of Intermediates

Reactive intermediates are often short-lived and difficult to isolate. Spectroscopic techniques and trapping experiments are used to detect and characterize them.

- **Spectroscopic Methods**: Techniques like UV-Vis spectroscopy, IR spectroscopy, EPR spectroscopy, and NMR spectroscopy can be used to detect and study reactive intermediates in situ, especially in matrix isolation or flash photolysis experiments.
- **Trapping Experiments**: Reactive intermediates can be trapped by reacting them with trapping agents to form stable products that can be identified. For example, free radicals can be trapped by reacting with stable radicals like nitric oxide (NO).

### 7.4.3 Role of Intermediates in Reaction Mechanisms

Reactive intermediates are key components of reaction mechanisms. Understanding the formation, structure, and reactivity of intermediates is essential for elucidating reaction pathways and designing new chemical reactions. Reaction mechanisms often involve a series of elementary steps, each involving one or more reactive intermediates.

## 7.5 Reaction Mechanisms

A reaction mechanism is a step-by-step sequence of elementary reactions that describe the overall chemical transformation. It provides a detailed picture of how reactants are converted into products at the molecular level.

### 7.5.1 Elementary Reactions

Elementary reactions are single-step reactions that occur in one step without any intermediates. Examples include unimolecular reactions (e.g., isomerization, dissociation) and bimolecular reactions (e.g., $S_N2$ reactions, cycloadditions).

### 7.5.2 Types of Reaction Mechanisms

Common types of reaction mechanisms include:

- **Addition Reactions**: Two or more reactants combine to form a single product (e.g., addition of $H_2$ to alkenes).
- **Elimination Reactions**: A molecule loses atoms or groups to form a smaller molecule, often with the formation of multiple bonds (e.g., dehydration of alcohols).
- **Substitution Reactions**: One atom or group in a molecule is replaced by another atom or group (e.g., $S_N1$ and $S_N2$ reactions).
- **Rearrangement Reactions**: Atoms or groups within a molecule are rearranged to form an isomer (e.g., Claisen rearrangement).
- **Redox Reactions**: Reactions involving the transfer of electrons between reactants, resulting in changes in oxidation states (e.g., combustion, electrochemical reactions).
- **Chain Reactions**: Reactions involving a series of steps, including initiation, propagation, and termination steps. Free radical reactions are often chain reactions (e.g., radical polymerization).
- **Catalytic Reactions**: Reactions accelerated by catalysts, which are substances that participate in the reaction mechanism but are regenerated at the end (e.g., enzyme catalysis, heterogeneous catalysis).

### 7.5.3 Determining Reaction Mechanisms

Determining reaction mechanisms involves experimental and computational methods.

- **Experimental Methods**: Kinetic studies, product analysis, stereochemical studies, isotopic labeling, and spectroscopic detection of intermediates are used to probe reaction mechanisms.
- **Computational Methods**: Quantum chemical calculations, PES analysis, and reaction dynamics simulations are used to model reaction mechanisms and predict reaction pathways.

Understanding reaction mechanisms is crucial for controlling chemical reactions, optimizing reaction conditions, and designing new synthetic strategies. It is a central theme in chemistry, bridging fundamental principles with practical applications.

In summary, particle interactions drive chemical reactions, and understanding these interactions, potential energy surfaces, reaction dynamics, reactive intermediates, and reaction mechanisms is essential for comprehending and predicting chemical reactivity. This chapter provides a foundation for further exploration into advanced topics in chemical kinetics and reaction engineering.

## Exercises

[Exercises(.md)](exercises/ch07_exercises.md)
[Exercises(.ipynb)](exercises/ch07_exercises.ipynb)

## References

[References](references/reference_list.md)
