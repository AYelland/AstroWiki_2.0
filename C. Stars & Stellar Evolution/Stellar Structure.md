---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
---
## Stellar Structure Equations

> [!key-idea] Overview
> There are four major equations that describe the basic structure of a star:
> 1) [[#Mass Continuity]]
> 2) [[#Hydrostatic Equilibrium]]
> 3) [[#Conservation of Energy]]
> 4) [[#Energy Transport]]

### Mass Continuity
*(Also known as the **Mass Profile**)*

$$\frac{\mathrm{d} M_{r}}{\mathrm{d} r} = 4 \pi r^{2} \rho$$
where $M_{r}$ is mass enclosed within a spherical shell of inner radius ($r$), thickness ($\mathrm{d} r$), and density ($\rho$). 

> [!derivation]-
> Consider the following shell of mass...
>
> ![[hydrostatic_equilibrium.png|align:center|300]]
>
>The change in the enclosed mass of a sphere ($\mathrm{d} M_{r}$), with respect to $r$, can be defined by the density ($\rho$) and the change in the enclosed volume ($\mathrm{d} V_{\rm shell}$).
> $$
> \mathrm{d} M_{r} = \rho \, \mathrm{d} V_{\rm shell} = \rho \left( 4 \pi r^{2} \, \mathrm{d} r \right)
> \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\frac{\mathrm{d} M_{r}}{\mathrm{d} r} = 4 \pi r^{2} \rho}
> $$

### Hydrostatic Equilibrium
*(Also known as the **Pressure Profile**)*

$$\frac{\mathrm{d} P}{\mathrm{d} r} = -\frac{G M_{r} \rho}{r^{2}} = -g(r) \rho$$

where $M_{r}$ is mass enclosed within a spherical shell of radius ($r$) and density ($\rho$). The resulting $g(r)$ value is the acceleration due to gravity at $r$.

> [!Derivation]-
> Consider the following shell of mass...
>
> ![[hydrostatic_equilibrium.png|align:center|300]]
>
> We need to balance the collapsing, gravitational force ($\mathrm{d} F_{G}$) and the expanding, gas pressure ($\mathrm{d} F_{P}$) on the two sides of the shell.
> 
> The gravitational force acting on the shell is:
> $$
> \mathrm{d} F_{G} = - \frac{G M_{r} \, \mathrm{d} m}{r^{2}}
> \hspace{1cm} \text{where} \hspace{1cm}
> \mathrm{d} m \equiv \rho \, A \, \mathrm{d} r
> $$
> 
> The gas pressure force acting on the shell is the difference between pressure pushing "down" from the outside and "out" from the inside. We define the minus sign such that $\mathrm{d} F_{P}$ points inward.
> $$
> \mathrm{d} F_{P} = - A \, \mathrm{d} P = - \left( \frac{\mathrm{d} P}{\mathrm{d} r} \right) \, \mathrm{d} r \, A
> $$
> 
> The motion of the shell is then determined by Newton's 2nd Law
> $$
> \sum_{i} \vec{F}_{i} = m \vec{a} = m \, \frac{\mathrm{d}^{2} r}{\mathrm{d} t^{2}} 
> \hspace{1cm} \Rightarrow \hspace{1cm} 
> \mathrm{d} m \, \frac{\mathrm{d}^{2} r}{\mathrm{d} t^{2}} = \mathrm{d} F_{G} + \mathrm{d} F_{P}
> $$
> At equilibirum, the system is static, such that the acceleration is zero. This provides us with the relationship:
> $$\mathrm{d} m \, \underbrace{\frac{\mathrm{d}^{2} r}{\mathrm{d} t^{2}}}_{= 0} = \left[ - \frac{G M_{r} \, \left( \rho \, A \, \mathrm{d} r \right)}{r^{2}} \right] + \left[ - \frac{\mathrm{d} P}{\mathrm{d} r} \, \mathrm{d} r \, A \right]$$
> $$\boxed{\frac{\mathrm{d} P}{\mathrm{d} r} = \frac{G M_{r} \, \rho}{r^{2}}}$$

### Conservation of Energy
*(Also known as the **Luminosity Profile**)*

$$\frac{\mathrm{d} L}{\mathrm{d} r} = 4 \pi r^{2} \rho \, \left[ \varepsilon_{m} - T \frac{\mathrm{d} S}{\mathrm{d} t} \right] \hspace{1cm} \text{where} \hspace{1cm} \varepsilon_{m} = \varepsilon_{n} + \cancelto{0}{\varepsilon_{\nu}}$$
where $L$ is the luminosity of the star producing energy from nuclear reactions at the rate ($\varepsilon_{n}$), temperature ($T$), and specific entropy ($S$) *(i.e. per unit mass)*.

> [!derivation]-
> 
> We can find the conservation of energy by equating total power entering the shell and exiting of the shell, where luminosity is $L(r) = 4 \pi r^{2} F(r)$.
>
> ![[luminosity_profile.png|align:center|300]]
>
> $$\mathrm{d} L  = L(r + \mathrm{d} r) - L(r)$$
> The net power generated from the inside the star can be described by the *energy generation rate per unit mass*, which has the following contributions... 
> - $\varepsilon_{n}$ : energy "produced" through nuclear processes
> - $\varepsilon_{\nu}$ : energy "lost" to escaping neutrinos
> - $\varepsilon_{g}$ : energy "produced" (or "lost") by gravitational expansion (or contraction)
> 
> With the density ($\rho$) and volume of the shell ($\mathrm{d} V_{\rm shell}$), we can define the mass of the shell and determine the change in luminosity with the energy generation rates.
> $$
> \mathrm{d} L = \rho \, \mathrm{d} V_{\rm shell} \, (\varepsilon_{n} - \varepsilon_{\nu} + \varepsilon_{g}) = \rho \, \left( 4 \pi r^{2} \, \mathrm{d} r \right) \, (\varepsilon_{n} - \varepsilon_{\nu} + \varepsilon_{g})
> $$
> Here, we ignore the energy lost to neutrinos ($\varepsilon_{\nu} = 0$), and we use the [[Thermodynamics#2nd Law of Thermodynamics]] to define the energy gained/lost from gravitational expansion/contraction ($\varepsilon_{g}$) as a heating rate ($-\frac{\mathrm{d} Q}{\mathrm{d} t}$).
> $$
> \textbf{2nd Law:} \quad \mathrm{d} Q = T \, \mathrm{d} S \hspace{1cm} \Rightarrow \hspace{1cm} \varepsilon_{g} = -\frac{\mathrm{d} Q}{\mathrm{d} t} = -T \frac{\mathrm{d} S}{\mathrm{d} t}
> $$
> Substituting in these values and rearranging...
> $$
> \mathrm{d} L = \left( \varepsilon_{n} - T \frac{\mathrm{d} S}{\mathrm{d} t} \right) \, 4 \pi r^{2} \rho \, \mathrm{d} r
> \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\frac{\mathrm{d} L}{\mathrm{d} r} = 4 \pi r^{2} \rho \, \left( \varepsilon_{n} - T \frac{\mathrm{d} S}{\mathrm{d} t} \right)}
> $$
> *Note: the last term (the $\varepsilon_{g}$ term) can be negative or positive depending on the heat lost or gained in the shell.*

### Energy Transport
*(Also known as the **Temperature Profile**)*

![[stellar_energy_transport.png|align:center|500]]

Energy can be transported radiatively or convectively, depending on the density and temperature, *(See [[#Schwarzschild Criterion]])*

#### Radiative Energy Transport

$$
\left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm actual} < \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm adiabatic} \hspace{1cm} \Rightarrow \hspace{1cm} 
\frac{\mathrm{d} T}{\mathrm{d} r} = - \frac{3 \kappa_{\rm R}}{64 \pi \sigma} \frac{\rho L}{ r^{2} T^{3}} = -\frac{3 \kappa_{\rm R}}{16 \pi a c}\frac{\rho L}{ r^{2} T^{3}}
$$

where $\sigma$ is the *Stefan-Boltzmann Constant* ($\sigma = \frac{2 \pi^{5} k_{\rm B}^{4}}{15 c^{2} h^{3}}$), $a$ is the *radiation constant* ($a = \frac{4 \sigma}{c}$), and $\kappa_{\rm R}$ is the *[[Optical Depth#Opacity|Rosseland Mean opacity]] of the medium* ($\rho \kappa_{\rm R} = \frac{1}{\ell} = n \sigma = \alpha$)

> [!derivation]-
> 
> Using the temperature to calculate the net flux ($F_{\rm net}$) coming in and out of the shell, we can determine the temperature profile dependent on the thickness of the shell.
>
> ![[temperature_profile.png|align:center|300]]
>
> **Approximate Argument:**
> Assuming the star emits like a blackbody, the net flux can be defined by...
> $$
> F = \sigma T^{4} \hspace{1cm} \Rightarrow \hspace{1cm} F_{\rm net} = \mathrm{d} F = \sigma \left[ T^{4}(r) - T^{4} (r + \Delta r) \right] = - \sigma \frac{\mathrm{d} \left( T^{4} \right)}{\mathrm{d} r} \, \Delta r
> $$
> For $\Delta r$ we use the photon mean-free-path:
> $$
> \Delta r \approx \ell_{\rm ph} = \frac{1}{\alpha} = \frac{1}{\kappa \rho}
> $$
> > [!note] 
> > - If $\Delta r \ll \ell_{\rm ph}$ then $T \approx \text{constant}$.
> > - If $\Delta r \gg \ell_{\rm ph}$ then $F(r) \ne \sigma T^{4}(r)$.
> 
> This brings our net flux to:
> $$
> F_{\rm net} = - \sigma \frac{\mathrm{d} \left( T^{4} \right)}{\mathrm{d} r}  \, \Delta r = - \frac{4 \sigma T^{3}}{\kappa \rho} \frac{\mathrm{d} T}{\mathrm{d} r} = - \frac{a c T^{3}}{\kappa \rho} \frac{\mathrm{d} T}{\mathrm{d} r}
> $$
> Applying the net flux to the Luminosity relationship yields a result that is $3/4$ off from the exact answer.
> $$
> L(r) = 4 \pi r^{2} F(r) \hspace{1cm} \Rightarrow \hspace{1cm} L = - \frac{4 \pi a c r^{2} T^{3}}{\kappa \rho} \frac{\mathrm{d} T}{\mathrm{d} r} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\mathrm{d} T}{\mathrm{d} r} = - \frac{\kappa \rho L}{4 \pi a c r^{2} T^{3}}
> $$
> 
> **Better Argument (Rosseland Mean Opacity):**
> 
> Using the *[[Optical Depth#Opacity|Rosseland Mean Opacity]]* ($\kappa_{\rm R}$), where the flux is defined over a spherically symmetric geometry (instead of a plane parallel geometry)...
> $$
> F_{\rm net} = - \frac{c}{\rho \kappa_{\rm R}} \frac{\mathrm{d} P_{\rm rad}}{\mathrm{d} r} = - \frac{c}{\rho \kappa_{\rm R}} \left( \frac{4}{3} a T^{3} \frac{\mathrm{d} T}{\mathrm{d} r} \right) \hspace{1cm} \text{where} \hspace{1cm} \underbrace{P_{\rm rad} = \frac{1}{3} a T^{4}}_{\text{isotropic blackbody}}
> $$
> ...the Luminosity relationship yields:
> $$
> L(r) = 4 \pi r^{2} F(r) \hspace{1cm} \Rightarrow \hspace{1cm} L = - \frac{4 \pi r^{2} c}{\rho \kappa_{\rm R}} \left( \frac{4}{3} a T^{3} \frac{\mathrm{d} T}{\mathrm{d} r} \right) \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\frac{\mathrm{d} T}{\mathrm{d} r} = -\frac{3 \kappa_{\rm R}}{16 \pi a c}\frac{\rho L}{ r^{2} T^{3}}}
> $$

![[Mnemonics#^e7ef73]]

#### Convective ("Adiabatic") Energy Transport

$$
\left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm actual} \gtrsim \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm adiabatic} \hspace{1cm} \Rightarrow \hspace{1cm} 
\frac{\mathrm{d} T}{\mathrm{d} r} = \left( 1 - \frac{1}{\gamma_{rad}} \right) \frac{T}{P} \frac{\mathrm{d} P}{\mathrm{d} r}
$$

where $\gamma_{rad}$ is the [[Polytropes|polytropic]] exponent. Convection occurs when the temperature gradient is large.

## Schwarzschild Criterion

The Schwarzschild Criterion describes the limits at which convection becomes a more favorable means of energy transport in comparison to radiation.

Consider a parcel of gas in a region of a star with density, pressure, and temperature ($\rho_{1}$, $P_{1}$, $T_{1}$). Now, consider moving that parcel of gas up to a region with a different density, pressure, and temperature ($\rho_{2}$, $P_{2}$, $T_{2}$). 

![[schwarzschild_gasParcels.png|align:center|400]]

Letting ($\rho_{*}$, $P_{*}$, $T_{*}$) represent the properties of the parcel after some displacement ($\Delta r$), we know that...
- If $\rho_{*} < \rho_{2}$, then the parcel will continue to rise causing instability in the system. If this progression continues, the system will begin convection.
- If $\rho_{*} \ge \rho_{2}$, then the parcel will stop rising or sink to the equilibrium point, making the system stable against convection.

To be more explicit in the definition of this limit, we assume that the displacement of the parcel will act on the [[Timescales#Dynamical Timescale|dynamical timescale]] while heat flow will act on the [[Timescales#Thermal Timescale|thermal timescale]], such that the motion of the parcel is adiabatic and the gas is in pressure equilibrium ($P_{1} = P'_{1}$ , $\rho_{1} = \rho'_{1}$ , $P_{2} = P'_{2}$).

This then allows us to use a [[Polytropes|polytropic]] equation of state to relate the density and pressure of the two regions through the adiabatic index ($\gamma_{\rm ad}$).

$$
P = K \, \rho^{\gamma_{\rm ad}} 
\hspace{1cm} \Rightarrow \hspace{1cm} \left\{ \;
\begin{aligned}
	P'_{1} = K \, (\rho_{1}')^{\gamma_{\rm ad}} \\
	P'_{2} = K \, (\rho_{2}')^{\gamma_{\rm ad}}
\end{aligned} \right.
\hspace{1cm} \Rightarrow \hspace{1cm}
\frac{P'_{1}}{P'_{2}} = \left(\frac{\rho'_{1}}{\rho'_{2}}\right)^{\gamma_{\rm ad}} \underbrace{= \frac{P_{1}}{P_{2}}}_{\rm P\ equilibrium}
$$
$$\rho'_{2} = \rho_{1} \left(\frac{P_{2}}{P_{1}}\right)^{1/\gamma}$$

The following mathematical steps are used to convert from working with pressures in favor of working with temperatures.

- Approximate $P_{2}$ in terms of $P_{1}$. $$P_{2} \approx P_{1} + \left. \frac{\mathrm{d} P}{\mathrm{d} r} \right|_{r} \Delta r \hspace{1cm} \Rightarrow \hspace{1cm} \begin{aligned}[t] \rho'_{2} &= \rho_{1} \left(\frac{P_{2}}{P_{1}}\right)^{1/\gamma_{\rm ad}} \\ &\approx \rho_{1} \left( 1 + \frac{1}{P_{1}} \frac{\mathrm{d} P}{\mathrm{d} r} \Delta r \right)^{1/\gamma_{\rm ad}} \\ &\approx \rho_{1} \left( 1 + \frac{1}{\gamma_{\rm ad} P_{1}} \frac{\mathrm{d} P}{\mathrm{d} r} \Delta r \right) \end{aligned}$$
- Approximate $\rho_{1}$ in terms of $\rho_{2}$. $$\rho_{2} \approx \rho_{1} + \left. \frac{\mathrm{d} \rho}{\mathrm{d} r} \right|_{r} \Delta r$$
- Combine together with the condition for stability against convection. $$\begin{align} \rho'_{2} &> \rho_{2} \\ \rho_{1} \left( 1 + \frac{1}{\gamma_{\rm ad} P_{1}} \frac{\mathrm{d} P}{\mathrm{d} r} (\Delta r) \right) &> \rho_{1} + \frac{\mathrm{d} \rho}{\mathrm{d} r} (\Delta r) \\ \frac{\rho_{1}}{\gamma_{\rm ad} P_{1}} \frac{\mathrm{d} P}{\mathrm{d} r} &> \frac{\mathrm{d} \rho}{\mathrm{d} r} \end{align}$$
- Use the [[Thermodynamics#Ideal Gas Law]] to convert pressure into temperature. $$P = \left(\frac{\rho}{\mu m_{\rm p}}\right) k_{\rm B} T \hspace{1cm} \Rightarrow \hspace{1cm} \begin{aligned}[t] \frac{\mathrm{d} \rho}{\mathrm{d} r} &= \frac{\mu m_{\rm p}}{k_{\rm B}} \frac{\mathrm{d} }{\mathrm{d} r} \left(\frac{P}{T}\right) \\ \frac{\rho}{\gamma_{\rm ad} P} \frac{\mathrm{d} P}{\mathrm{d} r} &> \frac{\mu m_{\rm p}}{k_{\rm B}} \left[ \frac{1}{T} \frac{\mathrm{d} P}{\mathrm{d} r} - \frac{P}{T^{2}} \frac{\mathrm{d} T}{\mathrm{d} r} \right] \\ \frac{1}{\gamma_{\rm ad}} \left(\frac{\mu m_{\rm p}}{k_{\rm B} T}\right) \frac{\mathrm{d} P}{\mathrm{d} r} &> \frac{\mu m_{\rm p}}{k_{\rm B}} \left[ \frac{1}{T} \frac{\mathrm{d} P}{\mathrm{d} r} - \frac{P}{T^{2}} \frac{\mathrm{d} T}{\mathrm{d} r} \right] \\ \frac{1}{\gamma_{\rm ad}} \frac{\mathrm{d} P}{\mathrm{d} r} &> \frac{\mathrm{d} P}{\mathrm{d} r} - \frac{P}{T} \frac{\mathrm{d} T}{\mathrm{d} r} \\ \frac{\mathrm{d} T}{\mathrm{d} r} &> \frac{T}{P} \left( 1 - \frac{1}{\gamma_{\rm ad}} \right) \frac{\mathrm{d} P}{\mathrm{d} r} \equiv \left. \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm adiabatic} \end{aligned}$$
The resulting inequality is the **Schwarzschild Criterion** that gives us a condition for stability against convection in terms of temperature.

$$
\left\{ \; 
\begin{alignat}{3}
	&\text{Stable (Radiation):} &\hspace{1cm} \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right| &< \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad} \\
	&\text{Unstable (Convection):} &\hspace{1cm} \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right| &\gtrsim \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad}
\end{alignat}
\; \right\}
\hspace{1cm} \text{where} \hspace{1cm}
\boxed{ \; \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad} = \frac{T}{P} \left( 1 - \frac{1}{\gamma_{\rm ad}} \right) \frac{\mathrm{d} P}{\mathrm{d} r} \; }
$$

> [!space] The Limiting Cases
> The Schwarzschild Criterion tells us that a star is convective when the temperature gradient is large. Let us now examine the [[#Radiative Energy Transport]] equation and look for what physics could lead to large temperature gradients, and thus convective zones: 
> $$
> \left. \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm rad}= - \frac{3 \, \kappa_{\rm R}}{16 \pi a c} \frac{\rho L}{r^{2} T^{3}}
> $$
> $| \mathrm{d} T / \mathrm{d} r |$ is large (and thus convective) when...
> - Large $\kappa_{\rm R}$ , low $T$ $\implies$ convective outer layer of Sun-like stars
> - $L/r^{2} \; \propto \; F$ is large $\implies$ convective cores of very luminous stars
> - $\gamma_{\rm ad}$ small $\implies$ fully convective low mass stars
> 
> ![[stellar_energy_transport.png|align:center|350]]
^schwarzchild-limits
## Mass-Luminosity Relationship

Beginning with the [[#Radiative Energy Transport]] and the [[#Hydrostatic Equilibrium]] relationships...

$$
\begin{alignat}{3}
	\frac{\mathrm{d} T}{\mathrm{d} r} &= - \left(\frac{3 \kappa_{\rm R}}{16 \pi a c}\right) \frac{\rho L}{ r^{2} T^{3}} &\hspace{1cm} \Rightarrow \hspace{1cm} \frac{T}{R} &\propto \frac{\rho L}{ R^{2} T^{3}} \propto \frac{M L}{R^{5} T^{3}} \\
	&&& \\
	\frac{\mathrm{d} P}{\mathrm{d} r} &= -\frac{G M_{r} \rho}{r^{2}} &\hspace{1cm} \Rightarrow \hspace{1cm} \frac{P}{R} &\propto \frac{M \rho}{R^{2}} \propto \frac{M^{2}}{R^{5}}
\end{alignat}
$$

...we can use dimensional analysis to derive a relationship between mass ($M$) and luminosity ($L$), assuming the opacity ($\kappa_{\rm R}$) remains constant and that the star can be represented by an [[Thermodynamics#Ideal Gas Law|ideal gas]].

$$
\underbrace{\; \frac{T}{R} \propto \frac{M L}{R^{5} T^{3}} \;}_{\rm radiation\ transport}
\hspace{2cm} 
\underbrace{\; \frac{P}{R} \propto \frac{M^{2}}{R^{5}} \;}_{\rm hydrostatic\ equilibrium}
\hspace{2cm} 
\underbrace{\; P \propto \frac{M T}{R^{3}} \;}_{\rm ideal\ gas\ law}
$$

Quickly eliminating pressure ($P$), these three relations can be reduced to two.

$$
\underbrace{\; \frac{T}{R} \propto \frac{M L}{R^{5} T^{3}} \;}_{\rm radiation\ transport}
\hspace{2cm} 
\underbrace{\; \frac{M T}{R^{4}} \propto \frac{M^{2}}{R^{5}} \implies T \propto \frac{M}{R} \;}_{\text{ideal gas law} + \text{hydrostatic equilibrium}}
$$

And combining one step further...

$$ 
\frac{T}{R} \propto \frac{M L}{R^{5} T^{3}}
\hspace{1cm} \Rightarrow \hspace{1cm} 
\left(\frac{M}{R}\right)^{4} \propto \frac{M L}{R^{4}}
\hspace{1cm} \Rightarrow \hspace{1cm} 
\boxed{L \propto M^{3}}
$$
