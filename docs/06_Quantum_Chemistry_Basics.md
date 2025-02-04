[前の章: 05 Chemical Bonding in Relativistic Contexts](05_Chemical_Bonding_in_Relativistic_Contexts.md) - [次の章: 07 Particle Interactions in Chemical Reactions](07_Particle_Interactions_in_Chemical_Reactions.md)

# Quantum Chemistry Basics

This chapter provides an introduction to the fundamental principles of quantum chemistry. Quantum chemistry applies quantum mechanics to chemical systems and is essential for understanding molecular properties, chemical reactions, and spectroscopy. This chapter covers the basic postulates of quantum mechanics and their application to atomic and molecular systems.

## 6.1 Postulates of Quantum Mechanics

Quantum mechanics is built upon a set of postulates that form the foundation of the theory. These postulates describe the state of a quantum system, how observables are represented, and how the state evolves over time.

### 6.1.1 State of a Quantum System

**Postulate 1**: The state of a quantum mechanical system is completely specified by a function $\Psi(\mathbf{r}_1, \mathbf{r}_2, ..., t)$ called the wavefunction, which depends on the coordinates of all particles and time. For a many-electron system, $\Psi$ also depends on the spin coordinates of the electrons. The wavefunction must be single-valued, continuous, and square-integrable.

The wavefunction contains all the information that can be known about the system. The probability of finding a particle in a volume element $d\tau$ is given by $|\Psi|^2 d\tau$.

### 6.1.2 Observables and Operators

**Postulate 2**: To every physically observable quantity in classical mechanics there corresponds a linear, Hermitian operator in quantum mechanics.

For example, the position observable $x$ corresponds to the operator $\hat{x} = x$, and the momentum observable $p_x$ corresponds to the operator $\hat{p}_x = -i\hbar \frac{\partial}{\partial x}$. Some important quantum mechanical operators are:

- **Position operator** ($\hat{\mathbf{r}}$): Represents the position of a particle.
- **Momentum operator** ($\hat{\mathbf{p}} = -i\hbar \nabla$): Represents the momentum of a particle.
- **Kinetic energy operator** ($\hat{T} = -\frac{\hbar^2}{2m} \nabla^2$): Represents the kinetic energy of a particle.
- **Potential energy operator** ($\hat{V}(\mathbf{r})$): Represents the potential energy of a particle, which is a function of position.
- **Hamiltonian operator** ($\hat{H} = \hat{T} + \hat{V}$): Represents the total energy of the system.

### 6.1.3 Measurement in Quantum Mechanics

**Postulate 3**: In any measurement of the observable associated with the operator $\hat{A}$, the only values that will ever be observed are the eigenvalues of the operator $\hat{A}$.

If $\hat{A} \phi_n = a_n \phi_n$, where $a_n$ are eigenvalues and $\phi_n$ are eigenfunctions, then the possible measured values of the observable $A$ are the eigenvalues $a_n$.

**Postulate 4**: If the system is in a state described by a normalized wavefunction $\Psi$, then the average or expectation value of the observable corresponding to $\hat{A}$ is given by:

$$ \langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^* \hat{A} \Psi d\tau $$

This expectation value represents the average result of a large number of measurements on identically prepared systems.

### 6.1.4 Time Evolution of a Quantum System

**Postulate 5**: The time evolution of the state of a quantum mechanical system is governed by the time-dependent Schrödinger equation:

$$ i\hbar \frac{\partial \Psi}{\partial t} = \hat{H} \Psi $$

where $\hat{H}$ is the Hamiltonian operator for the system. If the Hamiltonian is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$ \hat{H} \psi = E \psi $$

where $E$ is the energy eigenvalue and $\psi$ is the time-independent wavefunction.

## 6.2 The Schrödinger Equation

The Schrödinger equation is the central equation of quantum mechanics. It describes how quantum mechanical systems behave and is used to calculate the allowed energies and wavefunctions of these systems.

### 6.2.1 Time-Independent Schrödinger Equation

For a time-independent potential, the Schrödinger equation simplifies to the time-independent Schrödinger equation:

$$ \hat{H} \psi(\mathbf{r}) = E \psi(\mathbf{r}) $$

In one dimension, for a single particle, this equation is:

$$ -\frac{\hbar^2}{2m} \frac{d^2 \psi(x)}{dx^2} + V(x) \psi(x) = E \psi(x) $$

Solving the Schrödinger equation for a given potential $V(x)$ yields the energy eigenvalues $E$ and the corresponding eigenfunctions $\psi(x)$.

### 6.2.2 Particle in a Box

The particle in a box is a fundamental problem in quantum mechanics that illustrates the quantization of energy. Consider a particle of mass $m$ confined to move in a one-dimensional box of length $L$ with infinite potential walls. The potential is:

$$ V(x) = \begin{cases} 0 & 0 \le x \le L \\ \infty & \text{otherwise} \end{cases} $$

Solving the Schrödinger equation for this potential gives the energy eigenvalues:

$$ E_n = \frac{n^2 \pi^2 \hbar^2}{2mL^2}, \quad n = 1, 2, 3, ... $$

and the corresponding eigenfunctions:

$$ \psi_n(x) = \sqrt{\frac{2}{L}} \sin\left(\frac{n\pi x}{L}\right), \quad 0 \le x \le L $$

The energy levels are quantized, meaning only discrete energy values are allowed. The quantum number $n$ labels the energy levels and wavefunctions.

### 6.2.3 Harmonic Oscillator

The harmonic oscillator is another crucial model system in quantum mechanics, representing systems undergoing vibrational motion. The potential for a one-dimensional harmonic oscillator is:

$$ V(x) = \frac{1}{2} kx^2 = \frac{1}{2} m\omega^2 x^2 $$

where $k$ is the force constant and $\omega = \sqrt{k/m}$ is the angular frequency. Solving the Schrödinger equation for this potential gives quantized energy levels:

$$ E_v = \hbar \omega \left(v + \frac{1}{2}\right), \quad v = 0, 1, 2, ... $$

and corresponding eigenfunctions involving Hermite polynomials. The harmonic oscillator model is essential for understanding molecular vibrations and infrared spectroscopy.

## 6.3 Atomic Orbitals and Atomic Structure

Quantum mechanics provides the framework for understanding the electronic structure of atoms. Atomic orbitals are solutions to the Schrödinger equation for a single electron in an atom.

### 6.3.1 Hydrogen Atom

The hydrogen atom, with one proton and one electron, is the simplest atom and an important system for quantum chemistry. The potential energy is due to the Coulomb attraction between the electron and the nucleus:

$$ V(r) = -\frac{e^2}{4\pi\epsilon_0 r} $$

Solving the Schrödinger equation for the hydrogen atom yields the atomic orbitals, characterized by quantum numbers:

- **Principal quantum number** ($n = 1, 2, 3, ...$): Determines the energy level and size of the orbital.
- **Angular momentum or azimuthal quantum number** ($l = 0, 1, 2, ..., n-1$): Determines the shape of the orbital (s, p, d, f orbitals).
- **Magnetic quantum number** ($m_l = -l, -l+1, ..., 0, ..., l-1, l$): Determines the orientation of the orbital in space.

### 6.3.2 Many-Electron Atoms

For atoms with more than one electron, the Schrödinger equation becomes more complex due to electron-electron interactions. Approximations are necessary to solve the many-electron Schrödinger equation.

- **Hartree-Fock Approximation**: An independent-particle model that treats each electron as moving in an average field created by all other electrons and the nucleus. It leads to a set of one-electron equations that can be solved iteratively.
- **Electron Configuration**: Describes the distribution of electrons among atomic orbitals in an atom. The Aufbau principle, Hund's rule, and Pauli exclusion principle guide the filling of atomic orbitals.
- **Term Symbols**: Used to describe the electronic state of an atom, considering total angular momentum and spin multiplicity.

## 6.4 Molecular Structure and Molecular Orbitals

Quantum chemistry extends the concepts of atomic structure to molecules, describing chemical bonds and molecular properties using molecular orbitals.

### 6.4.1 Born-Oppenheimer Approximation

The Born-Oppenheimer approximation simplifies molecular quantum mechanics by separating nuclear and electronic motion. Since nuclei are much heavier than electrons, we assume that the nuclei are stationary relative to the rapidly moving electrons. This allows us to solve the electronic Schrödinger equation for fixed nuclear positions.

### 6.4.2 Molecular Orbital Theory (MOT)

Molecular Orbital Theory (MOT) describes the electronic structure of molecules in terms of molecular orbitals, which are delocalized over the entire molecule. Molecular orbitals are formed by linear combinations of atomic orbitals (LCAO).

- **Linear Combination of Atomic Orbitals (LCAO)**: Molecular orbitals are approximated as linear combinations of atomic orbitals. For example, for a diatomic molecule AB, molecular orbitals can be formed by combining atomic orbitals of atom A and atom B.
- **Bonding and Antibonding Orbitals**: Combining atomic orbitals results in bonding molecular orbitals (lower energy, increased electron density between nuclei) and antibonding molecular orbitals (higher energy, decreased electron density between nuclei).
- **Sigma ($\sigma$), Pi ($\pi$), and Delta ($\delta$) Orbitals**: Molecular orbitals are classified based on their symmetry with respect to the internuclear axis.
- **Molecular Electronic Configuration**: Describes the filling of molecular orbitals with electrons, following the same rules as for atomic electron configurations (Aufbau principle, Hund's rule, Pauli exclusion principle).
- **Bond Order**: Calculated from the molecular electronic configuration, bond order indicates the number of chemical bonds and bond strength.

### 6.4.3 Examples of Molecular Orbitals

- **Diatomic Molecules**: MOT can be applied to diatomic molecules like $H_2, N_2, O_2, F_2$ to understand their bonding and magnetic properties. For example, the molecular orbital diagram of $O_2$ explains its paramagnetic nature due to unpaired electrons in $\pi^*$ antibonding orbitals.
- **Polyatomic Molecules**: MOT can be extended to polyatomic molecules, using symmetry and group theory to construct molecular orbitals and understand molecular bonding.

## 6.5 Computational Quantum Chemistry

Computational quantum chemistry uses numerical methods and computer programs to solve the Schrödinger equation and calculate molecular properties. It has become an indispensable tool in modern chemistry.

### 6.5.1 Hartree-Fock and Post-Hartree-Fock Methods

- **Hartree-Fock (HF)**: A mean-field method that provides a starting point for electronic structure calculations. It neglects electron correlation beyond the average field approximation.
- **Post-Hartree-Fock Methods**: Include electron correlation effects beyond the Hartree-Fock approximation. Examples include Møller-Plesset perturbation theory (MPn), Configuration Interaction (CI), and Coupled Cluster (CC) methods. These methods provide more accurate results but are computationally more demanding.

### 6.5.2 Density Functional Theory (DFT)

Density Functional Theory (DFT) is a widely used electronic structure method that calculates the electronic energy and other properties based on the electron density rather than the wavefunction. DFT methods are computationally efficient and often provide good accuracy for many chemical systems.

- **Functionals**: Approximations for the exchange-correlation energy functional in DFT. Common functionals include Local Density Approximation (LDA), Generalized Gradient Approximation (GGA), and hybrid functionals.
- **Applications of DFT**: DFT is used in a wide range of applications, including geometry optimization, vibrational frequency calculations, electronic spectra, and studying chemical reactions.

### 6.5.3 Basis Sets

Basis sets are sets of atomic orbitals used to construct molecular orbitals in computational quantum chemistry. The choice of basis set affects the accuracy and computational cost of calculations.

- **Minimal Basis Sets**: Use a minimum number of basis functions to represent each atomic orbital (e.g., STO-3G).
- **Split-Valence Basis Sets**: Use more basis functions for valence orbitals than core orbitals (e.g., 3-21G, 6-31G).
- **Polarization and Diffuse Functions**: Basis sets can be augmented with polarization functions (higher angular momentum functions) and diffuse functions (more extended functions) to improve accuracy, especially for anions and weak interactions.

### 6.5.4 Software Packages

Several software packages are available for computational quantum chemistry, such as Gaussian, ORCA, NWChem, and Q-Chem. These packages implement various quantum chemical methods and provide tools for calculating molecular properties and simulating chemical systems.

Computational quantum chemistry plays a crucial role in modern chemical research, enabling the study of complex molecules and chemical processes that are difficult to investigate experimentally. It provides valuable insights into molecular properties, reaction mechanisms, and materials design.

In summary, quantum chemistry provides the theoretical foundation and computational tools for understanding the electronic structure and properties of atoms and molecules. It is essential for explaining chemical bonding, molecular spectroscopy, chemical reactivity, and many other aspects of chemistry. This chapter has introduced the basic principles and methods of quantum chemistry, setting the stage for more advanced topics in subsequent chapters.

## Exercises

[Exercises(.md)](exercises/ch06_exercises.md)
[Exercises(.ipynb)](exercises/ch06_exercises.ipynb)

## References

[References](references/reference_list.md)
