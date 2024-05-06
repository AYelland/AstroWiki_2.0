---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
  - binary
  - binary stars
  - binary star
  - binaries
  - binary system
  - binary systems
---

> [!measure] Typical Parameters and Characteristics
> - About $\sim 50 \%$ of stars in the Milky Way are in binary (or higher) systems
> - Orbital periods range from $\sim 10 \; {\rm min}$ to $\sim 10^{6} \; {\rm yr}$
>	- Mean period of $P \sim 10^{4} \; {\rm day}$ (long tail on distribution)
>- Orbital separation range from $\sim 10^{-3} \; {\rm AU}$ to $\sim 10^{5} \; {\rm AU}$
>	- Mean separation of $a \sim 30 \; {\rm AU}$
>- Large range of eccentricities
>	- For short periods, $\varepsilon \ll 1$ due to tidal circularization
>	- Tidal forces remove/add orbital energy through [[Planetary Migration#Tidal Migration]] while conserving angular momentum

## Types of Binary Systems

### Optical Doubles

![[binary_opticalDouble.png|align:center|550]]

Optical doubles are not actually binary star systems. Instead, they are two stars on the observational/sky plane that appear very close to each other; however, radially are far apart.

### Visual Binary

![[binary_visual.jpeg|align:center|550]]

A binary star system where both stars can be independently resolved by imaging. With high quality observations, we can get precise measurements of the stellar orbits, if the period of the system are not too long.

Seeing a visual binary allows you to make a few assumptions about the system while trying to analyze it.
- The two stars are the same radial distance away from the observer
- The stars almost have same velocity through space - moving center of mass (excluding the orbital motion)

### Astrometric Binary 

![[binary_astrometric.png|align:center|550]]

A binary star system discovered by measuring the "wobble" of a single star, and inferring the existence of the companion.

**Example:** Sirius A/B

### Eclipsing Binary
*(Also known as a **transiting binary**)*

![[binary_ecllipsing.svg|align:center|550]]

A binary star system whose orbit plane almost perpendicular to the observing plane ($i\approx 90 \degree$), such that the light curves from the [[luminosity]] profile can to identify the existence of a secondary body.

**Measurable Quantities from a Light Curve:**
- orbital period ($P$)
- semimajor axis ratio ($a/R_{*}$)
- inclination (how much of the eclipse is passing over the star? partially? fully?)
- temperature
- brightness
- radius of the stars
- presence of additional bodies
- possible orbital decay (inspiraling orbits and [[Planetary Migration#Tidal Migration|tidal migration]])
- is the orbit precessing? ratio of light curves

**Example:** Algol Binary ($P \sim 2.85 \; {\rm day}$)

### Spectroscopic Binary

![[binary_spectroscopic.svg|align:center|550]]

A binary star system identified through Doppler Shifts in the spectral lines due to orbital motion along the line of sight. When observing, the doppler shifted emission is "double-lined", such that the spectral line are composed of two superimposed spectra. Over time, the phase shifts in the two spectra can be observed moving in different directions, allowing us to measure the projected radial velocity curve.

### X-Ray Binary
*(also known as a **Clock Binary**, **Pulsar Binary**)*

![[binary_xray.jpg|align:center|400]]

When one of the stars has a regularly observed x-ray emission/pulsations (pulsars), then temporal deviations of these observations over time can lead to the discovery of a binary system. As the secondary body (without the time-measured pulsation) orbits, the primary star can be shifted closer and further away causing the pulsations to travel less/more before being observed.

The x-rays are generated as matter from the donor star releases gravitational potential energy ($\sim 30 \%$ of rest mass) as it falls into the compact object. The lifetime and the mass-transfer rate in an X-ray binary is dependent on:
- The evolutionary status of the donor star
- The mass ratio between the stellar components
- Their orbital separation.

#### Low Mass X-Ray Binary (LMXB)

A **low-mass X-ray binary (LMXB)** is composed of a [[Black Hole|black hole]] or [[Neutron Star|neutron star]] with a donor star that usually fills its [[#Roche Lobe]] and accretes mass to the compact object. The donor is less massive and younger than the compact object, such that it can be a [[Hertzsprung-Russell Diagram#Main Sequence (MS)|main sequence]], a degenerate dwarf ([[Stellar Classes#White Dwarf|white dwarf]]), or an evolved star ([[Stellar Classes#Red Giant|red giant]]).

Usually formed via capture of a companion or by exchanging places with the less massive member of a binary.

#### Intermediate Mass X-Ray Binary (IMXB)

An **intermediate-mass X-ray binary (IMXB)** is composed of a [[Black Hole|black hole]] or [[Neutron Star|neutron star]]  with an intermediate-mass star.

#### High Mass X-Ray Binary (HMXB)

A **high-mass X-ray binary (HMXB)** is composed of a [[Black Hole|black hole]] or [[Neutron Star|neutron star]]  with a massive star ([[Spectral Classes#O]] or [[Spectral Classes#B]] star, a [[Stellar Classes#Blue Supergiant|blue supergiant]], or in some cases, a [[Stellar Classes#Red Supergiant|red supergiant]] or a [[Stellar Classes#Wolf-Rayet Star]]). 

A fraction of the stellar wind of the massive star is captured by the compact object, and produces X-rays as it falls onto the compact object. This allows the compact object to emit strongly in the X-ray while the massive star emits strongly in the optical. 

Usually formed in star forming regions where the large, hot, short-lived stars can be formed. (i.e. the [[Anatomy of a Galaxy#Galactic Disk]])


### Cataclysmic Variables (CVs)

![[binary_CVs.png|align:center|450]]

A binary star system composed of a [[Stellar Classes#White Dwarf|white dwarf]] and a secondary, donor companion star (typically [[Spectral Classes#G]] star or later). The secondary star accretes matter onto the [[Stellar Classes#White Dwarf|white dwarf]] causing irregularly increases in brightness due to eruptive outbursts called [[Stellar Explosions#Nova|novas]]. After the eruption and increase in brightness, it returns to the initial quiescent state. 

This mass accretion is not enough to exceed the [[Chandrasekhar Limit]] and cause a [[Stellar Explosions#Supernova|supernova]]. All of the [[Stellar Explosions#Nova|nova]] events occur on the surface and don't perturb the star enough to de-structure it.

> [!measure] Typical Parameters
> - Orbital Period: $P\sim 20\,\pu{mins} - 5\,\pu{days}$
> 	- There is a period gap between $\sim 80 - 200 \; {\rm min}$. maybe due to abrupt changes in angular momentum?
> - Average WD Mass: $M_{\rm WD} \sim 0.86 \; {\rm M_{\odot}}$ ($M_{\rm WD} > 0.6 \; {\rm M_{\odot}}$ for isolated white dwarfs)

## Measuring the Masses

### For a [[#Visual Binary]]

![[ellipse.png|align:center|500]]

Using [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] and necessary [[Kepler's Laws of Planetary Motion#Parameters for Orbits|parameters]], we can find the following relations
$$\theta_{1} = \frac{a_{1}}{d} \hspace{1cm} \theta_{2} = \frac{a_{2}}{d} \hRightarrow \frac{m_{1}}{m_{2}} = \frac{\theta_{2}}{\theta_{1}}$$
$$P^{2} = \frac{4 \pi^{2} a^{3}}{G M} = \frac{4 \pi^{2} (\theta \, d)^{3}}{G M} \hWhere M = m_{1} + m_{2}$$

Complications:
1) Need the distance to the system
2) Center of Mass Motion is not constant (it wobbles)
3) The inclination of the orbital plane is non-zero in the sky. So, we observing, we are not observing pure circles about the center of mass

To address this, we introduce the [[Kepler's Laws of Planetary Motion#Parameters for Orbits|Euler Angles]] such that we can measure the projected angles: $\widetilde{\theta}$, $\widetilde{\theta}_{1}$, $\widetilde{\theta}_{2}$ . These are projections of the actual angles onto the plane of the sky.
$$\widetilde{\theta}_{1} = \theta_{1} h(i, \omega, \Omega) \hspace{1cm} \widetilde{\theta}_{2} = \theta_{2} h(i, \omega, \Omega) \hRightarrow \frac{m_{1}}{m_{2}} = \frac{\theta_{2}}{\theta_{1}} = \frac{\widetilde{\theta}_{2} h}{\widetilde{\theta}_{1} h} = \frac{\widetilde{\theta}_{2}}{\widetilde{\theta}_{1}}$$

### For a [[#Spectroscopic Binary]]

![[binary_zShifting.png|align:center|500]]

**If the spectra is "double-lined"...**

When observing the binary system, we can measure the radial velocity of the independents stars through their Doppler Shifts ($\Delta \lambda$) in the non-relativistic limit. If the binary system is inclined ($i \ne 0 \degree$), this allows us to measure these radial displacements such that we can find the true velocity ($v$) through the observed, radial velocity ($v_{\rm r}$).

$$\frac{\Delta \lambda}{\lambda} = \frac{v}{c} \hWhere v_{\rm r} = v \sin(i)$$

If the binary system is face-on ($i = 0 \degree$), then there is no detectable motion.

> [!note] For a receding object, the radial velocity is positive.

With the true velocity measured of both stars ($v_{1}$, $v_{2}$), we can then find the binary mass ratio through the relationship between the velocity and the orbital period.

$$
v_{1} = \omega a_{1} = \frac{2 \pi a_{1}}{P} \hspace{1cm} v_{2} = \omega a_{2} = \frac{2 \pi a_{2}}{P}  
\begin{aligned}[t]
	&\hRightarrow \frac{m_{1}}{m_{2}} = \frac{a_{2}}{a_{1}} = \frac{v_{2}}{v_{1}} = \frac{v_{\rm r,2}}{v_{\rm r,1}} \\
	& \\
	&\hRightarrow a = a_{1} + a_{2} = \frac{P}{2 \pi} \left( v_{1} + v_{2} \right)
\end{aligned}
$$

Here, we can see that the inclination of the system is irrelevant for the binary mass ratio. From [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]], we can then find the total mass for the system.

$$
P^{2} = \frac{4 \pi^{2} a^{3}}{G M} \hRightarrow 
\begin{aligned}[t]
	M = m_{1} + m_{2} &= \frac{4 \pi^{2} a^{3}}{G P^{2}} \\
	&= \frac{P}{2 \pi G} \left( v_{1} + v_{2} \right)^{3} \\
	&= \frac{P}{2 \pi G} \left( \frac{v_{\rm r, 1}}{\sin i} + \frac{v_{\rm r, 2}}{\sin i} \right)^{3} \\
	&= \frac{P}{2 \pi G} \frac{\left( v_{\rm r, 1} + v_{\rm r, 2} \right)^{3}}{\sin^{3} i}
\end{aligned}
$$
$$\boxed{ \; M = \frac{P}{2 \pi G} \frac{\left( v_{\rm r,1} + v_{\rm r,2} \right)^{3}}{\sin^{3} i} \; }$$

**If the spectra is "single-lined"...**

We can  measure $v_{\rm r,1}$, but we cannot measure $v_{\rm r,2}$. Using the mass ratio, we can re-express the velocity of one object into terms of the velocity of the other. Then, we can immediately apply it to our "double-lined" relationships.

$$v_{2} = \fpar{m_{1}}{m_{2}} \, v_{1} = \fpar{m_{1}}{m_{2}} \, \frac{v_{\rm r,1}}{\sin(i)} \hRightarrow M = m_{1}+m_{2} = \frac{P}{2 \pi G} \frac{v_{\rm r,1}^{3}}{\sin^{3}i} \left( 1 + \frac{m_{1}}{m_{2}} \right)^{3}$$

The resulting expression can be re-organized for the **Binary Mass Function**. 

$$
\begin{aligned}[b]
	m_{1}+m_{2} &= \frac{P}{2 \pi G} \frac{v_{\rm r,1}^{3}}{\sin^{3}i} \left( 1 + \frac{m_{1}}{m_{2}} \right)^{3} \\
	m_{1}+m_{2} &= \frac{P}{2 \pi G} v_{\rm r,1}^{3} \fpar{m_{1} + m_{2}}{m_{2} \sin i}^{3} \\
	v_{\rm r,1}^{3} &= \frac{2 \pi G}{P} \frac{(m_{2} \sin i)^{3}}{(m_{1} + m_{2})^{2}} \\
	v_{\rm r,1} &= \fpar{2 \pi G}{P}^{1/3} \underbrace{\fpar{m_{2} \sin i}{(m_{1} + m_{2})^{2/3}}}_{f \equiv (\text{binary mass function})^{1/3}} = \frac{2 \pi a_{1} \sin i}{P}
\end{aligned}
$$
$$
\boxed{f(m_{1}, m_{2}) \equiv \frac{(m_{2} \sin i)^{3}}{(m_{1} + m_{2})^{2}} = \frac{4 \pi^{2} (a_{1} \sin i)^{3}}{G P^{2}} = \fpar{P}{2 \pi G}  v_{\rm r,1}^{3}} \hRightarrow G \Omega f = v_{\rm r,1}^{3}
$$

The left-hand-side is the relationship between masses, while the right-hand-side is computed from purely observables. 

This function represents the minimum companion mass ($m_{2} \ge f(m)$) in a binary star system, given that $i \in \left[ 0, \pi/2 \right]$ such that $\sin i \in \left[ 0 , 1 \right]$.

$$
f = \frac{(m_{2} \sin i)^{3}}{(m_{1} + m_{2})^{2}} \hRightarrow m_{2}^{3} = \frac{f (m_{1} + m_{2})^{2}}{\sin^{3} i} \gt \frac{f \, m_{2}^{2}}{\sin^{3} i} \ge f \, m_{2}^{2} \hRightarrow \boxed{\, m_{2} \gt f(m_{1}, m_{2}) \,}
$$

> [!note] This is also re-derived in [[Question 8]] using a stellar mass $m_{1} \equiv M_{*}$) and a planetary mass ($m_{2} \equiv M_{\rm p}$).


## Binary Evolution


![[binary_evolution.png|align:center]]


## Roche Lobe

In a binary system with a circular orbit, we can describe the system in a coordinate system that rotates along with the objects. 

In this non-inertial frame, one must consider...
- The gravitational contribution from the primary mass ($M_{1}$)
- The gravitational contribution from the secondary mass ($M_{2}$)
- The centrifugal force of the rotating frame

Together, the effective potential on a test mass ($m$) describes the **Roche Potential**, where the binary masses ($M_{1}$ , $M_{2}$) fall along equipotential surfaces.

![[binary_rochePotential.png|align:center|400]]

$$
\Phi_{\rm roche} \equiv \Phi_{\rm eff} = \left( - \frac{G M_{1} m}{\left| \vec{r} - \vec{r}_{1} \right|} \right) + \left( - \frac{G M_{2} m}{\left| \vec{r} - \vec{r}_{2} \right|} \right) + \left( -\frac{1}{2} \Omega^{2} \left| \vec{r} - \vec{r}_{\rm CoM} \right|^{2} \right)
$$

where

$$
\left\{\begin{aligned}
	a &= a_{1} + a_{2} \\
	M_{1}& a_{1} = M_{2} a_{2} \\
\end{aligned} \right\}
\hRightarrow
a_{1} = \fpar{M_{2}}{M_{1}} a_{2} = \fpar{M_{2}}{M_{1}} \left( a - a_{1} \right) = \fpar{\mu}{M_{1}} a
$$

$$
\vec{r} = \left(x, \, y, \, z \right) 
\hspace{2cm} 
\vec{r}_{1} = \left(0, \, 0, \, 0 \right) 
\hspace{2cm} 
\vec{r}_{2} = \left(a, \, 0, \, 0 \right) 
\hspace{2cm} 
\vec{r}_{\rm CoM} = \big( \underbrace{\tfrac{\mu}{M_{1}} a}_{a_{1}}, \, 0, \, 0 \big)
$$

Close to each binary mass, surfaces of equal gravitational potential are approximately spherical and concentric. Far from the stellar system, the equipotentials are approximately ellipsoidal and elongated, parallel to the axis joining the mass centers. 

The first common equipotential intersects itself at the L1 [[Lagrange Points|Lagrange Point]] of the system, forming a two-lobed figure-of-eight with the binary masses at the center of each lobe. This critical equipotential defines the **Roche Lobes**. 

When an object has a radius greater than or equal to the size of its Roche Lobe, it will undergo **Roche Lobe Overflow (RLOF)**, where any material outside the Roche Lobe either escape the system completely, orbit both stars, or fall onto the binary companion by transferring matter through the inner L1 [[Lagrange Points|Lagrange Point]].

> [!note] Roche Lobe, Sphere, and Limit?
> The Roche Lobe is different from the Roche Sphere and the Roche Limit(see [[Question 48#Define the Roche limit.|48]]), though all named after the same Édouard Roche.
> 
> **Roche Lobe** - the teardrop-shaped region around an astronomical body in a binary system, within which orbiting material is gravitationally bound.
> 
> **Roche Sphere** - the gravitational sphere of influence of one astronomical body in the face of perturbations from a more massive body that it orbits. 
> 
> **Roche limit** - the distance at which an object held together only by gravity begins to break up due to tidal forces. 
