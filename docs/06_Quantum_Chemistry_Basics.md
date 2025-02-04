# Quantum Chemistry Basics

This chapter introduces the fundamental principles and methods of quantum chemistry. Building upon the foundations of quantum mechanics, atomic structure, and chemical bonding, we will explore how quantum mechanics is applied to describe molecules and chemical reactions. This chapter will cover essential approximations and computational techniques used to solve the molecular Schrödinger equation, forming the basis for understanding more advanced relativistic quantum chemistry methods discussed in later chapters.

## 6.1 Introduction to Quantum Chemistry

Quantum chemistry is the branch of chemistry that applies quantum mechanics to chemical systems. It aims to understand and predict molecular properties, chemical reactions, and spectroscopic phenomena from first principles, using the laws of quantum mechanics.

### 6.1.1 The Molecular Schrödinger Equation

The central equation in quantum chemistry is the molecular Schrödinger equation, which describes the behavior of electrons and nuclei in molecules:

$$
\hat{H} \Psi(\mathbf{r}, \mathbf{R}) = E \Psi(\mathbf{r}, \mathbf{R})
$$

where:
- $\hat{H}$ is the molecular Hamiltonian operator.
- $\Psi(\mathbf{r}, \mathbf{R})$ is the molecular wavefunction, depending on electron coordinates $\mathbf{r}$ and nuclear coordinates $\mathbf{R}$.
- $E$ is the total energy of the molecule.

The molecular Hamiltonian $\hat{H}$ includes terms for:
- Kinetic energy of electrons and nuclei.
- Potential energy of electron-nucleus attraction.
- Potential energy of electron-electron repulsion.
- Potential energy of nucleus-nucleus repulsion.

### 6.1.2 Born-Oppenheimer Approximation

Solving the molecular Schrödinger equation exactly is extremely challenging for polyatomic molecules. The Born-Oppenheimer approximation simplifies the problem by separating nuclear and electronic motion. Due to the large mass difference between nuclei and electrons, we assume that nuclei are stationary relative to the much faster-moving electrons.

Under the Born-Oppenheimer approximation, the molecular wavefunction is separated into electronic and nuclear wavefunctions:

$$
\Psi(\mathbf{r}, \mathbf{R}) \approx \psi_{elec}(\mathbf{r}; \mathbf{R}) \times \chi_{nuc}(\mathbf{R})
$$

The electronic Schrödinger equation is solved for fixed nuclear positions $\mathbf{R}$:

$$
\hat{H}_{elec} \psi_{elec}(\mathbf{r}; \mathbf{R}) = E_{elec}(\mathbf{R}) \psi_{elec}(\mathbf{r}; \mathbf{R})
$$

The electronic Hamiltonian $\hat{H}_{elec}$ includes kinetic energy of electrons and all potential energy terms, while treating nuclear positions as parameters. The eigenvalue $E_{elec}(\mathbf{R})$ is the electronic energy, which depends on nuclear positions and serves as the potential energy for nuclear motion.

## 6.2 Electronic Structure Methods

Solving the electronic Schrödinger equation is still complex and requires further approximations. Various electronic structure methods have been developed, broadly categorized into:

### 6.2.1 Hartree-Fock (HF) Theory

Hartree-Fock (HF) theory is a foundational method in quantum chemistry that approximates the many-electron wavefunction by a single Slater determinant of spin-orbitals. It treats electron-electron interactions in an average way, neglecting instantaneous electron correlation.

#### Key Approximations in HF Theory:

- **Independent Electron Approximation**: Each electron moves in an effective potential created by the average field of all other electrons and nuclei.
- **Variational Principle**: The HF energy is an upper bound to the exact ground state energy.
- **Self-Consistent Field (SCF) Procedure**: The HF equations are solved iteratively until the electron density and energy converge.

#### Limitations of HF Theory:

- **Neglect of Electron Correlation**: HF theory does not account for the instantaneous correlation between electron motions, leading to overestimation of energies and inaccurate descriptions of certain molecular properties.
- **Basis Set Dependence**: Accuracy depends on the choice of atomic basis sets used to represent molecular orbitals.

### 6.2.2 Post-Hartree-Fock Methods

Post-Hartree-Fock methods aim to improve upon HF theory by including electron correlation effects. These methods are generally more computationally demanding than HF.

#### Examples of Post-HF Methods:

- **Møller-Plesset Perturbation Theory (MPn)**: Treats electron correlation as a perturbation to the HF wavefunction. MP2 (second-order MP theory) is a common and relatively cost-effective method.
- **Configuration Interaction (CI)**: Expands the wavefunction as a linear combination of Slater determinants representing different electronic configurations. Full CI is exact within a given basis set but computationally very expensive. Truncated CI methods like CISD (CI with singles and doubles) are more practical.
- **Coupled Cluster (CC) Theory**: Provides a highly accurate description of electron correlation by exponentiating cluster operators. CCSD (CC with singles and doubles) and CCSD(T) (CCSD with perturbative triples) are widely used high-accuracy methods.
- **Multi-Configurational Self-Consistent Field (MCSCF)**: Optimizes both molecular orbitals and configuration coefficients simultaneously, important for describing molecules with multireference character (e.g., bond breaking, excited states).

### 6.2.3 Density Functional Theory (DFT)

Density Functional Theory (DFT) is a widely used electronic structure method that, in principle, exactly accounts for electron correlation at a lower computational cost than many post-HF methods. DFT is based on the Hohenberg-Kohn theorems, which state that the ground state electronic energy and all other ground state properties are uniquely determined by the electron density $\rho(\mathbf{r})$.

#### Key Concepts in DFT:

- **Electron Density as Basic Variable**: DFT focuses on the electron density $\rho(\mathbf{r})$ instead of the many-electron wavefunction.
- **Kohn-Sham Equations**: A set of effective single-particle equations that yield the exact electron density of the interacting system.
- **Exchange-Correlation Functional**: The central unknown in DFT is the exchange-correlation functional $E_{xc}[\rho]$, which accounts for exchange and correlation effects. Approximations to $E_{xc}[\rho]$ are crucial for the accuracy of DFT calculations.

#### Common Approximations for Exchange-Correlation Functionals:

- **Local Density Approximation (LDA)**: Approximates $E_{xc}[\rho]$ locally based on the uniform electron gas.
- **Generalized Gradient Approximation (GGA)**: Includes gradients of the density in $E_{xc}[\rho]$, improving upon LDA. Common GGAs include BLYP and PBE.
- **Hybrid Functionals**: Mixes HF exchange with DFT exchange and correlation, such as B3LYP and PBE0, often providing better accuracy for thermochemistry and kinetics.
- **Meta-GGA Functionals**: Include second derivatives of the density or kinetic energy density, further improving accuracy.
- **Range-Separated Functionals**: Separates exchange interaction into short-range and long-range parts, useful for systems with charge-transfer or long-range interactions.

#### Advantages of DFT:

- **Computational Efficiency**: DFT is generally less computationally demanding than post-HF methods, allowing for calculations on larger molecules.
- **Inclusion of Electron Correlation**: DFT, in principle, includes electron correlation, often providing better accuracy than HF theory.

#### Limitations of DFT:

- **Approximation of Exchange-Correlation Functional**: The exact form of $E_{xc}[\rho]$ is unknown, and the accuracy of DFT calculations depends on the quality of the approximate functional used.
- **Challenges with Dispersion Interactions and Strong Correlation**: Standard DFT functionals may struggle with van der Waals dispersion interactions and strongly correlated systems.

## 6.3 Basis Sets

In quantum chemical calculations, molecular orbitals are typically expanded as linear combinations of atomic basis functions. The choice of basis set affects the accuracy and computational cost of calculations.

### 6.3.1 Types of Basis Sets

- **Slater-Type Orbitals (STOs)**: Functions that resemble atomic orbitals and have the correct exponential decay. STO-3G is a minimal basis set using Gaussian approximations to STOs.
- **Gaussian-Type Orbitals (GTOs)**: Gaussian functions are computationally more efficient than STOs for evaluating integrals. Basis sets are typically constructed from contracted Gaussian functions (CGFs), which are linear combinations of primitive Gaussians.

### 6.3.2 Common Basis Set Families

- **Pople-style basis sets**: e.g., 6-31G, 6-31G(d), 6-31+G(d,p). Split-valence basis sets (e.g., 6-31G) describe core and valence electrons with different numbers of basis functions. Polarization functions (e.g., (d), (d,p)) add functions with higher angular momentum to allow for better description of molecular bonding. Diffuse functions (e.g., +) are important for anions and Rydberg states.
- **Correlation-Consistent basis sets (cc-pVnZ)**: Designed for correlation calculations and systematically converge to the complete basis set limit as n increases (cc-pVDZ, cc-pVTZ, cc-pVQZ, etc.). Augmented versions (aug-cc-pVnZ) include diffuse functions.
- **Polarization-Consistent basis sets (pc-n)**: Optimized for DFT calculations and provide systematic convergence for DFT energies and properties.

### 6.3.3 Basis Set Superposition Error (BSSE)

When using finite basis sets, especially for intermolecular interactions, Basis Set Superposition Error (BSSE) can arise. BSSE is an artifact that artificially lowers the energy of interacting systems due to basis functions from one molecule "borrowing" basis functions from another molecule to improve its description. BSSE can be corrected using methods like the Counterpoise Correction.

## 6.4 Molecular Properties

Quantum chemistry methods can be used to calculate a wide range of molecular properties beyond energies and structures:

### 6.4.1 Electronic Properties

- **Dipole Moments, Multipole Moments**: Describe the charge distribution in a molecule.
- **Polarizability**: Measures the response of a molecule to an electric field.
- **Electron Density, Molecular Electrostatic Potential (MEP)**: Visualize charge distribution and reactive sites in molecules.
- **Ionization Potentials, Electron Affinities**: Energies related to removing or adding electrons.

### 6.4.2 Spectroscopic Properties

- **Vibrational Frequencies, IR and Raman Spectra**: Calculated from the Hessian matrix (second derivatives of energy with respect to nuclear coordinates).
- **Electronic Excitation Energies, UV-Vis Spectra**: Calculated using time-dependent DFT (TD-DFT) or excited-state methods like CIS, EOM-CCSD.
- **NMR Chemical Shifts, EPR g-tensors**: Magnetic resonance parameters sensitive to electronic and molecular structure.

### 6.4.3 Thermochemical Properties

- **Enthalpies of Formation, Reaction Energies**: Calculated using total energies and vibrational frequencies.
- **Entropy, Gibbs Free Energy**: Statistical thermodynamics combined with quantum chemical calculations.
- **Reaction Rate Constants**: Transition state theory and quantum dynamics calculations.

## 6.5 Software and Computational Chemistry

Quantum chemistry calculations are typically performed using specialized software packages. Popular quantum chemistry software includes:

- **Gaussian**: A widely used commercial software package with a broad range of methods and properties.
- **ORCA**: A versatile and efficient quantum chemistry program with a focus on advanced methods and spectroscopy.
- **NWChem**: A powerful open-source software package with high-performance computing capabilities.
- **Psi4**: An open-source software package focused on high-accuracy methods and extensibility.
- **Q-Chem**: A commercial software package with a focus on fast methods and large systems.

Computational chemistry involves using these software packages to solve chemical problems, design molecules, and interpret experimental data. It is an essential tool in modern chemical research and development.

In summary, quantum chemistry provides the theoretical framework and computational tools to understand molecular structure, properties, and reactivity from a quantum mechanical perspective. This chapter lays the groundwork for exploring more advanced topics, including relativistic quantum chemistry, in subsequent chapters.
