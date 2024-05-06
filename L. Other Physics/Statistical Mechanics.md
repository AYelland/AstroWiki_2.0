---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
## Classical Limit

When the number of particles becomes very large ($N \gg 1$), all probabilities take on a Guassian distribution.
$$N \gg 1 \hRightarrow \bar{n}_{s} \ll 1 \hspace{0.5cm} , \hspace{0.5cm} e^{\beta H} \gg 1$$

## Equipartition Energy

The principle of equipartition states, *"In a system in thermal equilibrium, on the average, an equal amount of energy will be associated with each degree of freedom."*

## Ensembles

### Microcanonical

To determine the number of microstates ($\Omega$) in a system, we have to use a variety of counting methods. Many of them involve using the *combinations* and *permutations* formulas.
$$\ce{_{r}C_{n}} = \begin{pmatrix} n \\ r \end{pmatrix} = \frac{n!}{r! \, (n - r)!} \hspace{2cm} \ce{_{r}P_{n}} = \frac{n!}{(n - r)!}$$
The probability distribution function (PDF) is then:
$$
p(\mu) = \frac{1}{\Omega} \;  
\begin{cases}
	1 & \text{if } E = E_{\mu} \\
	0 & \text{otherwise}
\end{cases}
$$

### Maxwell-Boltzmann
*(Also known as the **Canonical Distribution**)*

**Maxwell-Boltzmann Statistics** describes a system containing a large number of identical non-interacting, non-relativistic classical particles in thermodynamic equilibrium. *(Only valid when the temperature is high enough or the particle density is low enough to render quantum effects negligible.)*

**Single Partition Function:**$$Z_{1} = e^{- \beta H} \quad\hWhere \beta \equiv \frac{1}{k_{\rm B} T}$$
**Partition Function:**$$Z = \frac{1}{N!} \left( Z_{1} \right)^{N} = \sum_{\mu}^{N} e^{- \beta H_{\mu}}$$
**Probability Distribution Function (PDF):**$$p(\mu) = \frac{1}{Z} e^{- \beta H_{\mu}} \hRightarrow p(v)  = \left[ \frac{m}{2 \pi k_{\rm B} T} \right]^{3/2} \exp\left( - \frac{m v^{2}}{2 k_{\rm B} T} \right)$$
**Average Number Density:**$$\bar{n}_{s} = \sum n_{s} p(\mu_{s}) = - \frac{1}{\beta} \pd{\ln(Z)}{E_{s}} \hRightarrow \bar{n}_{\rm s} = g_{\rm s} \fpar{m_{\rm s} k_{\rm B} T}{2 \pi \hbar^{2}}^{3/2} \exp \left( - \frac{m_{\rm s} c^{2}}{k_{\rm B} T} \right)$$

### Fermi-Dirac & Bose-Einstein
*(Also known as the **Quantum Canonical Distribution**)*

The **Fermi-Dirac Statistics** ($+$) should be used when dealing with non-interacting, identical particles that obey the Pauli exclusion principle. Specifically, this applies to fermions - particles with odd, half-integer spins.

The **Bose-Einstein Statistics** ($-$) should be used when dealing with non-interacting, identical particles that do not obey the Pauli exclusion principle. Specifically, this applies to bosons - particles with integer spins.

> [!note] 
> In the following equations, the *Fermi-Dirac* distributions are represented by choosing the **+** signs. Similarly, the *Bose-Einstein* distributions are represented by choosing the **-** signs.

**Single Partition Function:**$$Z_{1} = \left( 1 \pm e^{- \beta H} \right)^{\pm 1}$$
**Partition Function:**$$Z = \prod_{i}^{N} Z_{1}$$
**Average Number Density:**$$\bar{n}_{s} = \left( e^{\beta H} \pm 1 \right)^{-1}$$

## Partition Function Relationships
Where $\Omega$ is the number of microstates, $Z$ is the partition function, and $\mathcal{Z}$ is the Gibb's partition function...

**Entropy using Microcanonical Ensemble:**$$S = k_{\rm B} \ln \Omega$$
**Helmholtz Free Energy:**$$F = - k_{\rm B} T \, \ln(Z)$$
**Gibbs Free Energy:**$$G = - k_{\rm B} T \, \ln(\mathcal{Z})$$

## Expectation Values and Canonical Pairs

### Canonical Pairs

For any set of canonical pairs $\left\{ \, (T ,S) \, , \, (J, x) \, , \, (\mu, N) \, , \, \dots \, (\mathcal{O}_{1}, \mathcal{O}_{2}) \, \right\}$, we can calculate the averages of any of the powers by following the pattern...

$$
\begin{aligned}
	\langle \mathcal{O}_{1} \rangle_{c} &= - \frac{1}{\beta} \pd{\ln(Z)}{\mathcal{O}_{2}} \\
	\langle \mathcal{O}_{1}^{2} \rangle_{c} &= - \frac{1}{\beta} \pd{\langle \mathcal{O}_{1} \rangle_{c}}{\mathcal{O}_{2}} \\
	\langle \mathcal{O}_{1}^{3} \rangle_{c} &= - \frac{1}{\beta} \pd{\langle \mathcal{O}_{1}^{2} \rangle_{c}}{\mathcal{O}_{2}} \\
	&\dots
\end{aligned}
\hspace{1cm} \underbrace{\Leftrightarrow}_{\text{flip the negative}} \hspace{1cm}
\begin{aligned}
	\langle \mathcal{O}_{2} \rangle_{c} &= - \frac{1}{\beta} \pd{\ln(Z)}{\mathcal{O}_{1}} \\
	\langle \mathcal{O}_{2}^{2} \rangle_{c} &= - \frac{1}{\beta} \pd{\langle \mathcal{O}_{2} \rangle_{c}}{\mathcal{O}_{1}} \\
	\langle \mathcal{O}_{2}^{3} \rangle_{c} &= - \frac{1}{\beta} \pd{\langle \mathcal{O}_{2}^{2} \rangle_{c}}{\mathcal{O}_{1}} \\
	&\dots
\end{aligned}
$$

### Energy

For the average energy to the $n^{th}$ power...
$$\langle E^{n} \rangle_{c} = (-1)^{n} \pd{^{n} \ln (Z)}{\beta^{n}}$$
If dealing with a...
$$
\begin{alignat}{6}
	&\textbf{Monatomic Gas:} \hspace{1cm}& 3 \text{ trans d.o.f.} &+ 0 \text{ rot d.o.f.} &= 3 \text{ d.o.f.} &\hRightarrow \langle E \rangle &= 3 \, (\tfrac{1}{2} k_{\rm B} T) = \tfrac{3}{2} k_{\rm B} T \\
	&\textbf{Diatomic Gas:} \hspace{1cm}& 3 \text{ trans d.o.f.} &+ 2 \text{ rot d.o.f.} &= 5 \text{ d.o.f.} &\hRightarrow \langle E \rangle &= 5 \, (\tfrac{1}{2} k_{\rm B} T) = \tfrac{5}{2} k_{\rm B} T \\
	&\textbf{Polyatomic Gas:} \hspace{1cm}& 3 \text{ trans d.o.f.} &+ 3 \text{ rot d.o.f.} &= 5 \text{ d.o.f.} &\hRightarrow \langle E \rangle &= 6 \, (\tfrac{1}{2} k_{\rm B} T) = 3 k_{\rm B} T \\
\end{alignat}
$$