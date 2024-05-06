### Question
---
TESS finds an exoplanet. What can one directly determine from this measurement? What additional observations are needed to determine the mass of this planet?

### Answer
---
##### TESS finds an exoplanet. 

[[Instruments#TESS]] is the ***T**ransiting **E**xoplanet **S**urvey **S**atellite*. (led by George Ricker, MIT)

##### What can one directly determine from this measurement?

From a planetary [[Detection Methods#Transit Method|transit]], (using only [[Instruments#TESS]]) we can measure the ***period*** of the orbit around the host star and the ***size*** of the planetary body.

![[transiting_planet.png|align:center|550]]

**Measuring the Planet's Orbital Period:**

The time between (at least) two consecutively measured transit dips can be measured as the orbital period of the planet around the host star.

**Measuring the Planet's Size:**
*(Source: [Exoplanets, Seager - Winn](https://arxiv.org/pdf/1001.2010.pdf))*

If the planet is without an atmosphere, then we can assume the emission is the same across the whole stellar disk. From this, we can relate area of the stellar disk to observed [[Flux|flux]] of the star before ($F_{\rm b}$) and during ($F_{\rm d}$) the transit through the [[Luminosity|luminosity]] (an intrinsic property of the star).

$$
F_{\rm b} = \frac{L}{4 \pi R_{*}^{2}} \quad , \quad F_{\rm d} = \frac{L}{4 \pi \left(R_{*}^{2} - R_{\rm p}^{2} \right)}
\hRightarrow
\begin{aligned}[t]
	F_{\rm b} \left( 4 \pi R_{*}^{2} \right) &= F_{\rm d} \left( 4 \pi \left(R_{*}^{2} - R_{\rm p}^{2} \right) \right) \\
	\frac{F_{\rm d}}{F_{\rm b}} &= \frac{R_{*}^{2} - R_{\rm p}^{2}}{R_{*}^{2}}
\end{aligned}
$$
$$\delta \equiv \left( 1 - \frac{F_{\rm d}}{F_{\rm b}} \right) = \fpar{R_{\rm p}}{R_{*}}^{2} \equiv \text{percentage change in light-curve}$$

If the planet has an atmosphere, then we assume the atmosphere has an exponential density profile with a constant [[Optical Depth#Optical depth|optical depth]] ($\tau_{\nu}$), an atmospheric scale height ($H$), and a specific number of scale heights ($N_{H}$). Performing the same calculation with a new radius...
$$
R_{\rm p} \; \longrightarrow \; R_{\rm p} + \underbrace{N_{H} H (1 - e^{-\tau_{\nu}})}_{\text{atmosphere height}}
\hWhere \left\{ \;
\begin{aligned}
	H &\equiv \text{atmospheric scale height} = \tfrac{k_{\rm B} T}{\mu g} \\
	\mu &= \text{mean molcular mass} \\
	g &= \text{local gravity on planet} \\
	N_{H} &\equiv \text{number of scale heights} \sim 2\\
	(1 - e^{-\tau_{\nu}}) &\equiv \text{density profile}
\end{aligned} \; \right\}
$$

$$
\delta \equiv \left( 1 - \frac{F_{\rm d}}{F_{\rm b}} \right) = \fpar{R_{\rm p} + N_{H} H (1 - e^{-\tau_{\nu}})}{R_{*}}^{2} 
$$

> [!note] Normalizing the Flux
> For the definition of $\delta$ above (representative of the dip in the light curve) to be correct, one would need to normalize the average flux emitted before the transit to one. In other words, the top-flat part of the light curve should be at 1 such that...
> $$F_{\rm dip} = (1 - \delta) F_{\rm top}$$

> [!bonus]
> 
> - [[Bonus#Bonus - Measuring the Stellar Density]]
> - [[Bonus#Bonus - Measuring the Planet's Temperature]]

##### What additional observations are needed to determine the mass of this planet?

To determine the planet's mass, we need its *radial velocity* ($v_{\rm r}$). This can be measured through a [[Detection Methods#Radial Velocity Method|spectroscopic follow-up]]. *(This can also tell you additional information about the star, allowing you to determine other properties the planetary body.)*

Why does this give you the mass? Once you have the radial velocity, you can use the [[Binary Stars#Spectroscopic Binary|binary mass function]] to find the mass of the planet. Here, I will go through the derivation for this function again...

1) Start by assuming the planet has a circular orbit. 
	- The period of oscillations allow us to replace the orbital radius ($a$) with the **true** orbital velocity ($v$).
		- True velocity can be measured when the orbiting body is moving along the line-of-sight, directly towards or away from us. 
	- The conversion from true velocity to radial velocity is through the inclination angle ($i$)
	- The center of mass of the system gives us the **binary mass ratio**.
$$v = a \omega = a \fpar{2 \pi}{P} \hspace{1.5cm} v = v_{\rm r} \sin i \hspace{1.5cm} \underbrace{M_{*} a_{*} = M_{\rm p} a_{\rm p}}_{\rm center\ of\ mass}$$
$$
a_{*} = v_{*} \fpar{P}{2 \pi} \; , \; a_{\rm p} = v_{\rm p} \fpar{P}{2 \pi}
\begin{aligned}[t]
&\hRightarrow
	\frac{M_{*}}{M_{\rm p}} = \frac{a_{\rm p}}{a_{*}} = \frac{v_{\rm p}}{v_{*}} = \frac{v_{\rm r,p}}{v_{\rm r,*}} \\
	\\
	&\hRightarrow 
	\begin{aligned}[t]
		a = a_{*} + a_{\rm p} &= \fpar{P}{2 \pi} (v_{*} + v_{\rm p}) \\
		&= \fpar{P}{2 \pi} \fpar{v_{\rm r,*} + v_{\rm r,p}}{\sin i}
	\end{aligned}
\end{aligned}
$$
> [!note]
> The circular orbit assumption is not unreasonable given the [[Detection Methods#Transit Method|transit method]] is biased to small orbital radii -- which tend to lead to smaller eccentricities.

2) Use [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] to find the total mass of they star-planet system in terms of the star's mass ($M_{*}$) and the planet's mass ($M_{\rm p}$). 
	- Since we only measure $v_{*,r}$ in practice, we use the mass ratio to express $v_{p,r}$ in terms of the other parameters.
	- This yields an equivalent expression to the **binary mass function**
$$
P^{2} = \frac{4 \pi^{2} a^{3}}{G M} \hRightarrow 
\begin{aligned}[t]
	M_{\rm tot} &= \frac{4 \pi^{2} a^{3}}{G P^{2}} \\
	M_{\rm tot} &= \frac{4 \pi^{2}}{G P^{2}} \fpar{P}{2 \pi}^{3} \fpar{v_{\rm r,*} + v_{\rm r,p}}{\sin i}^{3} \\
	M_{\rm tot} &= \frac{P}{2 \pi G} \fpar{v_{\rm r,*} + v_{\rm r,p}}{\sin i}^{3} \\
	M_{\rm tot} &= \frac{P}{2 \pi G} \fpar{v_{\rm r,*}}{\sin i}^{3} \left( 1 + \frac{v_{\rm r,p}}{v_{\rm r,*}} \right)^{3} \\
	M_{\rm tot} &= \frac{P}{2 \pi G} \fpar{v_{\rm r,*}}{\sin i}^{3} \left( 1 + \frac{M_{*}}{M_{\rm p}} \right)^{3} \\
	v_{\rm r,*}^{3} &= \frac{2 \pi G}{P} \fpar{M_{\rm p}^{3} (M_{*} + M_{\rm p})}{(M_{*} + M_{\rm p})^{3}} \sin^{3} i
\end{aligned}
$$
$$v_{\rm r,*} = \fpar{2 \pi G}{P}^{1/3} \underbrace{\fpar{M_{\rm p} \sin i}{(M_{*} + M_{\rm p})^{2/3}}}_{(\text{binary mass function})^{1/3}}$$

Given we know the radial velocity and stellar mass from the spectroscopic observations, we can solved implicitly for $M_{p}$. 

> [!note]
> There is another version of this derivation where we don't have to assume circular orbits. This results in an addition factor to account for the eccentricity ($\varepsilon$).
> $$
> v_{\rm r,*} = \fpar{2 \pi G}{P}^{1/3} \fpar{M_{\rm p} \sin i}{(M_{*} + M_{\rm p})^{2/3}} \fpar{1}{\sqrt{1 - \varepsilon^{2}}}
> $$

