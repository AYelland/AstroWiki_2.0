### Question
---
Calculate the approximate distance to the heliopause. Does the local interstellar medium begin at this boundary? Explain.

### Answer
---

> [!space] The Scale of the Solar System
> ![[solarSystem_scale.jpg|align:center]]

##### Calculate the approximate distance to the heliopause.

> [!note]
> The [[Sun#Heliosphere|heliosphere]] is **not spherical**, so the following derivation requires some heavy approximations.

To find the approximate size to of the heliosphere (closest point being the heliopause), we need to balance the [[Sun#Solar Wind|solar wind]] pressure with the [[Interstellar Medium|ISM]] thermal pressure.


**1) Solar Wind Pressure**

The [[Sun#Solar Wind|solar wind]] in the [[Sun#heliosphere]] can be viewed as exerting a [[Fluid Mechanics#Ram Pressure|ram pressure]] on the [[Interstellar Medium|ISM]].

$$
P_{\rm{ram}} = \rho_{\rm sw} v_{\rm n}^{2} \hWhere
\begin{aligned}
	\rho_{\rm sw} \equiv \rho_{\rm sw}(R_{\rm ram})
\end{aligned}
$$

Here, $R_{\rm ram}$ labels the distance from the [[Sun]] to [[Sun#Heliopause|heliopause]], $v_{\rm n}$ is the [[Center of Mass & Relative Coordinates#Relative Position|relative]] velocity of the two bodies, and we use the subscript $X_{\rm sw}$ for [[Sun#heliosphere]] ( or [[Sun#Solar Wind|solar wind]]).

- We approximate the relative velocity ($v_{\rm n}$) by assuming the speed of the [[Sun#Solar Wind|solar wind]] is approximately the same as the particle escape velocity from the surface of the [[Sun]], and by assuming the speed remains constant until reaching the [[Sun#Heliopause|heliopause]]. (Within the [[Sun#heliosphere]], we can treat the [[Interstellar Medium|ISM]] to be at rest.) $$v_{\rm n} \sim v_{\rm esc,\odot} = \sqrt{\frac{2 G M_{\odot}}{R_{\odot}}} \simeq 600 \, {\rm km/s} = 6 \times 10^{5} \; {\rm m/s}$$

- We approximate the mass density ($\, \rho_{\rm sw} \equiv \rho_{\rm sw}(r) \,$) of the [[Sun#Heliosphere|heliosphere]] by assuming the inner-heliospheric medium is composed purely of ionized hydrogen gas. From earth ground-based measurements, we can determine the solar wind density at $r = 1 \; {\rm AU}$. $$\rho_{\rm sw, AU} \simeq n_{\rm AU} \, \mu \, m_{\rm p} \simeq (7 \times 10^{6} \pu{m^{-3}})\, \fpar{1}{2} \, (1.6\times 10^{-27}\,\pu{kg}) \simeq 10^{-21} \; {\rm kg/m^{3}}$$Here, the number density is ($n_{\rm AU} = 6 \times 10^{3} \; {\rm m^{-3}}$), the [[Mean Molecular Weight|mean molecular weight ]] is ($\mu = 1/2$) for purely ionized hydrogen gas, and the hydrogen mass ($m_{\rm H} \approx m_{\rm p}$) is about $1 \; {\rm amu}$.

- Using this solar wind density ($\rho_{\rm sw,AU} = \rho_{\rm sw}(r = 1 \; {\rm AU})$), we can apply [[Stellar Structure#Mass Continuity|mass continuity]] for a spherically symmetric density field to find $\rho_{\rm sw}(r)$ at any radial distance from the sun. $$\td{M}{r} = \left( 4 \pi r^{2} \right) \, \rho(r) = \text{constant} \hRightarrow \rho(r) \propto \frac{1}{r^{2}}$$As a result, we have... $$4 \pi r^{2} \, \rho_{\rm sw}(r) = 4 \pi \, (1 \; {\rm AU})^{2} \, \rho_{\rm sw, AU} \hRightarrow \rho_{\rm sw}(r) = \fpar{1 \; {\rm AU}}{r}^{2} \rho_{\rm sw, AU}$$
**2) ISM Pressure**

The thermal pressure of the [[Interstellar Medium|ISM]] can be modeled as an [[Thermodynamics#Ideal Gas Law|ideal gas]] with pressure 
$$P_{\rm ISM} = n_{\rm ISM} \, k_{\rm B} \, T_{\rm ISM}$$
where we use parameters from the molecular cloud the [[sun]] was presumably formed in *(see [[Interstellar Medium|ISM]])* to determine the number density as ($n_{\rm ISM} \simeq 0.01 \; {\rm cm^{-3}} = 10^{4} \; {\rm m^{-3}}$) and the coronal gas temperature as ($T_{\rm ISM} \simeq 10^{5} \; {\rm K}$). The Boltzmann constant is $k_{\rm B} = 1.38\times 10^{-23} \; \pu{m^2 kg s^{-2} K^{-1}}$.


**3) Equating the Pressures**
$$
\begin{align}
	P_{\rm ram} &= P_{\rm ISM} \\
	\rho_{\rm sw} \, v_{n}^{2} &= n_{\rm ISM} \, k_{\rm B} \, T_{\rm ISM} \\
	\left( \fpar{R_{\rm AU}}{r}^{2} \rho_{\rm sw, AU} \right) \, (v_{\rm \odot, esc})^{2} &= n_{\rm ISM} \, k_{\rm B} \, T_{\rm ISM} \\
	&\Downarrow
\end{align}
$$
$$
\begin{align}
	r &= \left( \sqrt{\frac{\rho_{\rm sw, AU} \, (v_{\rm \odot, esc})^{2}}{n_{\rm ISM} \, k_{\rm B} \, T_{\rm ISM}}} \right) \; {\rm AU} \\
	&\approx \left( \sqrt{(\frac{(10^{-21} \; {\rm kg/m^{3}}) \, (6 \times 10^{5} \; {\rm m/s})^{2}}{(10^{4} \; {\rm m^{3}}) \, (10^{-23} \; \pu{kg m^{2} s^{-2} K^{-1}}) \, (10^{5} \; {\rm K})}} \right) \; {\rm AU} \\
	&\approx 10^{\frac{1}{2}(-21+11-4+23-5)} \; {\rm AU} \\
	&\sim 100 \, {\rm AU}
\end{align}
$$

##### Does the local interstellar medium begin at this boundary? Explain.

![[heliopause.jpg|align:center|500]]

The [[Sun#Heliopause|heliopause]] is the location where pressure between the solar wind and the ISM thermal pressure reaches an equilibrium. Therefore, by definition, the heliopause is the central point of the mixing, meaning that the solar wind extends further into the ISM and the ISM reaches in closer to the Sun. Hence, the heliopause has no clear boundary between the two gaseous species. *(for more information, see [[Sun#Heliopause]])*

> [!note] The Local Bubble
> 
> - The sun is located near the edge of a void in interstellar matter called the **Local Bubble**, which is believed to have resulted from an old supernovae ($\sim 10 - 20 \; {\rm Myr}$ ago)
> 	- $n \sim 0.05 \; {\rm cm^{-3}}$ ($\sim 10 \% \langle n_{\rm ISM} \rangle$ is in the Milky Way)
> 	- Still emitting x-ray radiation
> 
> - Within the Local Bubble, there is:
> 	- Local interstellar cloud (aka local fluff), containing the Sun & solar system with $n\sim 0.3 \; {\rm cm^{-3}}$ 
> 	- G-cloud (contains $\alpha$Centauri)
> 	- Ursa Majr moving group
> 	- Hyades
