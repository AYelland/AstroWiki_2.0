---
banner: "![[particles.jpg]]"
banner_y: 0.55
aliases:
---

> [!key-idea] Equation
> **Energy Generated (per unit volume):**
> $$
>\epsilon_{\rm v} = Q_{\rm nuc} \,  n_{A} \, n_{B} \, \sigma v \left( \frac{1}{1 + \delta_{AB}} \right) \quad \propto \quad Q_{\rm nuc} \,  n_{A} \, n_{B} \, S(E_{0}) \; T_{6}^{-2/3} \, e^{-B T_{6}^{-1/3}}
> $$
> **Energy Generated (per unit mass):** 
> - *used in the [[Stellar Structure#Conservation of Energy]] Stellar Structure Equation*
> $$
> \epsilon_{\rm m} = \frac{\epsilon_{\rm v}}{\rho} \quad \propto \quad Q_{\rm nuc} \, \rho X_{A} \, X_{B} \, S(E_{0}) \; T_{6}^{-2/3} \, e^{-B T_{6}^{-1/3}}
> \hspace{1cm} \text{where} \hspace{1cm} X_{i} \equiv \text{mass fraction}
> $$
> **where** $A \equiv 1$ and $B \equiv 2$
> $$
> T_{6} = \frac{T}{10^{6} \; {\rm K}} \hspace{1.5cm}
> \mathcal{A} = \frac{A_{1} A_{2}}{A_{1} + A_{2}} \hspace{1.5cm}
> B = 42.6 \,\left( Z_{1}^{2} Z_{2}^{2} \,\mathcal{A} \right)^{1/3} \; {\rm keV}
> $$

*What is the energy generation rate (per unit volume) for a given nuclear reaction?* 

$$A + B \longrightarrow C + D$$

If we have two sets of particles ($A\equiv 1$ and $B \equiv 2$), we can create a system to determine the number of interactions these two sets will have that can generate particles $C$ and $D$.

For both particles types, their relative velocity (with respect to each other), $v_{\rm rel} \equiv v$,  will follow a [[Statistical Mechanics#Maxwell-Boltzmann|Maxwellian]] distribution, $f(v)$. Using the kinetic energy relationship $E = \frac{1}{2} \mu v^{2}$, we can express this velocity distribution in terms of energy.

$$f(v) = 4 \pi v^{2} \, \left(\frac{\mu}{2 \pi k_{\rm B} T}\right)^{3/2} \exp \left( - \frac{\mu v^{2}}{2 k_{\rm B} T}  \right)$$
$$\Downarrow$$
$$f(E) = \left(\frac{4 \beta^{3} E}{\pi}\right)^{1/2} \exp \left( - \beta E \right) \hspace{1cm} \text{where} \hspace{1cm} \beta = \frac{1}{k_{\rm B} T}$$

Taking $\sigma(E)$ as the interaction cross section between the two nuclei approaching at energy $E$...

$$
\sigma(E) = \underbrace{\frac{1}{E} \;\exp \left[ - \frac{b}{\sqrt{E}} \right]}_{\text{quantum mechanics}} \; \underbrace{S(E)}_{\text{nuclear physics}}
\hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}[t]
	&b = \frac{1}{2 \epsilon_{0} \hbar} \left(\frac{\mu}{2}\right)^{1/2} Z_{1} Z_{2} e^{2} \\
	\\
	&\textcolor{gray}{S(E) = \text{slow-varying function, empirical}}
\end{aligned}
$$

...we can integrate over the [[Statistical Mechanics#Maxwell-Boltzmann|Maxwell]] distribution for average of all relative velocities.
$$
\begin{align}
	\langle \sigma v \rangle &= \int_{0}^{\infty} \sigma(E) \, v(E) \, f(E) \; \mathrm{d} E \\
	&= \int_{0}^{\infty} \left[ \frac{S(E)}{E} \; e^{- \frac{b}{\sqrt{E}}} \right] \, \left[ \frac{2 E}{\mu} \right]^{1/2} \, \left[ \left(\frac{4 \beta^{3} E}{\pi}\right)^{1/2} e^{- \beta E} \right] \; \mathrm{d} E \\
	&= \sqrt{\frac{8}{\pi \mu (k_{\rm B} T)^{3}}} \int_{0}^{\infty} S(E) \; \underbrace{e^{-E/k_{\rm B} T}}_{\rm decaying} \, \underbrace{e^{- b/\sqrt{E}}}_{\rm growing} \; \mathrm{d} E \\
\end{align}
$$
In this integral, the only significant contribution is near the "Gamow Peak" due to the product of decaying and growing exponentials.

![[gamow_peak.png|align:center|300]]

Therefore, the only negligible range is near $E=E_{0}$ ($E_{0} \gg k_{B} T$) such that we can take $S(E) \simeq S(E_{0})$ and pull it out of the integral.

$$
\begin{align}
	\langle \sigma v \rangle &= \sqrt{\frac{8}{\pi \mu (k_{\rm B} T)^{3}}} \int_{0}^{\infty} S(E) \; e^{-E/k_{\rm B} T} \, e^{- b/\sqrt{E}} \; \mathrm{d} E \\
	&= \sqrt{\frac{8}{\pi \mu (k_{\rm B} T)^{3}}} \, S(E_{0}) \;\underbrace{\int_{0}^{\infty} e^{-E/k_{\rm B} T} \, e^{- b/\sqrt{E}} \; \mathrm{d} E}_{I \, \equiv \, \text{integrand}}
\end{align}
$$

The maximum of this integrand occurs at the effective mean energy ($E_{0}$) for fusion reactions at temperature $T$.
$$
e^{E/k_{\rm B} T} = e^{-b/\sqrt{E}}
\hspace{1cm} \Rightarrow \hspace{1cm} 
E_{0} = \left( \frac{1}{2} b k_{\rm B} T \right)^{2/3} \textcolor{gray}{= 1.22 \; \left( Z_{1}^{2} Z_{2}^{2} \,\mathcal{A}\, T_{6}^{2} \right)^{1/3} \; {\rm keV}} 
$$
$$\hspace{1cm} \text{where} \hspace{1cm}
\mathcal{A} = \frac{A_{1} A_{2}}{A_{1} + A_{2}} 
\quad {\rm and} \quad 
T_{6} = \frac{T}{10^{6} \; {\rm K}}$$
$$\Downarrow$$
$$I_{\rm max} = I(E_{0}) = e^{-3 E_{0} / k_{\rm B} T} \textcolor{gray}{\; = e^{- B T_{6}^{-1/3}} \hspace{1cm} \text{where} \hspace{1cm} B = 42.6 \,\left( Z_{1}^{2} Z_{2}^{2} \,\mathcal{A} \right)^{1/3} \; {\rm keV}}$$

Approximating this distribution as a Gaussian, we can solve this integral by...
$$
\begin{align}
	\int_{0}^{\infty} \left[ e^{-E/k_{\rm B} T} \, e^{- b/\sqrt{E}} \right] \; \mathrm{d} E \; &\simeq \int_{0}^{\infty} I_{\rm max} \exp \left[ - \left(\frac{E - E_{0}}{\Delta E_{0} / 2}\right)^{2} \right] \; \mathrm{d} E \\
	&= I_{\rm max} \int_{0}^{\infty} \exp \left[ - \left(\frac{E - E_{0}}{\Delta E_{0} / 2}\right)^{2} \right] \; \mathrm{d} E \\
	&= I_{\rm max} \left( \sqrt{\frac{\pi}{4}} \, \Delta E_{0} \right) \textcolor{gray}{\hspace{1cm} \text{where} \hspace{1cm} \Delta E_{0} = 4 \sqrt{\frac{E_{0} k_{\rm B} T}{3}}}
\end{align}
$$
$$\Downarrow$$
$$\langle \sigma v \rangle = \sqrt{\frac{2}{\mu}} \left(\frac{\Delta E_{0}}{ (k_{\rm B} T)^{3/2}}\right) \; S(E_{0}) \; \exp \left( - \frac{3 E_{0}}{k_{\rm B} T} \right)$$

Applying this to the two number densities ($n_{A}$ and $n_{B}$), we can find the interaction rate *per volume* between $A$ and $B$. This is known as the **nuclear reaction rate**.

$$r_{AB} = \frac{\text{\# of interactions}}{\text{volume} \times \text{time}} = n_{A} \, n_{B} \, \langle \sigma v \rangle \hspace{1cm} \text{where} \hspace{1cm} (A \ne B)$$

If $A$ and $B$ are the same species of particle, then we need to divide by 2 to avoid double counting the interactions.

$$r_{AB} = n_{A} \, n_{B} \, \langle \sigma v \rangle \, \left(\frac{1}{1 + \delta_{AB}}\right) \hspace{1cm} \text{where} \hspace{1cm} \delta_{AB} = \begin{cases}
1 &{\rm if} \; A = B \\
0 &{\rm if} \; A \ne B
\end{cases}$$

Then, if we take the energy generated in per interaction to be...

$$Q_{\rm nuc} = \text{energy of RHS - energy of LHS} = \left( m_{\rm C} + m_{\rm D} \right) c^{2} - \left( m_{\rm A} + m_{\rm B} \right) c^{2}$$

...we can express the energy generated (per unit volume) as: 

$$
\boxed{\quad \epsilon_{\rm v} = Q_{\rm nuc} \,  n_{A} \, n_{B} \, \langle \sigma v \rangle \left( \frac{1}{1 + \delta_{AB}} \right) \quad \propto \quad Q_{\rm nuc} \,  n_{A} \, n_{B} \, S(E_{0}) \; T_{6}^{-2/3} \, e^{-B T_{6}^{-1/3}}\quad}
$$

> [!sun] Comparison of Burning Processes
>
> Below is a comparison of the main $\ce{^{4}He}$ production processes...
> - [[Proton-Proton Chain]] (PP-Chain)
> 	- Energy generation Rate: $\varepsilon \; \propto \; T^{4}$
> - [[Carbon-Nitrogen-Oxygen Cycle]] (CNO Cycle)
> 	- Energy generation Rate: $\varepsilon \; \propto \; T^{20}$
> - [[Triple-Alpha Process]] (Triple-$\alpha$ Process)
> 	- Energy generation Rate: $\varepsilon \; \propto \; T^{40}$
>
> ![[stellar_nucleosynthesis.svg.png|align:center|500]]
>
> Important Notes:
> - The sun's core temperature is $T_{\rm c, \odot} \approx 1.5 \times 10^{7} \; {\rm K}$.
> 	- In the sun, about $\sim 99 \%$ of the energy produced is through the [[Proton-Proton Chain|pp chain]] while the other $\sim 1 \%$ is produced through the [[Carbon-Nitrogen-Oxygen Cycle|CNO cycle]].
> - The cross over between the [[Proton-Proton Chain|pp chain]] and the [[Carbon-Nitrogen-Oxygen Cycle|CNO cycle]] is at $T \sim 2 \times 10^{7} \; {\rm K}$.
> - [[Triple-Alpha Process|Triple-alpha]] is highly temperature sensitive and explosive. Ignition happens near $T\sim 10^{8}\;{\rm K}$
^nuclearBurning-comparison