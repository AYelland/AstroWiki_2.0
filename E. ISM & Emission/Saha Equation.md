---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
The **Saha Equation** uses the Boltzmann factor to calculate the ratio of the particle's population in some specific ionized state to the population in the next ionized state (i.e. after losing one electron) based on their relative energies in a gas at equilibrium. 

$$\frac{n_{r+1}}{n_{r}} = \left(\frac{g_{e} \, g_{r+1}}{g_{r}}\right) \left(\frac{n_{Q,e}}{n_{e}}\right) \,e^{-\chi_{r} / k_{\rm B} T} \hspace{1cm} \text{where} \hspace{1cm} n_{Q,e} \equiv \left(\frac{2 \pi m_{e} k_{\rm B} T}{h^{2}}\right)^{3/2}$$
or
$$\frac{n_{r+1}}{n_{r}} = \left(\frac{g_{e}\,g_{r+1}}{g_{r}}\right) \left(\frac{1}{\lambda^{3} \, n_{e}}\right) \,e^{-\chi_{r} / k_{\rm B} T} \hspace{1cm} \text{where} \hspace{1cm} \lambda \equiv \left(\frac{h^{2}}{2 \pi m_{e} k_{\rm B} T}\right)^{1/2}$$

where 
- $n_{r}$ is the number density of atoms in the $r^{th}$ ionization state, that is with $r$ electrons removed.
- $n_{e}$ is the electron number density
- $n_{Q,e}$ is the quantum number density (related to the de Broglie wavelength, $\lambda$)
- $g_{e}$ is the free electron degeneracy $= 2 (\tfrac{1}{2}) + 1 = 2$
- $g_{r}$ is the degeneracy of states for the $r$-ions (see below)
- $\chi_{r} = \left( \epsilon_{r+1} - \epsilon_{r} \right)$ is the ionization energy required to remove the next electron from the ion
- $m_{e}$ is the mass of an electron $\sim 10^{-32} \; {\rm kg}$
- $T$ is the temperature of the gas
- $h$ is Planck's constant $\sim 6 \times 10^{-34} \; {\rm J \, Hz^{-1}}$
- $\lambda$ is the thermal de Broglie wavelength for the electron (for $k_{\rm B}$ Boltzmann's constant)

>[!note] Comparison to the Boltzmann Equation
>
> The [[Saha Equation]] relates the ionization levels while the [[Boltzmann Equation]] distribution deals with the energy levels.

> [!derivation]-
> 
> Beginning with [[Statistical Mechanics#Fermi-Dirac & Bose-Einstein|Fermi-Dirac & Bose-Einstein Statistics]], the particle number density in phase space is defined as...
> 
> $$
> \frac{\mathrm{d} N}{\mathrm{d}^{3}x \, \mathrm{d}^{3}p} = \frac{g}{h^{3}} \left(\frac{1}{e^{(E-\mu)/k_{\rm B}T} \pm 1}\right)
> \hspace{1cm} \text{where} \hspace{1cm}
> \begin{aligned}
> 	h &\equiv \text{Planck's constant} \\
> 	h^{3} &\equiv \text{volume in phase space} \\
> 	g &\equiv \text{statistcal weight/degeneracy} \\
> 	\mu &\equiv \text{chemical potential} \\
> \end{aligned}
> $$
> 
> We integrate over this phase space while making two approximations:
> 1) The particles are in a non-relativistic regime $\implies E = \frac{p^{2}}{2 m} + m c^{2}$
> 2) The population can be represented by [[Statistical Mechanics#Maxwell-Boltzmann]] distribution, such that we can neglect the $\pm 1$.
> 
> $$\begin{align}
> 	n &= \int \frac{\mathrm{d} N}{\mathrm{d}^{3} x \, \mathrm{d}^{3} p} \\
> 	&= \frac{4 \pi g}{h^{3}} \int_{0}^{\infty} p^{2} \, e^{-(E-\mu)/k_{\rm B}T} \; \mathrm{d} p \\
> 	&= \frac{4 \pi g}{h^{3}} e^{\mu / k_{\rm B} T} e^{- m c^{2} / k_{\rm B} T} \int_{0}^{\infty} p^{2} e^{-p^{2}/2 m k_{\rm B} T}\; \mathrm{d} p \\
> 	&= \frac{g}{h^{3}} \left( 2 \pi m k_{\rm B} T \right)^{3/2} e^{(\mu - m c^{2}) / k_{\rm B} T}
> \end{align}$$
> $$\exp \left[ \frac{\mu - m c^{2}}{k_{\rm B} T} \right] = \frac{1}{g} \left(\frac{n}{n_{\rm Q}}\right) \hspace{1cm} \text{where} \hspace{1cm} n_{\rm Q} \equiv \left(\frac{2 \pi mk_{\rm B} T}{h^{2}}\right)^{3/2}$$
> 
> Here, we define the quantum density ($n_{\rm Q}$). It is directly correlated with the thermal DeBroglie wavelength ($\lambda$), such that we can use it to determine with degeneracy effects become important.
> 
> $$\lambda \equiv n_{\rm Q}^{-1/3} \hspace{1cm} \Rightarrow \hspace{1cm}\lambda  = \sqrt{\frac{h^2}{2 \pi \,m_{\rm e} k_{\rm B} T}}$$
> 
> We now use thermodynamics to write the chemical potential ($\mu$) in terms of other quantities, for a specific particles species ($i$).
> 
> $$\mu_{i} = m_{i} c^{2} + k_{\rm B} T \; \ln \left( \frac{1}{g_{i}} \frac{n_{i}}{n_{Q,i}} \right) = \left( \frac{\partial U}{\partial n_{i}} \right)_{S,V}$$
> 
> For a chemical reaction in thermal equilibrium, we know that...
> 
> $$
> \begin{alignat}{3}
> 	A + B &\; \longleftrightarrow \; C + D\\
> 	\mu_{A} + \mu_{B} &\; \longleftrightarrow \; \mu_{C} + \mu_{D}
> \end{alignat}
> $$
> *(If coefficients, they also follow the reaction directly. (i.e. $2 A + B \to 2 \mu_{A} + \mu_{B}$ ))*
> 
> Specifically, we are interested in the ionization chemical reaction for some element $X$ in the $r^{th}$ state of ionization, such that $r$ electrons are lost.
> 
> $$p + e^{-} \; \longleftrightarrow \; H + \gamma \hspace{1cm} \Rightarrow \hspace{1cm} X_{r+1} + e^{-} \; \longleftrightarrow X_{r} + \gamma$$
> 
> With $\chi_{r}$ representing the **energy necessary to remove the next electron** from the $X_{r}$ ion, the chemical potential balance equation becomes:
> 
> $$\mu_{r+1} + \mu_{e} = \mu_{r} + \cancelto{0}{\mu_{\gamma}}$$
> $$m_{r+1} c^{2} + m_{e} c^{2} + k_{\rm B} T \left[ \ln \left( \frac{1}{g_{r+1}} \frac{n_{r+1}}{n_{Q,r+1}} \right) + \ln \left( \frac{1}{g_{e}} \frac{n_{e}}{n_{Q,e}} \right) \right] = m_{r} c^{2} + k_{\rm B} T \left[ \ln \left( \frac{1}{g_{r}} \frac{n_{r}}{n_{Q,r}} \right) \right]$$
> $$\underbrace{m_{r+1} c^{2} + m_{e} c^{2} - m_{r} c^{2}}_{\left( m_{r+1} \, c^{2} \right) + \left( m_{e} \, c^{2} \right) = \left( m_{r}\, c^{2} \right) + \chi_{r}} = k_{\rm B} T \, \ln \left( \frac{g_{e} \, g_{r+1}}{g_{r}} \frac{n_{r}}{n_{r+1} n_{e}}  \frac{n_{Q,r+1} n_{Q,e}}{n_{Q,r}} \right)$$
> $$\chi_{r} = k_{\rm B} T \, \ln \left( \frac{g_{e} \, g_{r+1}}{g_{r}} \frac{n_{r}}{n_{r+1} n_{e}}  \frac{n_{Q,r+1} n_{Q,e}}{n_{Q,r}} \right)$$
> $$e^{-\chi_{r} / k_{\rm B} T} = \left(\frac{g_{r}}{g_{e} \, g_{r+1}}\right) \left(\frac{n_{r+1} n_{e}}{n_{r}}\right) \left(\frac{n_{Q,r}}{n_{Q,r+1} n_{Q,e}}\right)$$
> $$\frac{n_{r+1}}{n_{r}} = \left(\frac{g_{e} \, g_{r+1}}{g_{r}}\right) \underbrace{\left(\frac{n_{Q,r+1}}{n_{Q,r}}\right)}_{\approx 1} \left(\frac{n_{Q,e}}{n_{e}}\right) \,e^{-\chi_{r} / k_{\rm B} T}$$
> $$\boxed{ \; \frac{n_{r+1}}{n_{r}} = \left(\frac{g_{e} \, g_{r+1}}{g_{r}}\right) \left(\frac{n_{Q,e}}{n_{e}}\right) \,e^{-\chi_{r} / k_{\rm B} T} \; } \hspace{1cm} \text{where} \hspace{1cm} n_{Q,e} \equiv \left(\frac{2 \pi m_{e} k_{\rm B} T}{h^{2}}\right)^{3/2}$$
> 
> If we replace the statistical weight / degeneracy ($g_{r}$) with the partition function ($Z_{r}$), then we can express this relation as:
> 
> $$Z_{r} = \sum_{s} g_{r,s} \; e^{-(E_{r,s} - E_{r,0})/k_{\rm B} T}$$
> $$\boxed{ \; \frac{n_{r+1}}{n_{r}} = \left(\frac{Z_{e} \, Z_{r+1}}{Z_{r}}\right) \left(\frac{n_{Q,e}}{n_{e}}\right) \,e^{-\chi_{r} / k_{\rm B} T} \; } \hspace{1cm} \text{where} \hspace{1cm} n_{Q,e} \equiv \left(\frac{2 \pi m_{e} k_{\rm B} T}{h^{2}}\right)^{3/2}$$

If only the first excited state matters and $r$ represents the ground state, then $n_1 = n_e$ and defining the total non-electron density $n = n_0 + n_1$ we have $$\frac{n_{e}^{2}}{n - n_{e}} = \frac{2}{\lambda^{3}} \frac{g_{1}}{g_{0}} \, \exp \left[-\frac{\chi_{0}}{k_{\rm B} T}\right]$$for first ionization energy $\chi_{0}$.

On the degeneracy of states $g$, here is a quick reference table:
$$\begin{align}
\text{ionization of hydrogen:} \quad \chi_{0} = 13.54 \; {\rm eV}, \quad g_{e} \, g_{i+1} / g_{i} = 1 \\
\text{first ionization of helium:} \quad \chi_{0} = 24.48 \; {\rm eV}, \quad g_{e} \, g_{i+1} / g_{i} = 4 \\
\text{second ionization of helium:} \quad \chi_{1} = 54.17 \; {\rm eV}, \quad g_{e} \, g_{i+1} / g_{i} = 1
\end{align}$$
^degeneracies

**Limitations:**
The Saha equation is only applicable when...
- the system is in thermodynamic equilibrium
- the pressure is not too high ($n_{e} \ll n_{\rm Q}$), so pressure ionization and degeneracy pressure can be neglected
- Simple elemental composition, since more species complicate the picture.

**Use in Stellar Structure:**
- The stellar spectrum is directly correlated to its relative atomic abundance and elemental composition, because each atom or ion can absorb or emit radiation of a particular set of wavelengths.
- The strength of those lines is strongly dependent on temperature (because the relative populations of ionization and atomic energy levels depends on temperature).
	- The Saha Equation tells us the relative populations of ionization levels, and for the simplest inference, what fraction of atoms are not ionized
	- The [[Boltzmann Equation]] (ratio of Boltzmann factors) tell us relative populations of those un-ionized atomic energy levels *(see [[Spectral Features#Hydrogen Spectra]])*
- As a result, the presence and strength of lines used to [[Spectral Classes|classify stars]] are effectively a classification of composition and temperature.

> [!example]
> For example, the Saha equation explains why the [[Spectral Features#Balmer Series]] is seen most strongly in [[Spectral Classes#A]] stars. Hydrogen transitions from a [[Interstellar Medium#Atomic Hydrogen|neutral]] to [[Interstellar Medium#Ionized Hydrogen|ionized]] state around $T \sim 10^{4} \; {\rm K}$. Using the [[Boltzmann Equation]], we see that most hydrogen is in the $n=2$ state around this temperature. So, if an electron is captured by a hydrogen nuclei, it will transition from some higher $n$ state to $n=2$, and thus, the [[Spectral Features#Balmer Series]].
> *(see [[Question 78]])*

![[spectral_line_strengths.png|align:center|600]]