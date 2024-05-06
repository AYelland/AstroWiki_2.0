---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - degeneracy pressure
  - Fermi energy
  - Fermi momentum
  - degeneracy
---
Degeneracy pressure and energy can be provided through the **Pauli Exclusion Principle** (only one fermion permitted per quantum state), such that there is a *repulsion* to keep their wave functions from overlapping. 

> [!note]
> In other words, the *repulsion* in the Pauli Exclusion Principle is the kinetic energy of the electrons themselves as they try to expand and to not be on top of each other.

From kinetic theory, we can enforce this rule. Beginning with the phase space density...

$$
f(\vec{r}, \vec{p}) \equiv \frac{\rd N}{\rd^{3} x \, \rd^{3} p} = \frac{g}{h^{3}} \, (n_{\rm occ}) \hWhere 
\begin{aligned}
	n_{\rm occ} &\equiv \text{occupacy number} \\
	g &\equiv \text{degeneracy} = 2 \text{ for fermions} \\
	h &\equiv \text{Plank's Constant}
\end{aligned}
$$

...we will assume some homogenous, isotropic system composed of fermions. (using [[Statistical Mechanics#Fermi-Dirac & Bose-Einstein|Fermi Statistics]]).

$$
f(p) = \frac{g}{h^{3}} \, (n_{\rm occ}) = \frac{2}{h^{3}} \fpar{1}{e^{[E(p) - \mu] / k_{\rm B} T} + 1}
$$

The number density ($\bar{n}_{s}$) and pressure ($P$) are then defined by:

$$
\bar{n}_{s} = \int f(p) \; \rd^{3} p \hspace{2cm} P = \frac{1}{3} \int p \, v f(p) \; \rd^{3} p \hspace{2cm} \textcolor{gray}{s \equiv {\rm particle\ species}}
$$

> [!note] In the classical limit ($n_{\rm occ} \ll 1$), we can find the [[Statistical Mechanics#Maxwell-Boltzmann]] distribution.

With a completely degenerate fermion gas, we will take the Heisenberg Uncertainty Principle to be saturated ($\Delta x \; \Delta p \ge \hbar/2 \implies \Delta x \; \Delta p \sim \hbar$) such that every fermion will fill the lowest possible energy level (or "energy cells") accessible, without violating Pauli's Exclusion Principle.

In a spherical momentum-space shell, we can place two fermions ($g=2$) in each phase-space "energy cell". With this, Pauli's Exclusion Principle gives us a limit on our phase space density...

$$
\fpar{(4 \pi p^{2} \; \rd p) \; \rd^{3} x}{h^{3}} \; {\rm cells} \implies 2 \times \fpar{(4 \pi p^{2} \; \rd p) \; \rd^{3} x}{h^{3}} \; {\rm fermions} \hTherefore 
\underbrace{f(p) \; \rd^{3} p \; \rd^{3} x \; \le  \; \frac{8 \pi p^{2} \; \rd p \; \rd^{3} x}{h^{3}}}_{\text{Pauli's Exclusion Principle}}
$$

...where each cell can only be filled up to a certain maximum momentum (**Fermi Momentum**, $p_{\rm F}$).

$$
f(p) \; \rd^{3} p = \begin{cases}
\frac{8 \pi p^{2} \; \rd p}{h^{3}} &{\rm for} \quad p \le p_{\rm F} \\
0 &{\rm for} \quad p \gt p_{\rm F} \\
\end{cases}
\hWhere p_{\rm F} \equiv \text{Fermi Momentum}
$$

This maximum momentum can be found by integrating the total number fermions over accessible momentum range.

$$
\begin{align}
N_{\rm s} = \bar{n}_{s} \; \rd^{3} x = \rd^{3} x \int_{0}^{p_{\rm F}} &\fpar{8 \pi p^{2}}{h^{3}} \; \rd p = \fpar{8 \pi p_{\rm F}^{3}}{3 h^{3}} \rd^{3} x \\
\\
&\Downarrow \\
\\
\end{align}
$$
$$\boxed{ \; p_{\rm F} = \fpar{3 \bar{n}_{\rm s} h^{3}}{8 \pi}^{1/3} = \left( 3 \pi^{2} \hbar^{3} \bar{n}_{\rm s} \right)^{1/3} \; } \hspace{1cm} \textcolor{gray}{s \equiv {\rm particle\ species}}$$

The **Fermi Energy** is then defined through the kinetic energy with the *Fermi Momentum*.

$$E_{\rm F} = \frac{p_{\rm F}^{2}}{2 m_{\rm s}} \hRightarrow \boxed{ \; E_{\rm F} = \frac{\hbar^{2}}{2 m_{\rm s}} \left(3 \pi^{2} \bar{n}_{\rm s} \right)^{2/3} \;} \hspace{1cm} \textcolor{gray}{s \equiv {\rm particle\ species}}$$
 ## Non-Relativistic

Using the **Fermi Momentum** (defined above), we can now calculate the degeneracy pressure for completely degenerate fermion gas. In a *non-relativistic limit*, we take $v = p/m_{\rm s}$.

$$
\begin{align}
	P_{\rm deg} &= \frac{1}{3} \int p \, v \,f(p) \; \rd^{3} p \\ 
	&= \frac{1}{3} \int_{0}^{p_{\rm F}} p \fpar{p}{m_{\rm s}}^{2} \fpar{8 \pi p^{2}}{h^{3}} \; \rd p \\
	&= \frac{8 \pi}{3 h^{3} m_{\rm s}} \int_{0}^{p_{\rm F}} p^{4} \; \rd p \\
	&= \frac{8 \pi}{15 h^{3} m_{\rm s}} p_{\rm F}^{5} \\
	&= \frac{8 \pi}{15 h^{3} m_{\rm s}} \fpar{3 \bar{n}_{\rm s} h^{3}}{8 \pi}^{5/3} \\
	&= \frac{1}{20} \fpar{3}{\pi}^{2/3} \fpar{h^{2}}{m_{\rm s}} \, \bar{n}_{\rm s}^{5/3} \hRightarrow P_{\rm deg} \propto \bar{n}_{\rm s}^{5/3}
\end{align}
$$
Going a step further, we can express this in terms of total mass density ($\rho$) using the [[Mean Molecular Weight|mean molecular weight]] ($\mu_{\rm s}$) of our fermion species (WD - electrons, NS - neutrons).

$$
\bar{n}_{\rm s} \equiv \frac{\rho}{\mu_{\rm s} m_{\rm p}} \hRightarrow P_{\rm deg} = \underbrace{\frac{1}{20} \fpar{3}{\pi}^{2/3} \fpar{h^{2}}{m_{\rm s} \, (m_{\rm p})^{5/3}}}_{K_{\rm NR}} \, \fpar{\rho}{\mu_{\rm s}}^{5/3} = K_{\rm NR} \, \fpar{\rho}{\mu_{\rm s}}^{5/3}
$$

This is a [[Polytropes|polytrope]] expression with the adiabatic index of $\gamma_{\rm ad} = \gamma = 5/3$ (or polytropic index of $n = 3/2$).

## Ultra-Relativistic

Using the **Fermi Momentum** (defined above), we can now calculate the degeneracy pressure for completely degenerate fermion gas. In a *ultra-relativistic limit*, we take $v = c$.

$$
\begin{align}
	P_{\rm deg} &= \frac{1}{3} \int p \, v \,f(p) \; \rd^{3} p \\ 
	&= \frac{1}{3} \int_{0}^{p_{\rm F}} p \,c \fpar{8 \pi p^{2}}{h^{3}} \; \rd p \\
	&= \frac{8 \pi c}{3 h^{3}} \int_{0}^{p_{\rm F}} p^{3} \; \rd p \\
	&= \frac{2 \pi c}{3 h^{3}} p_{\rm F}^{4} \\
	&= \frac{2 \pi c}{3 h^{3}} \fpar{3 \bar{n}_{\rm s} h^{3}}{8 \pi}^{4/3} \\
	&= \frac{1}{8} \fpar{3}{\pi}^{1/3} (h c) \, \bar{n}_{\rm s}^{4/3} \hRightarrow P_{\rm deg} \propto \bar{n}_{\rm s}^{4/3}
\end{align}
$$
Going a step further, we can express this in terms of total mass density ($\rho$) using the [[Mean Molecular Weight|mean molecular weight]] ($\mu_{\rm s}$) of our fermion species (WD - electrons, NS - neutrons).

$$
\bar{n}_{\rm s} \equiv \frac{\rho}{\mu_{\rm s} m_{\rm p}} \hRightarrow P_{\rm deg} = \underbrace{\frac{1}{8} \fpar{3}{\pi}^{1/3} \fpar{hc}{(m_{\rm p})^{4/3}}}_{K_{\rm UR}} \, \fpar{\rho}{\mu_{\rm s}}^{4/3} = K_{\rm UR} \, \fpar{\rho}{\mu_{\rm s}}^{4/3}
$$

This is a [[Polytropes|polytrope]] expression with the adiabatic index of $\gamma_{\rm ad} = \gamma = 4/3$ (or polytropic index of $n = 3$).

## Condition for Degeneracy

Degeneracy pressure becomes important when...

$$P_{\rm deg} \gtrsim P_{\rm gas} \hRightarrow K_{\rm NR} \fpar{\rho}{\mu_{\rm s}}^{5/3} \gtrsim \frac{\rho k_{\rm B} T}{\mu_{\rm s} m_{\rm p}} \hWhere s \equiv e \equiv {\rm electrons}$$
$$\fpar{\rho}{\mu_{\rm s}} \; \gtrsim \; 730 \, \fpar{T}{10^{7} \; {\rm K}}^{3/2} \; {\rm g/cm^{3}} \hspace{1cm} \text{(for a fully ionized gas)}$$

This condition could also be seen through comparing the **Fermi Energy** to the [[Statistical Mechanics#Energy|average energy of an ideal gas]].
$$
\boxed{\frac{3}{2} k_{\rm B} T  < E_{\rm F}} \hWhere E_{\rm F} = \frac{\hbar^{2}}{2 m_{\rm s}} \left( 3 \pi^{2} \bar{n}_{\rm s} \right)^{2/3} = \frac{\hbar^{2}}{2 m_{\rm s}} \fpar{3 \pi^{2} \rho}{\mu_{\rm s} m_{\rm p}}^{2/3} 
$$
$$\frac{T}{\rho^{2/3}} \lesssim \underbrace{\frac{\hbar^{2}}{2 m_{\rm s} k_{\rm B}} \fpar{3 \pi^{2}}{m_{\rm p}}^{2/3}}_{{\rm constant} \equiv D} \; \fpar{1}{\mu_{\rm s}}^{2/3} \hRightarrow \frac{\rho}{\mu_{\rm s}} \gtrsim \fpar{T}{D}^{3/2}$$