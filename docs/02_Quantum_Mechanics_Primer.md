[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)

# Quantum Mechanics Primer

This chapter will provide a primer on quantum mechanics, laying the groundwork for understanding relativistic quantum chemistry. We will cover the fundamental concepts necessary to grasp the quantum phenomena that are crucial in the later chapters.

## 2.1 Wave-Particle Duality

One of the foundational concepts of quantum mechanics is wave-particle duality. This principle states that every quantum entity may be described as both a particle and a wave. 

### 2.1.1 de Broglie Wavelength

Louis de Broglie proposed that particles, like electrons, can exhibit wave-like properties, with a wavelength $\lambda$ related to their momentum $p$ by the de Broglie relation:

$$
\lambda = \frac{h}{p}
$$

where $h$ is Planck's constant. This equation implies that particles with larger momentum have shorter wavelengths, and vice versa.

### 2.1.2 Experimental Evidence

The wave nature of particles has been experimentally confirmed through phenomena like electron diffraction. In the double-slit experiment, electrons, when passed through two slits, create an interference pattern, which is characteristic of waves.

## 2.2 The Schrödinger Equation

The time-dependent Schrödinger equation is the central equation in quantum mechanics that describes how the quantum state of a physical system changes in time.

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

where:
- $i$ is the imaginary unit,
- $\hbar = \frac{h}{2\pi}$ is the reduced Planck's constant,
- $\Psi(\mathbf{r}, t)$ is the wave function, which describes the quantum state of the particle as a function of position $\mathbf{r}$ and time $t$,
- $\hat{H}$ is the Hamiltonian operator, representing the total energy of the system.

For a single particle in a potential $V(\mathbf{r}, t)$, the Hamiltonian is given by:

$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(\mathbf{r}, t)
$$

where $m$ is the mass of the particle and $\nabla^2$ is the Laplacian operator.

### 2.2.1 Time-Independent Schrödinger Equation

For stationary states, where the potential energy is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$
\hat{H}\psi(\mathbf{r}) = E\psi(\mathbf{r})
$$

where:
- $\psi(\mathbf{r})$ is the time-independent wave function,
- $E$ is the energy eigenvalue of the stationary state.

## 2.3 Quantum Operators

In quantum mechanics, physical observables are represented by linear operators acting on the wave function.

### 2.3.1 Position Operator

The position operator $\hat{\mathbf{r}}$ simply multiplies the wave function by the position vector $\mathbf{r}$:

$$
\hat{\mathbf{r}}\psi(\mathbf{r}) = \mathbf{r}\psi(\mathbf{r})
$$

### 2.3.2 Momentum Operator

The momentum operator $\hat{\mathbf{p}}$ is represented in position space as:

$$
\hat{\mathbf{p}} = -i\hbar\nabla
$$

Applying the momentum operator to a wave function gives:

$$
\hat{\mathbf{p}}\psi(\mathbf{r}) = -i\hbar\nabla\psi(\mathbf{r})
$$

### 2.3.3 Energy Operator (Hamiltonian)

As introduced in the Schrödinger equation, the Hamiltonian operator $\hat{H}$ represents the total energy of the system.

### 2.3.4 Angular Momentum Operator

The angular momentum operator $\hat{\mathbf{L}}$ is defined as:

$$
\hat{\mathbf{L}} = \hat{\mathbf{r}} \times \hat{\mathbf{p}}
$$

In Cartesian coordinates, the components are:

$$
\begin{aligned}
\hat{L}_x &= \hat{y}\hat{p}_z - \hat{z}\hat{p}_y \\
\hat{L}_y &= \hat{z}\hat{p}_x - \hat{x}\hat{p}_z \\
\hat{L}_z &= \hat{x}\hat{p}_y - \hat{y}\hat{p}_x
\end{aligned}
$$

## 2.4 Expectation Values

The expectation value of a physical observable $A$, represented by the operator $\hat{A}$, for a system in a state described by the normalized wave function $\Psi$, is given by:

$$
\langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^*(\mathbf{r}, t) \hat{A} \Psi(\mathbf{r}, t) d^3r
$$

For example, the expectation value of the position $\langle \mathbf{r} \rangle$ and momentum $\langle \mathbf{p} \rangle$ can be calculated using their respective operators.

## 2.5 Heisenberg's Uncertainty Principle

Heisenberg's uncertainty principle states that there is a fundamental limit to the precision with which certain pairs of physical properties of a particle, known as complementary variables, can be known simultaneously. For position and momentum, this principle is expressed as:

$$
\Delta x \Delta p_x \geq \frac{\hbar}{2}
$$

where $\Delta x$ and $\Delta p_x$ are the standard deviations of position and momentum in the x-direction, respectively. This principle is not due to limitations in measurement instruments but is inherent in the quantum nature of particles.

This primer provides a basic overview of quantum mechanics. In the following sections and chapters, we will build upon these fundamental concepts to explore more advanced topics in relativistic quantum chemistry.

## 2.6 Quantum Harmonic Oscillator

The quantum harmonic oscillator is a fundamental model in quantum mechanics that describes systems experiencing a restoring force proportional to their displacement from equilibrium. It is used to model molecular vibrations, lattice vibrations in solids, and many other physical systems.

### 2.6.1 Hamiltonian

The Hamiltonian for a one-dimensional quantum harmonic oscillator is given by:

$$
\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2
$$

where:
- $\hat{p}$ is the momentum operator,
- $m$ is the mass of the particle,
- $\omega$ is the angular frequency of the oscillator,
- $\hat{x}$ is the position operator.

### 2.6.2 Energy Eigenvalues

The energy eigenvalues for the quantum harmonic oscillator are quantized and given by:

$$
E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0, 1, 2, \ldots
$$

where $n$ is the quantum number. The lowest energy level, $E_0 = \frac{1}{2}\hbar\omega$, is known as the zero-point energy, which is a purely quantum mechanical phenomenon.

### 2.6.3 Wave Functions

The wave functions for the harmonic oscillator can be expressed in terms of Hermite polynomials. The ground state wave function ($n=0$) is a Gaussian function:

$$
\psi_0(x) = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}
$$

and higher energy wave functions are given by:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

where $H_n(x)$ are the Hermite polynomials.

The quantum harmonic oscillator illustrates key quantum mechanical concepts such as energy quantization and zero-point energy, and it serves as a crucial building block for understanding more complex quantum systems.

## 2.7 Hydrogen Atom

The hydrogen atom, consisting of a single proton and a single electron, is the simplest atom and one of the most important systems in quantum mechanics. It is the only atom for which the Schrödinger equation can be solved analytically, providing a foundation for understanding more complex atoms and molecules.

### 2.7.1 Hamiltonian

The Hamiltonian for the hydrogen atom, neglecting relativistic effects and spin-orbit coupling, is given by:

$$
\hat{H} = -\frac{\hbar^2}{2\mu}\nabla^2 - \frac{e^2}{4\pi\epsilon_0 r}
$$

where:
- $\mu = \frac{m_e m_p}{m_e + m_p}$ is the reduced mass of the electron-proton system,
- $m_e$ is the mass of the electron,
- $m_p$ is the mass of the proton,
- $e$ is the elementary charge,
- $\epsilon_0$ is the vacuum permittivity,
- $r$ is the distance between the electron and the proton.

### 2.7.2 Energy Eigenvalues

The energy eigenvalues for the hydrogen atom are given by the Rydberg formula:

$$
E_n = -\frac{R_y}{n^2}, \quad n = 1, 2, 3, \ldots
$$

where:
- $R_y = \frac{\mu e^4}{8\epsilon_0^2 h^2} \approx 13.6 \text{ eV}$ is the Rydberg constant,
- $n$ is the principal quantum number.

The negative sign indicates that the energy is bound, and $n=1$ corresponds to the ground state, with higher values of $n$ corresponding to excited states.

### 2.7.3 Atomic Orbitals

The wave functions for the hydrogen atom are called atomic orbitals and are described by three quantum numbers:
- Principal quantum number $n$: determines the energy level and can be any positive integer ($n = 1, 2, 3, \ldots$).
- Angular momentum or azimuthal quantum number $l$: determines the shape of the orbital and can range from $0$ to $n-1$. ($l=0, 1, 2, \ldots, n-1$)
- Magnetic quantum number $m_l$: determines the orientation of the orbital in space and can take integer values from $-l$ to $+l$. ($m_l = -l, -l+1, \ldots, 0, \ldots, l-1, l$)

For example, for $n=1$, we have only $l=0$ and $m_l=0$, which corresponds to the 1s orbital. For $n=2$, we have $l=0$ (2s orbital) and $l=1$ (2p orbitals, with $m_l = -1, 0, 1$).

The hydrogen atom solutions provide a crucial foundation for understanding the electronic structure of all atoms and molecules, and the concept of atomic orbitals is fundamental in chemistry.

## 2.8 Spin Angular Momentum

In addition to orbital angular momentum, particles like electrons possess an intrinsic angular momentum called spin angular momentum, or simply spin. Spin is a purely quantum mechanical property with no classical analogue.

### 2.8.1 Spin Quantum Numbers

For electrons, spin angular momentum is quantized and described by two quantum numbers:
- Spin quantum number $s = \frac{1}{2}$ (for electrons, always $\frac{1}{2}$).
- Spin magnetic quantum number $m_s$: can take two values, $m_s = +\frac{1}{2}$ (spin up, $\uparrow$) and $m_s = -\frac{1}{2}$ (spin down, $\downarrow$).

### 2.8.2 Spin Operators

Spin is also associated with operators, analogous to orbital angular momentum operators. The spin operators $\hat{S}^2$, $\hat{S}_x$, $\hat{S}_y$, and $\hat{S}_z$ satisfy similar commutation relations as the orbital angular momentum operators.

### 2.8.3 Total Angular Momentum

The total angular momentum $\hat{\mathbf{J}}$ of an electron in an atom is the sum of its orbital angular momentum $\hat{\mathbf{L}}$ and spin angular momentum $\hat{\mathbf{S}}$:

$$
\hat{\mathbf{J}} = \hat{\mathbf{L}} + \hat{\mathbf{S}}
$$

Total angular momentum is crucial for understanding atomic spectra and magnetic properties, especially in relativistic quantum mechanics where spin-orbit coupling becomes significant.

## 2.9 Approximation Methods

For most quantum mechanical systems, especially those involving multiple particles, solving the Schrödinger equation analytically is impossible. Therefore, approximation methods are essential tools in quantum mechanics to obtain approximate solutions that are sufficiently accurate for practical purposes. We will briefly introduce two common approximation methods: perturbation theory and the variational method.

### 2.9.1 Perturbation Theory

Perturbation theory is used when the Hamiltonian of a system can be written as a sum of an unperturbed Hamiltonian $\hat{H}_0$ for which the solutions are known, and a small perturbation $\hat{H}'$:

$$
\hat{H} = \hat{H}_0 + \lambda\hat{H}'
$$

where $\lambda$ is a dimensionless parameter much smaller than 1. We can then expand the energy eigenvalues and eigenfunctions in powers of $\lambda$.

To first order in perturbation theory, the energy correction is given by:

$$
E_n^{(1)} = \langle \psi_n^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle
$$

and the first-order correction to the wave function is:

$$
| \psi_n^{(1)} \rangle = \sum_{k \neq n} \frac{\langle \psi_k^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle}{E_n^{(0)} - E_k^{(0)}} | \psi_k^{(0)} \rangle
$$

where $E_n^{(0)}$ and $| \psi_n^{(0)} \rangle$ are the eigenvalues and eigenfunctions of the unperturbed Hamiltonian $\hat{H}_0$.

### 2.9.2 Variational Method

The variational method is based on the variational principle, which states that for any trial wave function $\phi$, the expectation value of the Hamiltonian $\hat{H}$ is an upper bound to the true ground state energy $E_0$:

$$
\langle \phi | \hat{H} | \phi \rangle \geq E_0
$$

By minimizing the expectation value of the Hamiltonian with respect to the parameters in the trial wave function, we can obtain an approximation to the ground state energy and wave function.

For example, if we choose a trial wave function $\phi(\alpha)$ that depends on a parameter $\alpha$, we can find the optimal $\alpha$ by minimizing the energy expectation value:

$$
\frac{d}{d\alpha} \langle \phi(\alpha) | \hat{H} | \phi(\alpha) \rangle = 0
$$

The variational method is particularly useful for finding approximate ground state energies and wave functions for complex systems.

## 2.10 Time-Dependent Quantum Mechanics

So far, we have mainly discussed time-independent quantum mechanics and stationary states. However, many phenomena, such as spectroscopy and scattering, require a time-dependent treatment. Time-dependent quantum mechanics describes how quantum systems evolve in time under the influence of time-dependent potentials.

### 2.10.1 Time-Dependent Schrödinger Equation

As introduced earlier, the time-dependent Schrödinger equation is:

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

For a time-dependent Hamiltonian $\hat{H}(t)$, the solutions $\Psi(\mathbf{r}, t)$ describe the time evolution of the quantum system.

### 2.10.2 Time Evolution Operator

The time evolution of a quantum state can be formally described by the time evolution operator $\hat{U}(t, t_0)$, which propagates the state from time $t_0$ to time $t$:

$$
\Psi(t) = \hat{U}(t, t_0)\Psi(t_0)
$$

For a time-independent Hamiltonian, the time evolution operator is given by:

$$
\hat{U}(t, t_0) = e^{-i\hat{H}(t - t_0)/\hbar}
$$

For time-dependent Hamiltonians, the time evolution operator is more complex and often requires numerical methods or approximations to calculate.

### 2.10.3 Transitions and Spectroscopy

Time-dependent quantum mechanics is essential for understanding transitions between quantum states induced by time-dependent perturbations, such as electromagnetic radiation. This is the basis for spectroscopy, where the absorption and emission of photons by atoms and molecules are studied to probe their energy levels and structure.

In summary, approximation methods and time-dependent quantum mechanics are crucial extensions of basic quantum mechanics that allow us to study more realistic and complex quantum systems and phenomena. These concepts will be further relevant when we discuss relativistic quantum chemistry and its applications.

---

[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)

---

## 2.11 Summary
# Quantum Mechanics Primer

This chapter will provide a primer on quantum mechanics, laying the groundwork for understanding relativistic quantum chemistry. We will cover the fundamental concepts necessary to grasp the quantum phenomena that are crucial in the later chapters.

<a href="01_Basics_of_Relativity.md">前の章: 01 Basics of Relativity</a> | <a href="03_Particle_Physics_and_Atomic_Structure.md">次の章: 03 Particle Physics and Atomic Structure</a>

---
[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)
## 2.1 Wave-Particle Duality

One of the foundational concepts of quantum mechanics is wave-particle duality. This principle states that every quantum entity may be described as both a particle and a wave. 

### 2.1.1 de Broglie Wavelength

Louis de Broglie proposed that particles, like electrons, can exhibit wave-like properties, with a wavelength $\lambda$ related to their momentum $p$ by the de Broglie relation:

$$
\lambda = \frac{h}{p}
$$

where $h$ is Planck's constant. This equation implies that particles with larger momentum have shorter wavelengths, and vice versa.

### 2.1.2 Experimental Evidence

The wave nature of particles has been experimentally confirmed through phenomena like electron diffraction. In the double-slit experiment, electrons, when passed through two slits, create an interference pattern, which is characteristic of waves.

## 2.2 The Schrödinger Equation

The time-dependent Schrödinger equation is the central equation in quantum mechanics that describes how the quantum state of a physical system changes in time.

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

where:
- $i$ is the imaginary unit,
- $\hbar = \frac{h}{2\pi}$ is the reduced Planck's constant,
- $\Psi(\mathbf{r}, t)$ is the wave function, which describes the quantum state of the particle as a function of position $\mathbf{r}$ and time $t$,
- $\hat{H}$ is the Hamiltonian operator, representing the total energy of the system.

For a single particle in a potential $V(\mathbf{r}, t)$, the Hamiltonian is given by:

$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(\mathbf{r}, t)
$$

where $m$ is the mass of the particle and $\nabla^2$ is the Laplacian operator.

### 2.2.1 Time-Independent Schrödinger Equation

For stationary states, where the potential energy is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$
\hat{H}\psi(\mathbf{r}) = E\psi(\mathbf{r})
$$

where:
- $\psi(\mathbf{r})$ is the time-independent wave function,
- $E$ is the energy eigenvalue of the stationary state.

## 2.3 Quantum Operators

In quantum mechanics, physical observables are represented by linear operators acting on the wave function.

### 2.3.1 Position Operator

The position operator $\hat{\mathbf{r}}$ simply multiplies the wave function by the position vector $\mathbf{r}$:

$$
\hat{\mathbf{r}}\psi(\mathbf{r}) = \mathbf{r}\psi(\mathbf{r})
$$

### 2.3.2 Momentum Operator

The momentum operator $\hat{\mathbf{p}}$ is represented in position space as:

$$
\hat{\mathbf{p}} = -i\hbar\nabla
$$

Applying the momentum operator to a wave function gives:

$$
\hat{\mathbf{p}}\psi(\mathbf{r}) = -i\hbar\nabla\psi(\mathbf{r})
$$

### 2.3.3 Energy Operator (Hamiltonian)

As introduced in the Schrödinger equation, the Hamiltonian operator $\hat{H}$ represents the total energy of the system.

### 2.3.4 Angular Momentum Operator

The angular momentum operator $\hat{\mathbf{L}}$ is defined as:

$$
\hat{\mathbf{L}} = \hat{\mathbf{r}} \times \hat{\mathbf{p}}
$$

In Cartesian coordinates, the components are:

$$
\begin{aligned}
\hat{L}_x &= \hat{y}\hat{p}_z - \hat{z}\hat{p}_y \\
\hat{L}_y &= \hat{z}\hat{p}_x - \hat{x}\hat{p}_z \\
\hat{L}_z &= \hat{x}\hat{p}_y - \hat{y}\hat{p}_x
\end{aligned}
$$

## 2.4 Expectation Values

The expectation value of a physical observable $A$, represented by the operator $\hat{A}$, for a system in a state described by the normalized wave function $\Psi$, is given by:

$$
\langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^*(\mathbf{r}, t) \hat{A} \Psi(\mathbf{r}, t) d^3r
$$

For example, the expectation value of the position $\langle \mathbf{r} \rangle$ and momentum $\langle \mathbf{p} \rangle$ can be calculated using their respective operators.

## 2.5 Heisenberg's Uncertainty Principle

Heisenberg's uncertainty principle states that there is a fundamental limit to the precision with which certain pairs of physical properties of a particle, known as complementary variables, can be known simultaneously. For position and momentum, this principle is expressed as:

$$
\Delta x \Delta p_x \geq \frac{\hbar}{2}
$$

where $\Delta x$ and $\Delta p_x$ are the standard deviations of position and momentum in the x-direction, respectively. This principle is not due to limitations in measurement instruments but is inherent in the quantum nature of particles.

This primer provides a basic overview of quantum mechanics. In the following sections and chapters, we will build upon these fundamental concepts to explore more advanced topics in relativistic quantum chemistry.

## 2.6 Quantum Harmonic Oscillator

The quantum harmonic oscillator is a fundamental model in quantum mechanics that describes systems experiencing a restoring force proportional to their displacement from equilibrium. It is used to model molecular vibrations, lattice vibrations in solids, and many other physical systems.

### 2.6.1 Hamiltonian

The Hamiltonian for a one-dimensional quantum harmonic oscillator is given by:

$$
\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2
$$

where:
- $\hat{p}$ is the momentum operator,
- $m$ is the mass of the particle,
- $\omega$ is the angular frequency of the oscillator,
- $\hat{x}$ is the position operator.

### 2.6.2 Energy Eigenvalues

The energy eigenvalues for the quantum harmonic oscillator are quantized and given by:

$$
E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0, 1, 2, \ldots
$$

where $n$ is the quantum number. The lowest energy level, $E_0 = \frac{1}{2}\hbar\omega$, is known as the zero-point energy, which is a purely quantum mechanical phenomenon.

### 2.6.3 Wave Functions

The wave functions for the harmonic oscillator can be expressed in terms of Hermite polynomials. The ground state wave function ($n=0$) is a Gaussian function:

$$
\psi_0(x) = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}
$$

and higher energy wave functions are given by:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

where $H_n(x)$ are the Hermite polynomials.

The quantum harmonic oscillator illustrates key quantum mechanical concepts such as energy quantization and zero-point energy, and it serves as a crucial building block for understanding more complex quantum systems.

## 2.7 Hydrogen Atom

The hydrogen atom, consisting of a single proton and a single electron, is the simplest atom and one of the most important systems in quantum mechanics. It is the only atom for which the Schrödinger equation can be solved analytically, providing a foundation for understanding more complex atoms and molecules.

### 2.7.1 Hamiltonian

The Hamiltonian for the hydrogen atom, neglecting relativistic effects and spin-orbit coupling, is given by:

$$
\hat{H} = -\frac{\hbar^2}{2\mu}\nabla^2 - \frac{e^2}{4\pi\epsilon_0 r}
$$

where:
- $\mu = \frac{m_e m_p}{m_e + m_p}$ is the reduced mass of the electron-proton system,
- $m_e$ is the mass of the electron,
- $m_p$ is the mass of the proton,
- $e$ is the elementary charge,
- $\epsilon_0$ is the vacuum permittivity,
- $r$ is the distance between the electron and the proton.

### 2.7.2 Energy Eigenvalues

The energy eigenvalues for the hydrogen atom are given by the Rydberg formula:

$$
E_n = -\frac{R_y}{n^2}, \quad n = 1, 2, 3, \ldots
$$

where:
- $R_y = \frac{\mu e^4}{8\epsilon_0^2 h^2} \approx 13.6 \text{ eV}$ is the Rydberg constant,
- $n$ is the principal quantum number.

The negative sign indicates that the energy is bound, and $n=1$ corresponds to the ground state, with higher values of $n$ corresponding to excited states.

### 2.7.3 Atomic Orbitals

The wave functions for the hydrogen atom are called atomic orbitals and are described by three quantum numbers:
- Principal quantum number $n$: determines the energy level and can be any positive integer ($n = 1, 2, 3, \ldots$).
- Angular momentum or azimuthal quantum number $l$: determines the shape of the orbital and can range from $0$ to $n-1$. ($l=0, 1, 2, \ldots, n-1$)
- Magnetic quantum number $m_l$: determines the orientation of the orbital in space and can take integer values from $-l$ to $+l$. ($m_l = -l, -l+1, \ldots, 0, \ldots, l-1, l$)

For example, for $n=1$, we have only $l=0$ and $m_l=0$, which corresponds to the 1s orbital. For $n=2$, we have $l=0$ (2s orbital) and $l=1$ (2p orbitals, with $m_l = -1, 0, 1$).

The hydrogen atom solutions provide a crucial foundation for understanding the electronic structure of all atoms and molecules, and the concept of atomic orbitals is fundamental in chemistry.

## 2.8 Spin Angular Momentum

In addition to orbital angular momentum, particles like electrons possess an intrinsic angular momentum called spin angular momentum, or simply spin. Spin is a purely quantum mechanical property with no classical analogue.

### 2.8.1 Spin Quantum Numbers

For electrons, spin angular momentum is quantized and described by two quantum numbers:
- Spin quantum number $s = \frac{1}{2}$ (for electrons, always $\frac{1}{2}$).
- Spin magnetic quantum number $m_s$: can take two values, $m_s = +\frac{1}{2}$ (spin up, $\uparrow$) and $m_s = -\frac{1}{2}$ (spin down, $\downarrow$).

### 2.8.2 Spin Operators

Spin is also associated with operators, analogous to orbital angular momentum operators. The spin operators $\hat{S}^2$, $\hat{S}_x$, $\hat{S}_y$, and $\hat{S}_z$ satisfy similar commutation relations as the orbital angular momentum operators.

### 2.8.3 Total Angular Momentum

The total angular momentum $\hat{\mathbf{J}}$ of an electron in an atom is the sum of its orbital angular momentum $\hat{\mathbf{L}}$ and spin angular momentum $\hat{\mathbf{S}}$:

$$
\hat{\mathbf{J}} = \hat{\mathbf{L}} + \hat{\mathbf{S}}
$$

Total angular momentum is crucial for understanding atomic spectra and magnetic properties, especially in relativistic quantum mechanics where spin-orbit coupling becomes significant.

## 2.9 Approximation Methods

For most quantum mechanical systems, especially those involving multiple particles, solving the Schrödinger equation analytically is impossible. Therefore, approximation methods are essential tools in quantum mechanics to obtain approximate solutions that are sufficiently accurate for practical purposes. We will briefly introduce two common approximation methods: perturbation theory and the variational method.

### 2.9.1 Perturbation Theory

Perturbation theory is used when the Hamiltonian of a system can be written as a sum of an unperturbed Hamiltonian $\hat{H}_0$ for which the solutions are known, and a small perturbation $\hat{H}'$:

$$
\hat{H} = \hat{H}_0 + \lambda\hat{H}'
$$

where $\lambda$ is a dimensionless parameter much smaller than 1. We can then expand the energy eigenvalues and eigenfunctions in powers of $\lambda$.

To first order in perturbation theory, the energy correction is given by:

$$
E_n^{(1)} = \langle \psi_n^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle
$$

and the first-order correction to the wave function is:

$$
| \psi_n^{(1)} \rangle = \sum_{k \neq n} \frac{\langle \psi_k^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle}{E_n^{(0)} - E_k^{(0)}} | \psi_k^{(0)} \rangle
$$

where $E_n^{(0)}$ and $| \psi_n^{(0)} \rangle$ are the eigenvalues and eigenfunctions of the unperturbed Hamiltonian $\hat{H}_0$.

### 2.9.2 Variational Method

The variational method is based on the variational principle, which states that for any trial wave function $\phi$, the expectation value of the Hamiltonian $\hat{H}$ is an upper bound to the true ground state energy $E_0$:

$$
\langle \phi | \hat{H} | \phi \rangle \geq E_0
$$

By minimizing the expectation value of the Hamiltonian with respect to the parameters in the trial wave function, we can obtain an approximation to the ground state energy and wave function.

For example, if we choose a trial wave function $\phi(\alpha)$ that depends on a parameter $\alpha$, we can find the optimal $\alpha$ by minimizing the energy expectation value:

$$
\frac{d}{d\alpha} \langle \phi(\alpha) | \hat{H} | \phi(\alpha) \rangle = 0
$$

The variational method is particularly useful for finding approximate ground state energies and wave functions for complex systems.

## 2.10 Time-Dependent Quantum Mechanics

So far, we have mainly discussed time-independent quantum mechanics and stationary states. However, many phenomena, such as spectroscopy and scattering, require a time-dependent treatment. Time-dependent quantum mechanics describes how quantum systems evolve in time under the influence of time-dependent potentials.

### 2.10.1 Time-Dependent Schrödinger Equation

As introduced earlier, the time-dependent Schrödinger equation is:

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

For a time-dependent Hamiltonian $\hat{H}(t)$, the solutions $\Psi(\mathbf{r}, t)$ describe the time evolution of the quantum system.

### 2.10.2 Time Evolution Operator

The time evolution of a quantum state can be formally described by the time evolution operator $\hat{U}(t, t_0)$, which propagates the state from time $t_0$ to time $t$:

$$
\Psi(t) = \hat{U}(t, t_0)\Psi(t_0)
$$

For a time-independent Hamiltonian, the time evolution operator is given by:

$$
\hat{U}(t, t_0) = e^{-i\hat{H}(t - t_0)/\hbar}
$$

For time-dependent Hamiltonians, the time evolution operator is more complex and often requires numerical methods or approximations to calculate.

### 2.10.3 Transitions and Spectroscopy

Time-dependent quantum mechanics is essential for understanding transitions between quantum states induced by time-dependent perturbations, such as electromagnetic radiation. This is the basis for spectroscopy, where the absorption and emission of photons by atoms and molecules are studied to probe their energy levels and structure.

In summary, approximation methods and time-dependent quantum mechanics are crucial extensions of basic quantum mechanics that allow us to study more realistic and complex quantum systems and phenomena. These concepts will be further relevant when we discuss relativistic quantum chemistry and its applications.

# Quantum Mechanics Primer

This chapter will provide a primer on quantum mechanics, laying the groundwork for understanding relativistic quantum chemistry. We will cover the fundamental concepts necessary to grasp the quantum phenomena that are crucial in the later chapters.

<a href="01_Basics_of_Relativity.md">前の章: 01 Basics of Relativity</a> | <a href="03_Particle_Physics_and_Atomic_Structure.md">次の章: 03 Particle Physics and Atomic Structure</a>

---
[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)
## 2.1 Wave-Particle Duality

One of the foundational concepts of quantum mechanics is wave-particle duality. This principle states that every quantum entity may be described as both a particle and a wave. 

### 2.1.1 de Broglie Wavelength

Louis de Broglie proposed that particles, like electrons, can exhibit wave-like properties, with a wavelength $\lambda$ related to their momentum $p$ by the de Broglie relation:

$$
\lambda = \frac{h}{p}
$$

where $h$ is Planck's constant. This equation implies that particles with larger momentum have shorter wavelengths, and vice versa.

### 2.1.2 Experimental Evidence

The wave nature of particles has been experimentally confirmed through phenomena like electron diffraction. In the double-slit experiment, electrons, when passed through two slits, create an interference pattern, which is characteristic of waves.

## 2.2 The Schrödinger Equation

The time-dependent Schrödinger equation is the central equation in quantum mechanics that describes how the quantum state of a physical system changes in time.

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

where:
- $i$ is the imaginary unit,
- $\hbar = \frac{h}{2\pi}$ is the reduced Planck's constant,
- $\Psi(\mathbf{r}, t)$ is the wave function, which describes the quantum state of the particle as a function of position $\mathbf{r}$ and time $t$,
- $\hat{H}$ is the Hamiltonian operator, representing the total energy of the system.

For a single particle in a potential $V(\mathbf{r}, t)$, the Hamiltonian is given by:

$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(\mathbf{r}, t)
$$

where $m$ is the mass of the particle and $\nabla^2$ is the Laplacian operator.

### 2.2.1 Time-Independent Schrödinger Equation

For stationary states, where the potential energy is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$
\hat{H}\psi(\mathbf{r}) = E\psi(\mathbf{r})
$$

where:
- $\psi(\mathbf{r})$ is the time-independent wave function,
- $E$ is the energy eigenvalue of the stationary state.

## 2.3 Quantum Operators

In quantum mechanics, physical observables are represented by linear operators acting on the wave function.

### 2.3.1 Position Operator

The position operator $\hat{\mathbf{r}}$ simply multiplies the wave function by the position vector $\mathbf{r}$:

$$
\hat{\mathbf{r}}\psi(\mathbf{r}) = \mathbf{r}\psi(\mathbf{r})
$$

### 2.3.2 Momentum Operator

The momentum operator $\hat{\mathbf{p}}$ is represented in position space as:

$$
\hat{\mathbf{p}} = -i\hbar\nabla
$$

Applying the momentum operator to a wave function gives:

$$
\hat{\mathbf{p}}\psi(\mathbf{r}) = -i\hbar\nabla\psi(\mathbf{r})
$$

### 2.3.3 Energy Operator (Hamiltonian)

As introduced in the Schrödinger equation, the Hamiltonian operator $\hat{H}$ represents the total energy of the system.

### 2.3.4 Angular Momentum Operator

The angular momentum operator $\hat{\mathbf{L}}$ is defined as:

$$
\hat{\mathbf{L}} = \hat{\mathbf{r}} \times \hat{\mathbf{p}}
$$

In Cartesian coordinates, the components are:

$$
\begin{aligned}
\hat{L}_x &= \hat{y}\hat{p}_z - \hat{z}\hat{p}_y \\
\hat{L}_y &= \hat{z}\hat{p}_x - \hat{x}\hat{p}_z \\
\hat{L}_z &= \hat{x}\hat{p}_y - \hat{y}\hat{p}_x
\end{aligned}
$$

## 2.4 Expectation Values

The expectation value of a physical observable $A$, represented by the operator $\hat{A}$, for a system in a state described by the normalized wave function $\Psi$, is given by:

$$
\langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^*(\mathbf{r}, t) \hat{A} \Psi(\mathbf{r}, t) d^3r
$$

For example, the expectation value of the position $\langle \mathbf{r} \rangle$ and momentum $\langle \mathbf{p} \rangle$ can be calculated using their respective operators.

## 2.5 Heisenberg's Uncertainty Principle

Heisenberg's uncertainty principle states that there is a fundamental limit to the precision with which certain pairs of physical properties of a particle, known as complementary variables, can be known simultaneously. For position and momentum, this principle is expressed as:

$$
\Delta x \Delta p_x \geq \frac{\hbar}{2}
$$

where $\Delta x$ and $\Delta p_x$ are the standard deviations of position and momentum in the x-direction, respectively. This principle is not due to limitations in measurement instruments but is inherent in the quantum nature of particles.

This primer provides a basic overview of quantum mechanics. In the following sections and chapters, we will build upon these fundamental concepts to explore more advanced topics in relativistic quantum chemistry.

## 2.6 Quantum Harmonic Oscillator

The quantum harmonic oscillator is a fundamental model in quantum mechanics that describes systems experiencing a restoring force proportional to their displacement from equilibrium. It is used to model molecular vibrations, lattice vibrations in solids, and many other physical systems.

### 2.6.1 Hamiltonian

The Hamiltonian for a one-dimensional quantum harmonic oscillator is given by:

$$
\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2
$$

where:
- $\hat{p}$ is the momentum operator,
- $m$ is the mass of the particle,
- $\omega$ is the angular frequency of the oscillator,
- $\hat{x}$ is the position operator.

### 2.6.2 Energy Eigenvalues

The energy eigenvalues for the quantum harmonic oscillator are quantized and given by:

$$
E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0, 1, 2, \ldots
$$

where $n$ is the quantum number. The lowest energy level, $E_0 = \frac{1}{2}\hbar\omega$, is known as the zero-point energy, which is a purely quantum mechanical phenomenon.

### 2.6.3 Wave Functions

The wave functions for the harmonic oscillator can be expressed in terms of Hermite polynomials. The ground state wave function ($n=0$) is a Gaussian function:

$$
\psi_0(x) = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}
$$

and higher energy wave functions are given by:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

where $H_n(x)$ are the Hermite polynomials.

The quantum harmonic oscillator illustrates key quantum mechanical concepts such as energy quantization and zero-point energy, and it serves as a crucial building block for understanding more complex quantum systems.

## 2.7 Hydrogen Atom

The hydrogen atom, consisting of a single proton and a single electron, is the simplest atom and one of the most important systems in quantum mechanics. It is the only atom for which the Schrödinger equation can be solved analytically, providing a foundation for understanding more complex atoms and molecules.

### 2.7.1 Hamiltonian

The Hamiltonian for the hydrogen atom, neglecting relativistic effects and spin-orbit coupling, is given by:

$$
\hat{H} = -\frac{\hbar^2}{2\mu}\nabla^2 - \frac{e^2}{4\pi\epsilon_0 r}
$$

where:
- $\mu = \frac{m_e m_p}{m_e + m_p}$ is the reduced mass of the electron-proton system,
- $m_e$ is the mass of the electron,
- $m_p$ is the mass of the proton,
- $e$ is the elementary charge,
- $\epsilon_0$ is the vacuum permittivity,
- $r$ is the distance between the electron and the proton.

### 2.7.2 Energy Eigenvalues

The energy eigenvalues for the hydrogen atom are given by the Rydberg formula:

$$
E_n = -\frac{R_y}{n^2}, \quad n = 1, 2, 3, \ldots
$$

where:
- $R_y = \frac{\mu e^4}{8\epsilon_0^2 h^2} \approx 13.6 \text{ eV}$ is the Rydberg constant,
- $n$ is the principal quantum number.

The negative sign indicates that the energy is bound, and $n=1$ corresponds to the ground state, with higher values of $n$ corresponding to excited states.

### 2.7.3 Atomic Orbitals

The wave functions for the hydrogen atom are called atomic orbitals and are described by three quantum numbers:
- Principal quantum number $n$: determines the energy level and can be any positive integer ($n = 1, 2, 3, \ldots$).
- Angular momentum or azimuthal quantum number $l$: determines the shape of the orbital and can range from $0$ to $n-1$. ($l=0, 1, 2, \ldots, n-1$)
- Magnetic quantum number $m_l$: determines the orientation of the orbital in space and can take integer values from $-l$ to $+l$. ($m_l = -l, -l+1, \ldots, 0, \ldots, l-1, l$)

For example, for $n=1$, we have only $l=0$ and $m_l=0$, which corresponds to the 1s orbital. For $n=2$, we have $l=0$ (2s orbital) and $l=1$ (2p orbitals, with $m_l = -1, 0, 1$).

The hydrogen atom solutions provide a crucial foundation for understanding the electronic structure of all atoms and molecules, and the concept of atomic orbitals is fundamental in chemistry.

## 2.8 Spin Angular Momentum

In addition to orbital angular momentum, particles like electrons possess an intrinsic angular momentum called spin angular momentum, or simply spin. Spin is a purely quantum mechanical property with no classical analogue.

### 2.8.1 Spin Quantum Numbers

For electrons, spin angular momentum is quantized and described by two quantum numbers:
- Spin quantum number $s = \frac{1}{2}$ (for electrons, always $\frac{1}{2}$).
- Spin magnetic quantum number $m_s$: can take two values, $m_s = +\frac{1}{2}$ (spin up, $\uparrow$) and $m_s = -\frac{1}{2}$ (spin down, $\downarrow$).

### 2.8.2 Spin Operators

Spin is also associated with operators, analogous to orbital angular momentum operators. The spin operators $\hat{S}^2$, $\hat{S}_x$, $\hat{S}_y$, and $\hat{S}_z$ satisfy similar commutation relations as the orbital angular momentum operators.

### 2.8.3 Total Angular Momentum

The total angular momentum $\hat{\mathbf{J}}$ of an electron in an atom is the sum of its orbital angular momentum $\hat{\mathbf{L}}$ and spin angular momentum $\hat{\mathbf{S}}$:

$$
\hat{\mathbf{J}} = \hat{\mathbf{L}} + \hat{\mathbf{S}}
$$

Total angular momentum is crucial for understanding atomic spectra and magnetic properties, especially in relativistic quantum mechanics where spin-orbit coupling becomes significant.

## 2.9 Approximation Methods

For most quantum mechanical systems, especially those involving multiple particles, solving the Schrödinger equation analytically is impossible. Therefore, approximation methods are essential tools in quantum mechanics to obtain approximate solutions that are sufficiently accurate for practical purposes. We will briefly introduce two common approximation methods: perturbation theory and the variational method.

### 2.9.1 Perturbation Theory

Perturbation theory is used when the Hamiltonian of a system can be written as a sum of an unperturbed Hamiltonian $\hat{H}_0$ for which the solutions are known, and a small perturbation $\hat{H}'$:

$$
\hat{H} = \hat{H}_0 + \lambda\hat{H}'
$$

where $\lambda$ is a dimensionless parameter much smaller than 1. We can then expand the energy eigenvalues and eigenfunctions in powers of $\lambda$.

To first order in perturbation theory, the energy correction is given by:

$$
E_n^{(1)} = \langle \psi_n^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle
$$

and the first-order correction to the wave function is:

$$
| \psi_n^{(1)} \rangle = \sum_{k \neq n} \frac{\langle \psi_k^{(0)} | \hat{H}' | \psi_n^{(0)} \rangle}{E_n^{(0)} - E_k^{(0)}} | \psi_k^{(0)} \rangle
$$

where $E_n^{(0)}$ and $| \psi_n^{(0)} \rangle$ are the eigenvalues and eigenfunctions of the unperturbed Hamiltonian $\hat{H}_0$.

### 2.9.2 Variational Method

The variational method is based on the variational principle, which states that for any trial wave function $\phi$, the expectation value of the Hamiltonian $\hat{H}$ is an upper bound to the true ground state energy $E_0$:

$$
\langle \phi | \hat{H} | \phi \rangle \geq E_0
$$

By minimizing the expectation value of the Hamiltonian with respect to the parameters in the trial wave function, we can obtain an approximation to the ground state energy and wave function.

For example, if we choose a trial wave function $\phi(\alpha)$ that depends on a parameter $\alpha$, we can find the optimal $\alpha$ by minimizing the energy expectation value:

$$
\frac{d}{d\alpha} \langle \phi(\alpha) | \hat{H} | \phi(\alpha) \rangle = 0
$$

The variational method is particularly useful for finding approximate ground state energies and wave functions for complex systems.

## 2.10 Time-Dependent Quantum Mechanics

So far, we have mainly discussed time-independent quantum mechanics and stationary states. However, many phenomena, such as spectroscopy and scattering, require a time-dependent treatment. Time-dependent quantum mechanics describes how quantum systems evolve in time under the influence of time-dependent potentials.

### 2.10.1 Time-Dependent Schrödinger Equation

As introduced earlier, the time-dependent Schrödinger equation is:

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

For a time-dependent Hamiltonian $\hat{H}(t)$, the solutions $\Psi(\mathbf{r}, t)$ describe the time evolution of the quantum system.

### 2.10.2 Time Evolution Operator

The time evolution of a quantum state can be formally described by the time evolution operator $\hat{U}(t, t_0)$, which propagates the state from time $t_0$ to time $t$:

$$
\Psi(t) = \hat{U}(t, t_0)\Psi(t_0)
$$

For a time-independent Hamiltonian, the time evolution operator is given by:

$$
\hat{U}(t, t_0) = e^{-i\hat{H}(t - t_0)/\hbar}
$$

For time-dependent Hamiltonians, the time evolution operator is more complex and often requires numerical methods or approximations to calculate.

### 2.10.3 Transitions and Spectroscopy

Time-dependent quantum mechanics is essential for understanding transitions between quantum states induced by time-dependent perturbations, such as electromagnetic radiation. This is the basis for spectroscopy, where the absorption and emission of photons by atoms and molecules are studied to probe their energy levels and structure.

In summary, approximation methods and time-dependent quantum mechanics are crucial extensions of basic quantum mechanics that allow us to study more realistic and complex quantum systems and phenomena. These concepts will be further relevant when we discuss relativistic quantum chemistry and its applications.

## 2.11 Summary

This chapter has provided a concise introduction to the fundamental principles of quantum mechanics. We began with wave-particle duality and the Schrödinger equation, which are central to describing quantum systems. We then explored quantum operators, expectation values, and Heisenberg's uncertainty principle, which highlight the probabilistic and non-classical nature of quantum mechanics. We also discussed important model systems like the quantum harmonic oscillator and the hydrogen atom, and concepts like spin angular momentum. Finally, we touched upon approximation methods and time-dependent quantum mechanics, which are essential for tackling more complex quantum problems.

These concepts are essential for understanding the behavior of atoms and molecules, especially when relativistic effects become important. In the subsequent chapters, we will delve into relativistic quantum mechanics and its applications in chemistry, building upon the foundation laid in this chapter.

---

[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)

---

# Quantum Mechanics Primer

This chapter will provide a primer on quantum mechanics, laying the groundwork for understanding relativistic quantum chemistry. We will cover the fundamental concepts necessary to grasp the quantum phenomena that are crucial in the later chapters.

[前の章へ](01_Basics_of_Relativity.md) | [次の章へ](03_Particle_Physics_and_Atomic_Structure.md)

## 2.1 Wave-Particle Duality

One of the foundational concepts of quantum mechanics is wave-particle duality. This principle states that every quantum entity may be described as both a particle and a wave. 

### 2.1.1 de Broglie Wavelength

Louis de Broglie proposed that particles, like electrons, can exhibit wave-like properties, with a wavelength $\lambda$ related to their momentum $p$ by the de Broglie relation:

$$
\lambda = \frac{h}{p}
$$

where $h$ is Planck's constant. This equation implies that particles with larger momentum have shorter wavelengths, and vice versa.

### 2.1.2 Experimental Evidence

The wave nature of particles has been experimentally confirmed through phenomena like electron diffraction. In the double-slit experiment, electrons, when passed through two slits, create an interference pattern, which is characteristic of waves.

## 2.2 The Schrödinger Equation

The time-dependent Schrödinger equation is the central equation in quantum mechanics that describes how the quantum state of a physical system changes in time.

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

where:
- $i$ is the imaginary unit,
- $\hbar = \frac{h}{2\pi}$ is the reduced Planck's constant,
- $\Psi(\mathbf{r}, t)$ is the wave function, which describes the quantum state of the particle as a function of position $\mathbf{r}$ and time $t$,
- $\hat{H}$ is the Hamiltonian operator, representing the total energy of the system.

For a single particle in a potential $V(\mathbf{r}, t)$, the Hamiltonian is given by:

$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(\mathbf{r}, t)
$$

where $m$ is the mass of the particle and $\nabla^2$ is the Laplacian operator.

### 2.2.1 Time-Independent Schrödinger Equation

For stationary states, where the potential energy is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$
\hat{H}\psi(\mathbf{r}) = E\psi(\mathbf{r})
$$

where:
- $\psi(\mathbf{r})$ is the time-independent wave function,
- $E$ is the energy eigenvalue of the stationary state.

## 2.3 Quantum Operators

In quantum mechanics, physical observables are represented by linear operators acting on the wave function.

### 2.3.1 Position Operator

The position operator $\hat{\mathbf{r}}$ simply multiplies the wave function by the position vector $\mathbf{r}$:

$$
\hat{\mathbf{r}}\psi(\mathbf{r}) = \mathbf{r}\psi(\mathbf{r})
$$

### 2.3.2 Momentum Operator

The momentum operator $\hat{\mathbf{p}}$ is represented in position space as:

$$
\hat{\mathbf{p}} = -i\hbar\nabla
$$

Applying the momentum operator to a wave function gives:

$$
\hat{\mathbf{p}}\psi(\mathbf{r}) = -i\hbar\nabla\psi(\mathbf{r})
$$

### 2.3.3 Energy Operator (Hamiltonian)

As introduced in the Schrödinger equation, the Hamiltonian operator $\hat{H}$ represents the total energy of the system.

### 2.3.4 Angular Momentum Operator

The angular momentum operator $\hat{\mathbf{L}}$ is defined as:

$$
\hat{\mathbf{L}} = \hat{\mathbf{r}} \times \hat{\mathbf{p}}
$$

In Cartesian coordinates, the components are:

$$
\begin{aligned}
\hat{L}_x &= \hat{y}\hat{p}_z - \hat{z}\hat{p}_y \\
\hat{L}_y &= \hat{z}\hat{p}_x - \hat{x}\hat{p}_z \\
\hat{L}_z &= \hat{x}\hat{p}_y - \hat{y}\hat{p}_x
\end{aligned}
$$

## 2.4 Expectation Values

The expectation value of a physical observable $A$, represented by the operator $\hat{A}$, for a system in a state described by the normalized wave function $\Psi$, is given by:

$$
\langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^*(\mathbf{r}, t) \hat{A} \Psi(\mathbf{r}, t) d^3r
$$

For example, the expectation value of the position $\langle \mathbf{r} \rangle$ and momentum $\langle \mathbf{p} \rangle$ can be calculated using their respective operators.

## 2.5 Heisenberg's Uncertainty Principle

Heisenberg's uncertainty principle states that there is a fundamental limit to the precision with which certain pairs of physical properties of a particle, known as complementary variables, can be known simultaneously. For position and momentum, this principle is expressed as:

$$
\Delta x \Delta p_x \geq \frac{\hbar}{2}
$$

where $\Delta x$ and $\Delta p_x$ are the standard deviations of position and momentum in the x-direction, respectively. This principle is not due to limitations in measurement instruments but is inherent in the quantum nature of particles.

This primer provides a basic overview of quantum mechanics. In the following sections and chapters, we will build upon these fundamental concepts to explore more advanced topics in relativistic quantum chemistry.

## 2.6 Quantum Harmonic Oscillator

The quantum harmonic oscillator is a fundamental model in quantum mechanics that describes systems experiencing a restoring force proportional to their displacement from equilibrium. It is used to model molecular vibrations, lattice vibrations in solids, and many other physical systems.

### 2.6.1 Hamiltonian

The Hamiltonian for a one-dimensional quantum harmonic oscillator is given by:

$$
\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2
$$

where:
- $\hat{p}$ is the momentum operator,
- $m$ is the mass of the particle,
- $\omega$ is the angular frequency of the oscillator,
- $\hat{x}$ is the position operator.

### 2.6.2 Energy Eigenvalues

The energy eigenvalues for the quantum harmonic oscillator are quantized and given by:

$$
E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0, 1, 2, \ldots
$$

where $n$ is the quantum number. The lowest energy level, $E_0 = \frac{1}{2}\hbar\omega$, is known as the zero-point energy, which is a purely quantum mechanical phenomenon.

### 2.6.3 Wave Functions

The wave functions for the harmonic oscillator can be expressed in terms of Hermite polynomials. The ground state wave function ($n=0$) is a Gaussian function:

$$
\psi_0(x) = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}
$$

and higher energy wave functions are given by:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

where $H_n(x)$ are the Hermite polynomials.

The quantum harmonic oscillator illustrates key quantum mechanical concepts such as energy quantization and zero-point energy, and it serves as a crucial building block for understanding more complex quantum systems.

## 2.7 Hydrogen Atom

The hydrogen atom, consisting of a single proton and a single electron, is the simplest atom and one of the most important systems in quantum mechanics. It is the only atom for which the Schrödinger equation can be solved analytically, providing a foundation for understanding more complex atoms and molecules.

### 2.7.1 Hamiltonian

The Hamiltonian for the hydrogen atom, neglecting relativistic effects and spin-orbit coupling, is given by:

$$
\hat{H} = -\frac{\hbar^2}{2\mu}\nabla^2 - \frac{e^2}{4\pi\epsilon_0 r}
$$

where:
- $\mu = \frac{m_e m_p}{m_e + m_p}$ is the reduced mass of the electron-proton system,
- $m_e$ is the mass of the electron,
- $m_p$ is the mass of the proton,
- $e$ is the elementary charge,
- $\epsilon_0$ is the vacuum permittivity,
- $r$ is the distance between the electron and the proton.

### 2.7.2 Energy Eigenvalues

The energy eigenvalues for the hydrogen atom are given by the Rydberg formula:

$$
E_n = -\frac{R_y}{n^2}, \quad n = 1, 2, 3, \ldots
$$

where:
- $R_y = \frac{\mu e^4}{8\epsilon_0^2 h^2} \approx 13.6 \text{ eV}$ is the Rydberg constant,
- $n$ is the principal quantum number.

The negative sign indicates that the energy is bound, and $n=1$ corresponds to the ground state, with higher values of $n$ corresponding to excited states.

### 2.7.3 Atomic Orbitals

The wave functions for the hydrogen atom are called atomic orbitals and are described by three quantum numbers:
- Principal quantum number $n$: determines the energy level and can be any positive integer ($n = 1, 2, 3, \ldots$).
- Angular momentum or azimuthal quantum number $l$: determines the shape of the orbital and can range from $0$ to $n-1$. ($l=0, 1, 2, \ldots, n-1$)
- Magnetic quantum number $m_l$: determines the orientation of the orbital in space and can take integer values from $-l$ to $+l$. ($m_l = -l, -l+1, \ldots, 0, \ldots, l-1, l$)

For example, for $n=1$, we have only $l=0$ and $m_l=0$, which corresponds to the 1s orbital. For $n=2$, we have $l=0$ (2s orbital) and $l=1$ (2p orbitals, with $m_l = -1, 0, 1$).

The hydrogen atom solutions provide a crucial foundation for understanding the electronic structure of all atoms and molecules, and the concept of atomic orbitals is fundamental in chemistry.

## 2.8 Spin Angular Momentum

In addition to orbital angular momentum, particles like electrons possess an intrinsic angular momentum called spin angular momentum, or simply spin. Spin is a purely quantum mechanical property with no classical analogue.

### 2.8.1 Spin Quantum Numbers

For electrons, spin angular momentum is quantized and described by two quantum numbers:
- Spin quantum number $s = \frac{1}{2}$ (for electrons, always $\frac{1}{2}$).
- Spin magnetic quantum number $m_s$: can take two values, $m_s = +\frac{1}{2}$ (spin up, $\uparrow$) and $m_s = -\frac{1}{2}$ (spin down, $\downarrow$).

### 2.8.2 Spin Operators

Spin is also associated with operators, analogous to orbital angular momentum operators. The spin operators $\hat{S}^2$, $\hat{S}_x$, $\hat{S}_y$, and $\hat{S}_z$ satisfy similar commutation relations as the orbital angular momentum operators.

### 2.8.3 Total Angular Momentum

The total angular momentum $\hat{\mathbf{J}}$ of an electron in an atom is the sum of its orbital angular momentum $\hat{\mathbf{L}}$ and spin angular momentum $\hat{\mathbf{S}}$:

$$
\hat{\mathbf{J}} = \hat{\mathbf{L}} + \hat{\mathbf{S}}
$$

Total angular momentum is crucial for understanding atomic spectra and magnetic properties, especially in relativistic quantum mechanics where spin-orbit coupling becomes significant.

## 2.9 Approximation Methods

For most quantum mechanical systems, especially those involving multiple particles, solving the Schrödinger equation analytically is impossible. Therefore, approximation methods are essential tools in quantum mechanics to obtain approximate solutions that

One of the foundational concepts of quantum mechanics is wave-particle duality. This principle states that every quantum entity may be described as both a particle and a wave. 

### 2.1.1 de Broglie Wavelength

Louis de Broglie proposed that particles, like electrons, can exhibit wave-like properties, with a wavelength $\lambda$ related to their momentum $p$ by the de Broglie relation:

$$
\lambda = \frac{h}{p}
$$

where $h$ is Planck's constant. This equation implies that particles with larger momentum have shorter wavelengths, and vice versa.

### 2.1.2 Experimental Evidence

The wave nature of particles has been experimentally confirmed through phenomena like electron diffraction. In the double-slit experiment, electrons, when passed through two slits, create an interference pattern, which is characteristic of waves.

## 2.2 The Schrödinger Equation

The time-dependent Schrödinger equation is the central equation in quantum mechanics that describes how the quantum state of a physical system changes in time.

$$
i\hbar\frac{\partial}{\partial t}\Psi(\mathbf{r}, t) = \hat{H}\Psi(\mathbf{r}, t)
$$

where:
- $i$ is the imaginary unit,
- $\hbar = \frac{h}{2\pi}$ is the reduced Planck's constant,
- $\Psi(\mathbf{r}, t)$ is the wave function, which describes the quantum state of the particle as a function of position $\mathbf{r}$ and time $t$,
- $\hat{H}$ is the Hamiltonian operator, representing the total energy of the system.

For a single particle in a potential $V(\mathbf{r}, t)$, the Hamiltonian is given by:

$$
\hat{H} = -\frac{\hbar^2}{2m}\nabla^2 + V(\mathbf{r}, t)
$$

where $m$ is the mass of the particle and $\nabla^2$ is the Laplacian operator.

### 2.2.1 Time-Independent Schrödinger Equation

For stationary states, where the potential energy is time-independent, we can separate variables and obtain the time-independent Schrödinger equation:

$$
\hat{H}\psi(\mathbf{r}) = E\psi(\mathbf{r})
$$

where:
- $\psi(\mathbf{r})$ is the time-independent wave function,
- $E$ is the energy eigenvalue of the stationary state.

## 2.3 Quantum Operators

In quantum mechanics, physical observables are represented by linear operators acting on the wave function.

### 2.3.1 Position Operator

The position operator $\hat{\mathbf{r}}$ simply multiplies the wave function by the position vector $\mathbf{r}$:

$$
\hat{\mathbf{r}}\psi(\mathbf{r}) = \mathbf{r}\psi(\mathbf{r})
$$

### 2.3.2 Momentum Operator

The momentum operator $\hat{\mathbf{p}}$ is represented in position space as:

$$
\hat{\mathbf{p}} = -i\hbar\nabla
$$

Applying the momentum operator to a wave function gives:

$$
\hat{\mathbf{p}}\psi(\mathbf{r}) = -i\hbar\nabla\psi(\mathbf{r})
$$

### 2.3.3 Energy Operator (Hamiltonian)

As introduced in the Schrödinger equation, the Hamiltonian operator $\hat{H}$ represents the total energy of the system.

### 2.3.4 Angular Momentum Operator

The angular momentum operator $\hat{\mathbf{L}}$ is defined as:

$$
\hat{\mathbf{L}} = \hat{\mathbf{r}} \times \hat{\mathbf{p}}
$$

In Cartesian coordinates, the components are:

$$
\begin{aligned}
\hat{L}_x &= \hat{y}\hat{p}_z - \hat{z}\hat{p}_y \\
\hat{L}_y &= \hat{z}\hat{p}_x - \hat{x}\hat{p}_z \\
\hat{L}_z &= \hat{x}\hat{p}_y - \hat{y}\hat{p}_x
\end{aligned}
$$

## 2.4 Expectation Values

The expectation value of a physical observable $A$, represented by the operator $\hat{A}$, for a system in a state described by the normalized wave function $\Psi$, is given by:

$$
\langle A \rangle = \langle \Psi | \hat{A} | \Psi \rangle = \int \Psi^*(\mathbf{r}, t) \hat{A} \Psi(\mathbf{r}, t) d^3r
$$

For example, the expectation value of the position $\langle \mathbf{r} \rangle$ and momentum $\langle \mathbf{p} \rangle$ can be calculated using their respective operators.

## 2.5 Heisenberg's Uncertainty Principle

Heisenberg's uncertainty principle states that there is a fundamental limit to the precision with which certain pairs of physical properties of a particle, known as complementary variables, can be known simultaneously. For position and momentum, this principle is expressed as:

$$
\Delta x \Delta p_x \geq \frac{\hbar}{2}
$$

where $\Delta x$ and $\Delta p_x$ are the standard deviations of position and momentum in the x-direction, respectively. This principle is not due to limitations in measurement instruments but is inherent in the quantum nature of particles.

This primer provides a basic overview of quantum mechanics. In the following sections and chapters, we will build upon these fundamental concepts to explore more advanced topics in relativistic quantum chemistry.

## 2.6 Quantum Harmonic Oscillator

The quantum harmonic oscillator is a fundamental model in quantum mechanics that describes systems experiencing a restoring force proportional to their displacement from equilibrium. It is used to model molecular vibrations, lattice vibrations in solids, and many other physical systems.

### 2.6.1 Hamiltonian

The Hamiltonian for a one-dimensional quantum harmonic oscillator is given by:

$$
\hat{H} = \frac{\hat{p}^2}{2m} + \frac{1}{2}m\omega^2\hat{x}^2
$$

where:
- $\hat{p}$ is the momentum operator,
- $m$ is the mass of the particle,
- $\omega$ is the angular frequency of the oscillator,
- $\hat{x}$ is the position operator.

### 2.6.2 Energy Eigenvalues

The energy eigenvalues for the quantum harmonic oscillator are quantized and given by:

$$
E_n = \hbar\omega\left(n + \frac{1}{2}\right), \quad n = 0, 1, 2, \ldots
$$

where $n$ is the quantum number. The lowest energy level, $E_0 = \frac{1}{2}\hbar\omega$, is known as the zero-point energy, which is a purely quantum mechanical phenomenon.

### 2.6.3 Wave Functions

The wave functions for the harmonic oscillator can be expressed in terms of Hermite polynomials. The ground state wave function ($n=0$) is a Gaussian function:

$$
\psi_0(x) = \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}}
$$

and higher energy wave functions are given by:

$$
\psi_n(x) = \frac{1}{\sqrt{2^n n!}} \left(\frac{m\omega}{\pi\hbar}\right)^{1/4} e^{-\frac{m\omega x^2}{2\hbar}} H_n\left(\sqrt{\frac{m\omega}{\hbar}}x\right)
$$

where $H_n(x)$ are the Hermite polynomials.

The quantum harmonic oscillator illustrates key quantum mechanical concepts such as energy quantization and zero-point energy, and it serves as a crucial building block for understanding more complex quantum systems.
