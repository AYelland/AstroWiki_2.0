---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - gravitational waves
  - GW
---
## Sources of Gravitational Waves

Gravitational waves originate from *any accelerating mass with a [[#Gravitational Radiation|quadrupole]] moment, and hence, a change in the quadruple.*

**The are 4 Classification of Gravitational Waves:**

1. Compact Binary Inspiral/Coalescence (CBI/CBC)
	- Binary [[Black Hole]] (BBH) - BH+BH Merger
	- Binary [[Neutron Star]] (BNS) - NS+NS Merger
	- Binary [[Neutron Star]]-[[Black Hole]] (NSBH) - NS+BH Merger
	- [[Stellar Classes#White Dwarf]] Binaries (WD+WD, WD+NS, WD+BH)
		- Undetected: too low of energy/frequency for current detectors
	- [[Black Hole#Supermassive Black Hole]] Binaries
		- Undetected: will be detectable with [[Instruments#LISA]] or [[Instruments#Pulsar Timing Arrays|PTAs]] *(See [[#Gravitational Wave Spectrum]])*
	- Extreme Mass-Ratio Inspiral ([[EMRI.jpg|EMRI]])
		- Undetected: will be detectable with [[Instruments#LISA]]
2. Continuous
	- Isolated, rotating [[Neutron Star|Neutron Stars]] with spherical asymmetry (e.g. "mountains" on the surface)
		- Undetected: the effect would only give a very weak signal at roughly a constant frequency (very hard measurement)
3. Stochastic
	- Primordial Gravitational Waves (fluctuations near big bang)
		- Analogous to the [[Cosmic Microwave Background|CMB]] in that it make a stochastic background on whole sky
	- Unresolved Merger events
	- More likely to be detected via [[Instruments#Pulsar Timing Arrays|PTAs]]. GW signal will be correlated across pulsar signals, but noise will not be. ([[Instruments#NANOGrav]] made a detection)
1. Burst
	- Asymmetric [[Stellar Explosions#Supernova]] or [[Fast Radio Burst#Long GRBs]]
		- If emitting GWs, then they can't be spherically symmetric
	- GW signal from such sources currently unclear, but probably "bursty"

## Gravitational Radiation
*([Source](https://www.astro.umd.edu/~miller/teaching/astr498/lecture24.pdf ))*

Similar to how an [accelerating point charge will emit electromagnetic radiation](https://physics.stackexchange.com/questions/65339/how-and-why-do-accelerating-charges-radiate-electromagnetic-radiation), an accelerating mass *with a quadruple moment* will emit **gravitational radiation.**

> [!atom] Electromagnetic Radiation
> With electromagnetic radiation (change is charge or magnetic moment with respect to time) can only be emitted with a dipole moment or higher. This can be seen with a given charge density ($\rho_{e}(r)$) that we expand into the moments.
> - The charge **monopole** moment is $\int \rho_{e}(r) \mathrm{d}^{3} r$. It represents the total charge ($Q$), which cannot vary. *(conserved in time)*.
> 	- *Electromagnetic monopole radiation is not possible.* 
> - The **electric dipole** moment is $\int r \, \rho_{e}(r) \mathrm{d}^{3} r$. There is no applicable conservation law. *(not conserved in time)*
> 	- *Electric dipole radiation is possible.* 
> - Using the variation of currents, the lowest order correction probes the **magnetic dipole**, represented by $\int r \left[ \rho_{e}(r) \times v(r) \right] \mathrm{d}^{3} r$. There is no applicable conservation law. *(not conserved in time)*
> 	- *Magnetic dipole radiation is possible.* 
> 	- The lower order moments will typically dominate the field unless their variation is reduced or eliminated by some special symmetry.

Gravitational radiation (change in mass with respect to time) can only be emitted from a quadrupole moment or higher. This can be seen with a given mass density ($\rho(r)$) that we expand into the moments.

- The mass **monopole** is $\int \rho_{e}(r) \mathrm{d}^{3} r$. It represents the total mass-energy in the system, which is constant. *(conserved in time)*
	- *Mass monopole radiation is not possible.*
- The mass **dipole** is $\int r \, \rho_{e}(r) \mathrm{d}^{3} r$. It represents the [[Center of Mass & Relative Coordinates|center-of-mass]] energy of a system, and in the center-of-mass references frame, this moment does not change as it effectively is a one-body problem. *(conserved in time)*
	- *Mass dipole radiation is not possible.*
	- The existence of radiation is frame-independent, the lack of radiation in the center-of-mass frame means there is no radiation in any other reference frame
- The equivalent of the **magnetic dipole** moment is $\int r \left[ \rho(r) \times v(r) \right] \mathrm{d}^{3} r$. This, however, is simply the total angular momentum of the system, which is also conserved in the center-of-mass frame.
	- *There is no magnetic dipolar (equivalent) gravitational radiation.*
- The mass **quadruple** moment is $I_{ij} = \int \rho(r) \, r_{i} r_{j} \, \mathrm{d}^{3} r$. This is the moment of inertia, which is not conserved in time.
	- *Mass quadruple radiation is possible*

As a result, the mass **quadruple** -- and higher -- is the first/lowest order contribution to gravitational radiation.

> [!note] The Equations...
> For a discrete system of $\ell$ point masses (or charges) each with mass $m_{\ell}$ (or charge $q_{\ell}$) and position $\mathbf{r}_{\ell } = \left( r_{x \ell}, r_{y \ell}, r_{z \ell} \right)$ relative to the coordinate system origin, the components of the moment of inertia tensor ($Q$) are defined by:
> 
> $$I_{ij} \equiv Q_{ij} = \sum _{\ell} m_{\ell} \left( 3 \, r_{i,\ell} \, r_{j,\ell} - \left\| \mathbf{r}_{\ell} \right\|^{2} \delta_{ij} \right)$$
> 
> The indices $(i,j)$ run over the Cartesian coordinates $(x,y,z)$ and $\delta _{ij}$ is the Kronecker delta. 
> 
> **The Gravitational Potential Energy:**
> 
> $$V_{\text{q}} (\mathbf{R}) = - {\frac{G}{2 |\mathbf{R}|^{3}}} \sum_{i,j} Q_{ij} \, \hat{R}_{i} \hat{R}_{j}$$
> 
> **The Radiation of Gravitational Waves:**
> 
> $$L_{\rm GW} \equiv \frac{\mathrm{d} {E}_{\rm GW}}{\mathrm{d} t} = \frac{G}{5 c^{5}} \left\langle \dddot{I}^{ij} \dddot{I}_{ij} \right\rangle$$
> 
> ---
> If we look at the specific case of a **binary black hole** system, we can use a pair of equal point masses ($M_{1} = M_{2} = M$) on a circular orbit (place origin at center-of-mass). This yields the quadruple tensor of...
> 
> $$I_{ij} = M \left( 3 x_{i} x_{j} - \left\| \mathbf{x} \right\|^{2} \delta_{ij} \right) = \frac{1}{2} \mu R^{2} \begin{bmatrix} 1 + \cos 2 \omega t & \sin 2 \omega t & 0 \\ \sin 2 \omega t & 1 - \cos 2 \omega t & 0  \\ 0 & 0 & 0 \end{bmatrix}$$
> 
> ...where $\omega \equiv$ orbital frequency, $R \equiv$ , and $\mu \equiv$ reduced mass.
^mass-quadruple

## Standard Siren
*(Source: [here](https://www.preposterousuniverse.com/blog/2017/10/16/standard-sirens/))*

A **Standard Siren** is a gravitational wave event that has observed electromagnetic follow-up.

The simultaneous observation of gravitational and electromagnetic waves is crucial to making an independent measurement of the [[Hubble]]. (see [[Hubble#Standard Sirens|here]] for details)

## Chirp Mass

The **chirp mass** of a compact binary system determines the leading-order orbital evolution of the system as a result of energy loss from emitting gravitational waves. Because the gravitational wave frequency is determined by orbital frequency, the chirp mass also determines the frequency evolution of the gravitational wave signal emitted during a binary's inspiral phase.

$$M_{\rm c} = \frac{(M_{1} M_{2})^{3/5}}{(M_{1} + M_{2})^{1/5}} = \frac{(M_{1} M_{2})^{3/5}}{M_{\rm tot}^{1/5}} = \mu^{3/5} M_{\rm tot}^{2/5}$$

For equal masses $M_{*} = M_{1} = M_{2}$, the chirp mass can be reduced to $M_c = M_{*}/2^{1/5} \simeq 0.9\,M_{*}$.

> [!note] Degeneracy with Redshift
> We note that chirp mass experiences a degeneracy with [[Redshift|redshift]]. 
> 
> What is actually derived from the observed gravitational waveform is the product $M_{c,\rm{eff}} = M_{c}(1+z)$. To break this degeneracy one must also obtain the cosmological redshift (dominant to other sources of redshifting).

## Chirp Frequency & Scaling Amplitude

![[Question 43#Give a qualitative description of the frequency and amplitude evolution of the gravitational wave signal from a binary compact star system.]]

## Sticky Bead Argument

> [!cian] 
> Feyman's argument (1957) to support the idea that gravitational waves carry energy. The argument is that for a rigid rod with two beads sliding on it (with friction), and a gravitational wave passing over the rod with a frequency much less than the sound speed in the rod, the GW will not have an effect on the rod that cant be "corrected" by the atomic bonds in the rod, and the beads will have a net translation along the rod, and thus due to friction the GW will have imparted energy onto the rod. I'll be honest though I dont think I get it. I would assume this explanation is flawed.

## Mass-Weighted Effective Spin
*(Also known as the **effective inspiral spin parameter**)*

This **mass-weighted effective spin parameter** ($\chi_{\rm eff}$) qualifies the impact of the spins on the rate of inspiral, and where the binary plunges together to merge. *(See [source](https://cplberry.com/2017/06/01/gw170104/#GW170104-properties).)*

$$
\chi_{\mathrm{eff}} = \frac{M_1 \vec{a}_1 + M_2 \vec{a}_2}{M_1 + M_2}\, \cdot \, \vec{L} \quad
$$

where $\vec{L}$ is the orbital angular momentum of the binary.

$\chi_{\rm eff}$ can range from -1 to +1.
- If $\chi_{\rm eff} = +1$ , then both black holes are spinning as fast as possible and rotate in the same direction as the orbital motion
- If $\chi_{\rm eff} = -1$ , then both black holes spinning as fast as possible but in the opposite direction to the way that the binary is orbiting. 
- If $\chi_{\rm eff} = 0$ , then the black holes are not spinning, their rotation axes are in the orbital plane (instead of aligned with the orbital angular momentum), or one black hole is aligned with the orbital motion and the other is anti-aligned. In all situations, their effects cancel out.

## Effective Precession Spin

The **effective precession spin parameter** ($\chi_{\rm p}$) qualifies the amount of precession, the way that the orbital plane and black hole [spins wobble](http://www.youtube.com/watch?v=S2vp7iVWrkE "YouTube: Simulation of GW170104") when they are not aligned. It is 0 for no precession, and 1 for maximal precession.


## Gravitational Wave Spectrum

![[GW_spectrum_withDetectors.jpg]]