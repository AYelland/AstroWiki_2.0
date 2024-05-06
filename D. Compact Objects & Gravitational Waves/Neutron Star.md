---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - neutron star
  - NS
  - neutron stars
  - Neutron Stars
---
*(A Good (simple) Introduction to Neutron Stars: [Youtube](https://www.youtube.com/watch?v=oLoLey75i2k&ab_channel=ScienceClicEnglish))***

A **neutron star** is a stellar remnant from a massive star ($M \sim 8 - 20 \; {\rm M_{\odot}}$) that has undergone a [[Core-Collapse|core-collapse]] [[Stellar Explosions#Supernova|supernova]]. It is physically supported through neutron [[Degeneracy Pressure|degeneracy pressure]] such that gravity can no longer compress the star further. 

During the collapse, through angular momentum conservation (?), the compact core increases its spin and generates a powerful magnetic field. This field leads to developing the neutron star subtypes including [[#Pulsar|pulsars]], [[#Magnetar|magnetars]], and [[Binary Stars#X-Ray Binary|XRBs]].

> [!measure] Typical Parameters
> - Mass: $M\sim 1 - 2 \; {\rm M_{\odot}}$ (often quoted as $1.4 \; {\rm M_{\odot}}$)
> - Radius: $R \sim 10 \; {\rm km} = 10^{4} \; {\rm m}$
> - Density: $\rho \lesssim 3 \times 10^{17} \; {\rm kg/m^{3}}$ (in core)
> - Magnetic field: $B \sim 10^{4} - 10^{8} \; {\rm T}$ 
> - Period: $P \sim 1.4 - 30 \; {\rm s}$
> 
> For $R \lesssim 9 \; {\rm km}$, the core of the neutron star acts as one giant nucleus because its density $\sim$ atomic nucleus density. (Nuclear Saturation Density of an Atom: $\rho \sim 2 \times 10^{17} \; {\rm kg / m^{3}}$). This is because the strong force interactions are very important here.
^typical-parameters

> [!cian] Random:
> - *Do we have a good idea for what the mass evolution looks like?* 
> 	- Maybe no?
> - *Why don't we see lots of neutron star merger/collisions?* 
> 	- Neutron stars don't have enough mass to dynamically "sink" towards the center of galaxies in the same way that black holes do. We expect black holes to merge in galactic centers, but neutron stars to stay "out". Therefore, they have a lower chance of interacting.

## Structure
*([AstroBites](https://astrobites.org/2017/10/05/nuclear-pasta-in-neutron-stars/))*

![[NS_densities.png|align:center|500]]

![[NS_anatomy+pasta.png|align:center|550]]

A neutron star has a very thin crust, some regions of "nuclear pasta", & superfluid neutron core.

- [[Degeneracy Pressure]] arises because neutrons (and electrons, protons) are fermions, and by the *Pauli Exclusion Principle* they can not occupy the same quantum state. 
- Lots of neutrons in a highly-dense region means [[Degeneracy Pressure|Fermi level]] (next "available" energy state) is actually very high, leading to an additional "pressure" that prevents the core from collapsing further. 
- Neutron degeneracy pressure is not by itself sufficient to maintain an object beyond $0.7\,M_\odot$ , and repulsive nuclear forces play a larger role in supporting more massive neutron stars.

Most of the basic models for these objects imply that neutron stars are composed almost entirely of neutrons; the electrons and protons present in normal matter combine to produce neutrons at the conditions in a neutron star through *neutronization*. Because electrons are fermions, unless an energy $E_F − m_e c^2$ is added to an electron, it is not possible to put the electron in the region of high density, since all the lower energy states are filled. If this energy becomes larger than $(m_n−m_p−m_e)c^2$, it becomes energetically favorable for the electron to combine with a proton to produce a neutron, rather than to exist as a free electron (assuming that neutrons are non-degenerate and a neutron can be created at the lowest energy state). Since $E_F$ increases with density, there is a critical density above which the electrons start combining with protons to give neutrons. At density well above the critical density, matter would mainly consist of neutrons. *(See [[Question 41]])*.

> [!note] **Size of Neutron Star Approximation:**
> For a relativistic neutron degenerate core, we can use the DeBroglie wavelength for a good approximation for how separated the neutrons are. Relating this to number density and mass density...
> 
> $$\lambda_{\rm D} = \frac{h}{m_{\rm n} c^{2}} \hRightarrow N \simeq \fpar{R}{\lambda_{\rm D}}^{3} \sim \fpar{1.4 \; M_{\odot}}{m_{\rm n}} \sim 10^{57}$$
> $$R \simeq \frac{N^{1/3}}{\lambda_{\rm D}} \simeq \frac{h N^{1/3}}{m_{\rm n} c} \sim 12 \; {\rm km}$$

## Types of Neutron Stars

![[NS_types.jpg|align:center]]

### Pulsar
*(**PULSA**ting **R**adio source)*

|     ![[NS_pulsar_axis.jpg\|230]]      |       ![[NS_lighthouse.gif\|400]]       |
| :-----------------------------------: | :-------------------------------------: |

A **pulsar** is a highly-magnetized neutron star that emits beams of EM radiation from the poles along its magnetic axis. These beams can only be observed when they are pointing directly at the observer. Given the pulsar's magnetic field axis is misaligned with the geometric spin axis of the neutron star, these beams appear like a lighthouse with two bulbs as one or both of the beams (if aligned fortunately) pass over Earth periodically.

> [!measure] Typical Parameters
> Same (roughly) as [[Neutron Star#^typical-parameters|neutron star]] with the following additions.
> - Period: $P \sim 0.01 - 10 \; {\rm s}$
> 	- Peak $\sim 0.5 \; {\rm s}$
> - Rate of Change in Period: $\dot{P} \sim 10^{-21} - 10^{-10}$
> 	- Peak $\sim 10^{-15}$ (dimensionless)
> - Peak Frequency: $\nu \sim 300 \; {\rm Hz} \implies \lambda \sim 10^{6} \; {\rm m}$ (low [[Electromagnetic Spectrum|radio]])

**Properties:**
- Born with millisecond periods
- Highly coherent, strongly polarized emission
- They require rapid rotation and strong magnetic field, meaning a pulsar must be a compact object
	- [[Stellar Classes#White Dwarf|WD]]: surface pulsation period (or maximum spin) is too slow $(t \simeq t_{\rm dyn} \sim (G \rho)^{1/2} \sim {\rm seconds})$
	- [[Black Hole|BH]]: Nothing to anchor coherent EM pulsations to
	- [[Neutron Star|NS]]: Best candidate by elimination
- Most of the beams emit in radio, but some detected in x-ray, gamma-ray, and other EM bands
	- Brightest at low frequencies
	- The x-ray emission originates from the surface of the NS, and never fully fades away in the spectra due to the large gravitational well (photons wrap around the NS)
- Isolated (not in binary) pulsars spin down due to EM back reaction

**Origin & Formation:**
- In rotation-powered pulsars, the beam is the result of the rotational energy of the neutron star.
- As the strong magnetic field moves, it generates a large electric field, inducing the acceleration of charged particles (electrons) on the star surface.
- They are then funneled out of the magnetic poles along the magnetic field lines.
- As the charged particles then curl around the magnetic field lines, the emit light through relativistic synchrotron radiation.
- This leads to the creation of the electromagnetic jet (charged matter + light) emanating from the magnetic poles.
	- The light continues to propagate in a straight line to the observer.
	- The charged matter is deflects along other electromagnetic field lines before reaching the observer. (this contributes to the cosmic ray population)
- As more energy is emitted, the rotation slows down until the pulsar evolves past the "death line" on the [[#P-Pdot Diagram]].
- After this, they no longer pulsate.

> [!note]- Rotational "Glitches"
> 
> Usually $\dot{P} > 0$ such that the pulsar is slowing down; however, occasionally, a young pulsar will have sudden, sharp spin-up events followed by an exponential return to the earlier spin-down trend. 
> 
> ![[NS_pulsar_glitch.png|align:center|350]]
> 
> This is thought to be caused by a sudden rearrangement of the internal moment of inertia, leading to spin-up to conserve angular momentum. 
> 
> The charged component of the crust couples to magnetic field, causing the crust to spin down. Then, there is weak intermittent coupling to the core, causing the spin-up episodes. This effect is only seen in young stars as they "settle" after collapse.

![[NS_pulsar_accretion_lightCylinder.png|align:center|500]]

> [!tip] Other References on Pulsars and their Subclasses
> - X-Ray Pulsar Mechanism: [[xray_pulsars.pdf|Walter+Ferrigno, 2017]], [[Question 63]]
> - Millisecond Pulsar: [[Question 53]]
> - First Binary Pulsar: [[Question 56]]
> - Rotational Energy Loss: [[Question 62]]
> - Accretion Spin-Up Rate: [[Question 64]]
> - Magnetospheric Radius: [[Question 64]]
> - Sites for Pulsars (Globular Clusters): [[Question 65]]
> - Magnetic Field Strength: [[Question 70]]

#### Millisecond Pulsar (MSP)

A **millisecond pulsar (MSP)** is a pulsar with a very short rotation period ($P \lesssim 10 \; {\rm ms}$) that are thought to be "spun up"/"recycled" through accretion from a companion star in a close binary ([[Binary Stars#Low Mass X-Ray Binary (LMXB)|LMXB]]?).

![[NS_pBplot_MSPs.png|align:center]]

1. An isolated or non-accreting pulsar will spin down over time due to the loss of rotational energy. $$E_{\rm rot} = \frac{1}{2} I \Omega^{2} \hRightarrow \dot{E} = I \Omega \dot{\Omega} = \text{power from mag. dipole} < 0$$ $$\therefore \quad\dot{\Omega} < 0 \quad \text{(rot. freq. decreasing)} \hspace{1cm} \dot{P} > 0 \quad \text{(period increasing)}$$
2. When period is long enough, there is no longer enough voltage to accelerate particles and produce $e^{\pm}$ pairs to power the radio emission. This leads to the pulsar activity becoming undetectable.
3. If they pulsar is in a binary or captures a companion, then as the younger star ages and overflows its [[Binary Stars#Roche Lobe]], it will accrete matter onto the NS (dead pulsar). This accretion also transfers angular momentum from the donor, increasing the spin of the NS until it co-rotates with the inner edge of the accretion disk and can begin pulsing again.

This process is evidenced by the existence of many MSPs being found in [[Stellar Clusters#Globular Cluster|globular clusters]] amongst older stellar populations.

> [!note]
> There have recently been MSPs found with high magnetic fields, which contradicts this formation picture and suggest another, similar population or a different formation channel.

#### Pulsar Timing

We use pulsars to construct a galactic-scale interferometer, with test masses bigger than the mass of the Sun. Use many millisecond pulsars to search for nHz GW signals (low freq because they're essentially a giant GW interferometer).


### Magnetar

![[NS_magnetar.jpg|align:center|500]]

A **magnetar** is a neutron star was an extremely powerful magnetic field. Over time, magnetic-field decay drives the emission of high-energy electromagnetic radiation (X-rays and gamma rays). 

- They are theorized to explain soft gamma-ray repeaters (SGRs).
- They are isolated neutron stars (i.e. not in a binary)
- We have discovered ~30 magnetars thus far.
	- 24 confirmed magnetars in 2021, one associated with repeating [[Fast Radio Burst|FRBs]]

**Origin & Formation:**

- Neutron stars originate from [[Core-Collapse|core-collapse]] [[Stellar Explosions#Supernova|supernovae]] from a massive star. 
- In the dramatic collapse, the magnetic field increases dramatically due to conservation of magnetic flux
- If conditions are correct, this can initiate the dynamo mechanic, converting heat & rotational energy into magnetic energy
- Hence, magnetars are born spinning very fast and with massive $B$ fields (~$10^{11}\,\pu{T}$) *(see [[#P-Pdot Diagram]])*
- Estimated about $1/10^{th}$ [[Stellar Explosions#Type II]] supernovae generate a magnetar versus a standard neutron star or pulsar

**Evidence of Existence:**

- Anomalous X-ray [[#Pulsar|Pulsars]] (AXPs): 
	- Isolated [[Neutron Star|neutron stars]] that emit in the X-ray
	- Usually expect to come from accretion in an [[Binary Stars#X-Ray Binary (XRB)]] 
	- Hypothesized to originate from the magnetar field.
- Soft Gamma Ray Repeaters (SGRs):
	- an astronomical object which emits large bursts of gamma-rays and X-rays at irregular intervals
- Since $B\propto \sqrt{P\dot{P}}$ , measurements of $P$ and $\dot{P}$ have revealed very high magnetic fields in some sources
	- Example: SGR 1806 in 1998

It turns out that SGRs = AXPs = magnetars (probably)

> [!measure] Typical Parameters
> Same (roughly) as [[Neutron Star#^typical-parameters|neutron star]] with the following additions/changes.
> - Magnetic field: $B \sim 10^{9} - 10^{11} \; {\rm T}$
> 	- about $10^{4}$ higher than typical NS
> - Period: $P \sim 1 - 10 \; {\rm s}$
> 	- a bit slower than typical NS
> 	- hard to quantify since they have a large range
> - Lifetime: $\sim 10^{4} \; {\rm yr}$ until magnetic field decays

> [!note] Magnetars in [[Stellar Clusters#Globular Cluster|globular clusters]]?
> 
> Maybe because the timescale for the magnetic field decay is too short relative to stellar evolution.

### Magnetar+Pulsar

Basically, a [[#Magnetar]] and [[#Pulsar]] combined into a single object. We have observed ~6 thus far.

### P-Pdot Diagram

![[NS_ppdot_together.png|align:center]]

> [!math] Lines of Constant Energy Loss Rate
> 
> Using the rotational energy for the pulsar *(see [[Question 62]])*...
> $$
> -\dot{E} = \td{E}{t} = \td{}{t} \left( \frac{I \Omega^{2}}{2} \right) = I \Omega \dot{\Omega} = - 4 \pi^{2} I \fpar{\dot{P}}{P^{3}} \hWhere \Omega = \frac{2 \pi}{P}
> $$
> If we set $\dot{E}$ as a constant, then we can plot the loss rate with linear lines on the $P$-$\dot{P}$ diagram.
> $$
> \dot{E} = 4 \pi^{2} I \fpar{\dot{P}}{P^{3}} \hRightarrow \dot{P} = \fpar{\dot{E}}{4 \pi^{2} I} P^{3}
> $$
> $$
> \log_{10} \left( \dot{P} \right) = 3 \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}
> $$
> When the energy loss reaches a certain threshold, the electric field becomes too low to accelerate particles high enough to create a current flow (i.e. the radio pulses). This gives rise to the "death line" or "graveyard" for pulsars.
^constant-Edot

> [!math] Lines of Constant Magnetic Field Strength
> 
> A rotating dipole will radiate energy at the rate of...
> 
> $$
> \dot{E} = \td{E}{t} = - \fpar{2 \pi B_{\rm p}^{2} \Omega^{4} R^{6} \sin^{2} \alpha}{3 \mu_{0} c^{3}}
> \hWhere
> \begin{aligned}
> 	B_{\rm p} &\equiv \text{polar B-field strength} \\
> 	\Omega &\equiv \text{rotational frequency} \\
> 	R &\equiv \text{radius of pulsar} \\
> 	\alpha &\equiv \text{angle between poles}
> \end{aligned}
> $$
> 
> Setting this equal to the change in rotational energy, we can find how the magnetic field strength is dependent on $P$ and $\dot{P}$.
> 
> $$
> I \Omega \dot{\Omega} = - \fpar{2 \pi B_{\rm p}^{2} \Omega^{4} R^{6} \sin^{2} \alpha}{3 \mu_{0} c^{3}}
> \hRightarrow
> \dot{\Omega} = - \fpar{2 \pi B_{\rm p}^{2} R^{6} \sin^{2} \alpha}{3 \mu_{0} c^{3} \, I} \Omega^{3} = - k \Omega^{3}
> $$
> Using $\Omega = 2 \pi / P$ such that $\dot{\Omega} = - 2 \pi \dot{P} / P^{2}$ ...
> $$
> - \frac{2 \pi \dot{P}}{P^{2}} = - \fpar{2 \pi B_{\rm p}^{2} R^{6} \sin^{2} \alpha}{3 \mu_{0} c^{3} \, I} \fpar{8 \pi^{3}}{P^{3}}
> \hRightarrow
> B_{\rm p} = \underbrace{\sqrt{\frac{3 \mu_{0} c^{3} \, I}{8 \pi^{3} R^{6} \sin^{2} \alpha}}}_{\rm constant} \; \left( P \dot{P} \right)^{1/2}
> $$
> $$B_{\rm p} \propto \left( P \dot{P} \right)^{1/2}$$
> 
> Quickly rearranging, we see that this relation yields linear lines on the $P$-$\dot{P}$ diagram (with a negative slope) for constant $B_{\rm p}$ values.
> 
> $$\frac{B_{\rm p}^{2}}{\rm constant} = P \dot{P} \hRightarrow \log_{10} \dot{P} = - \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}$$
^constant-bfield

> [!math] Lines of Constant Characteristic Age
> The lifetime of the pulsar is determined by the *braking index* ($n$).
> $$\dot{\Omega} = - k \Omega^{n}$$
> 
> Beginning with this general expression, we can assume that $k$ is constant (i.e. constant $B_{\rm p}$) of the lifetime of the pulsar and integrate.
> 
> $$
> \dot{\Omega} = - k \Omega^{n}
> \hRightarrow
> \begin{aligned}[t]
> 	k \; \rd t &= - \frac{\rd \Omega}{\Omega^{n}} \\
> 	\int_{t_{i} = 0}^{t_{f}=\tau} k \; \rd t &= - \int_{\Omega_{i}}^{\Omega_{f}} \frac{\rd \Omega}{\Omega^{n}} \\
> 	k \tau &= \frac{1}{n - 1} \left( \frac{1}{\Omega_{f}^{n-1}} - \frac{1}{\Omega_{i}^{n-1}} \right) \\
> 	\left( - \frac{1}{\Omega_{f}^{n-1}} \frac{\dot{\Omega}_{f}}{\Omega_{f}} \right) \tau &= \frac{1}{n - 1} \left( \frac{1}{\Omega_{f}^{n-1}} - \frac{1}{\Omega_{i}^{n-1}} \right) \\
> 	\left( - \frac{\dot{\Omega}_{f}}{\Omega_{f}} \right) \tau &= \frac{1}{n - 1} \left[ 1 - \fpar{\Omega_{f}}{\Omega_{i}}^{n-1} \right] \\
> 	\left( \frac{\dot{P}_{f}}{P_{f}} \right) \tau &= \frac{1}{n - 1} \left[ 1 - \fpar{P_{i}}{P_{f}}^{n-1} \right]
> \end{aligned}
> $$
> $$\tau = \frac{1}{n - 1} \left( \frac{P_{f}}{\dot{P}_{f}} \right) \left[ 1 - \fpar{P_{i}}{P_{f}}^{n-1} \right]$$
> 
> If we now approximate that $P_{i} \ll P_{f}$ , $n \approx 3$ , and $P_{f} \equiv P$ , then for constant $\tau$ values...
> 
> $$\tau = \frac{1}{n - 1} \left( \frac{P_{f}}{\dot{P}_{f}} \right) \left[ 1 - \fpar{P_{i}}{P_{f}}^{n-1} \right] \quad \approx \quad\frac{1}{2} \fpar{P}{\dot{P}}$$
> $$\dot{P} \approx \fpar{1}{2 \tau} P  \hRightarrow \log_{10} \dot{P} \approx \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}$$
^constant-age

### P-B Diagram

Similar plot as the [[#P-Pdot Diagram]], but with magnetic field strength on the axis...

![[NS_pBplot.png|align:center|550]]
> [!math] Lines of Constant Energy Loss
> 
> Use the final equation from [[#^constant-Edot|Lines of Constant Energy Loss]] and rearrange for lines with constant $\dot{P}$.
> $$
> B_{\rm p} = {\rm constant} \times (P \dot{P})^{1/2}
> \hRightarrow
> \dot{E} = 4 \pi^{2} I \fpar{\dot{P}}{P^{3}} = 4 \pi^{2} I \fpar{B_{\rm p}}{\rm constant}^{2} \frac{1}{P^{4}}
> $$
> $$B_{\rm p} = \left( {\rm constant} \times \sqrt{\frac{\dot{E}}{4 \pi^{2} I}} \right) P^{2}$$
> $$\log_{10} B_{\rm p} = 2 \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}$$
>
> This slope defines the angle death line like before.

> [!math] Lines of Constant Period Change (Pdot)
> 
> Use the final equation from [[#^constant-bfield|Lines of Constant Magnetic Field Strength]] and rearrange for lines with constant $\dot{P}$.
> $$B_{\rm p} = {\rm constant} \times (P \dot{P})^{1/2}$$
> $$\log_{10} B_{\rm p} = \frac{1}{2} \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}$$

> [!math] Lines of Constant Characteristic Age
> 
> Use the final equation from [[#^constant-age|Lines of Constant Characteristic Age]] and rearrange for lines with constant $\dot{P}$.
> $$
> B_{\rm p} = {\rm constant} \times (P \dot{P})^{1/2}
> \hRightarrow
> \dot{P} = \fpar{B_{\rm p}}{\rm constant}^{2} \frac{1}{P} = \frac{P}{2 \tau}
> $$
> $$B_{\rm p} = \fpar{\rm constant}{\sqrt{2 \tau}} P$$
> $$\log_{10} B_{\rm p} = \log_{10} P + {\rm constant} \hspace{2cm} \textcolor{gray}{\left[ y = m x + b \right]}$$


