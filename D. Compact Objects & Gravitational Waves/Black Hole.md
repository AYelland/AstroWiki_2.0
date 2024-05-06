---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - black holes
  - BH
  - Black Holes
  - black hole
---
A **black hole** is region of spacetime where gravity is so strong that nothing, including light and other electromagnetic waves, has enough energy to escape it.

## Black Hole Parameters

After reaching a stable condition, a black hole has only three independent, physical properties:
- **mass** ($M_{\rm BH}$)
- **electric charge** ($Q_{\rm BH}$)
- **angular momentum** ($J_{\rm BH}$)

Otherwise, black holes are featureless and indistinguishable from one another (no-hair theorem).

> [!note] Constraints on Parameters
> Though the mass of a black hole can be any positive value that formation and the universe allows, the charge and momentum on constrained by the mass. 
> $$\frac{Q}{4 \pi \varepsilon_{0}} + \frac{c^{2} J^{2}}{G M^{2}} \le G M^{2}$$
> See below for details.
^parameter-constraint
### Mass

The mass of a black hole is all contained within the [[#Singularity|singularity]]. 

![[BH_LIGO-Virgo_massplot.png]]

The above image summarizes the current compact object mass observations determined by **gravitational wave** observations (mergers measured by [[Instruments#LIGO]], [[Instruments#VIRGO]], [[Instruments#KAGRA]]) and **electromagnetic (EM)** observations (typically referring to [[Binary Stars#X-Ray Binary|x-ray binary]] measurements).

> [!space] Mass Gaps
> 
> In the image above, one can see an observed "**lower mass gap**" ($M \sim 2 - 5 \; {\rm M_{\odot}}$) in the black hole candidates.
> 
> There is also an "**upper mass gap**" known as the "**Pair Instability Gap**" ($M \sim 60 - 150 \; {\rm M_{\odot}}$) originating from a lack of theoretical backing. From [[Hertzsprung-Russell Diagram|stellar evolution]] of massive stars, we can for predict the formation of $M_{\rm BH} \sim 45-60 \; {\rm M_{\odot}}$ black holes through gravitational collapse. However, we do not know the mechanism of how larger black holes form. 
> 
> By the story of stellar evolution, when very massive stars ($130 - 250 \; M_{\odot}$) reach their end-of-life, their core undergoes pair production that leads to a partial gravitational collapse, followed by a thermonuclear explosion that destroys the star and leaves no remnant. Hence, there shouldn't be any progenitor stars big enough to form these [[#Intermediate-Mass Black Hole|IMBHs]].
> 
> The [[Question 163|GW190521]] observation shows that [[#Intermediate-Mass Black Hole|IMBHs]] are likely to be the result of mergers, but it is still a highly active area of research at the moment.
^mass-gap

Most of the black holes seen above are $\mathcal{O}(10 \; {\rm M_{\odot}})$, but they are still considered them as [[Black Hole#Stellar Black Hole|stellar black holes]].

### Spin

The spin (or angular momentum) can be parameterized by the maximum physical spin an an object could have, while still held together through gravitational force.

$$J_{\rm max} = \frac{G M^{2}}{c} \hRightarrow |J| \le |J_{\rm max}| = \frac{G M^{2}}{c} \hRightarrow a \equiv \frac{c \, |J|}{G M^{2}} \le 1$$

By this, we can define the spin-parameter $a \in \left[ -1, 1 \right]$ , such that any rotating black hole's spin is relative to the speed of light. *(In actuality, the maximum spin is $a \simeq 0.998$, but I won't go into details.)*

The physical meaning of this parameter is:

$$
a = \cases{
	-1 &\text{(retrograde, maximal spin)} \\ 
	~~~0 &\text{(Schwarzschild, zero spin)} \\ 
	+1 &\text{(prograde, maximal spin)}
}
$$

We could further describe another spin parameter ($\alpha$) through the [[General Relativity#Kerr Metric]] in general relativity. I will not go into details, but it can be derived as a function of $a$ such that...

$$
a = \cases{
	-1 &\text{(retrograde, maximal spin)} \\ 
	~~~0 &\text{(Schwarzschild, zero spin)} \\ 
	+1 &\text{(prograde, maximal spin)}
}
\hRightarrow
\alpha = \begin{cases}
	9 &\text{when } a=-1 \\
	6 &\text{when } a=~~~0 \\
	1 &\text{when } a=+1
\end{cases}
$$

> [!note] When considering black hole binaries...
> When considering black hole binary mergers and the production of gravitational waves, see the [[Gravitational Waves#Mass-Weighted Effective Spin]] ($\chi_{\rm eff}$). It is similar bounds as the spin parameter of the black hole, but is reliant on both merging masses.

### Charge

https://astronomy.stackexchange.com/questions/44811/how-can-a-black-hole-have-a-charge-or-be-charged

Charged black holes have not been seen (nor are predicted) to exist in nature; however, there is a theoretical probability that follows the fact that the elementary charge is carried by some matter particles.

A black hole would be considered "charged" if for some reason it accretes more protons than electrons (or vice versa).

## Structure

![[BH_anatomy.jpg|align:center|550]]


### Singularity

The gravitational **singularity** is at the centre of a black hole where the spacetime curvature becomes infinite. For a non-rotating black hole, this region takes the shape of a single point; for a rotating black hole it is smeared out to form a ring along the plane of rotation. In both cases, the singular region has zero volume. It can also be shown that the singular region contains all the mass of the black hole solution, such that it can be thought of as having infinite density.

### Event Horizon

![[BH_anatomy_kerr_layers.png|align:center|600]]

The **event horizon** is the boundary in spacetime at which matter and light can only travel inward towards the mass of the black hole. Hence, if an event occurs within the boundary, information from that event cannot reach an outside observer, making it impossible to determine whether such an event occurred.

For non-rotating black hole, the event horizon is defined by the **Schwarzschild Radius. 

$$R_{\rm S} = 2 R_{\rm g} = \frac{2 G M}{c^{2}}$$

For a rotating black hole, there is both an *outer horizon* (Schwarzschild horizon) and the *inner horizon* (Cauchy horizon). 
- The outer horizon is boundary of the region from which matter and light do not escape to infinity. 
- The inner horizon is the boundary of the region which contains *closed timelike geodesics/curves*. It lies entirely within the outer horizon. (mathematically complex)
- For non-rotating black hole, the inner and outer horizons coincide.
- *([A helpful reddit post](https://www.reddit.com/r/askscience/comments/5uzg51/what_is_the_inner_and_outer_horiz))*

The topology of the both event horizons is always spherical when in equilibrium; however, the geometry may not be. For non-rotating (static) black holes, the geometry of the event horizon is precisely spherical, while for rotating black holes, it can be geometrically more oblate. 


### Photon Sphere

![[BH_photonsphere.gif|align:center|550]]

The **photon sphere** is the boundary at which photons can exist in a purely tangential, circular orbit about the black hole. Past this boundary, all light will inspiral and eventually cross the [[#Event Horizon|event horizon]]. Similarly, for any light that escapes the black hole and reaches an outside observer must originate from beyond the photosphere.

For non-rotating black holes, the photon sphere has a radius $r_{\rm photon} \sim 1.5 \, R_{\rm S}$ (where $R_{\rm S} \equiv$ Schwarzschild radius). For a rotating black hole, the radius is dependent on the spin parameters and on the details of the photon orbit, which can be prograde or retrograde.

### Ergosphere

![[BH_anatomy_ergosphere.png]]

The **ergosphere** is a region of spacetime around a rotating black hole ([[#Kerr Black Hole|Kerr]], [[#Kerr-Newman Black Hole|Kerr-Newman]]) in which it is impossible to stand still due to *frame-dragging* (rotating masses "drags" the spacetime immediately surrounding it). Hence, any object in this region will start moving in the direction of rotation. 

It has a volume bounded by the black hole's event horizon and the ergosurface, which coincides with the event horizon at the poles but has a much larger radius around the equator.

Objects and radiation can escape normally from the ergosphere. Through the Penrose process, objects can emerge from the ergosphere with more energy than they entered with. The extra energy is taken from the rotational energy of the black hole. Thereby the rotation of the black hole slows down. A variation of the Penrose process in the presence of strong magnetic fields, the Blandford–Znajek process is considered a likely mechanism for the enormous luminosity and relativistic jets of quasars and other active galactic nuclei.

> [!note] For a rotating black hole, this effect is so strong near the event horizon that an object would have to move faster than the speed of light in the opposite direction to just stand still.

### Innermost Stable Circular Orbit (ISCO)

![[BH_isco.png|aling:center|400]]

The **innermost stable circular orbit (ISCO)** is the orbit at which any inward perturbations will cause the orbiting body to inspiral, and any outward perturbations could result the orbiting also inspiralling, finding a stable elliptical orbit, or escaping the black hole.

For non-rotating black holes, the ISCO has a radius $R_{\rm ISCO} \sim 3 \, R_{\rm S}$ (where $R_{\rm S} \equiv$ Schwarzschild radius). 

$$R_{\rm ISCO} = 3 R_{\rm S} = 6 R_{\rm g} = \frac{6 G M}{c^{2}} \hWhere R_{\rm g} = \frac{G M}{c^{2}}$$

For a rotating black hole, the location of the ISCO dependent on the [[#Spin|spin parameter]] ($a$) of the black hole.

$$
R_{\rm ISCO} = \begin{cases}
	9 R_{\rm g}=\tfrac{9}{2} R_{\rm S} &\hspace{1cm} a = -0.998 \quad &\text{(retrograde, maximal spin)} \\
	6 R_{\rm g}=3 R_{\rm S} &\hspace{1cm} a = ~~~0 \quad &\text{(Schwarzschild, zero spin)} \\
	R_{\rm g}=\tfrac{1}{2} R_{\rm S} &\hspace{1cm} a = + 0.998 \quad &\text{(prograde, maximal spin)}
\end{cases}
$$

## Mass Classification
### Micro Black Hole


> [!measure] Typical Parameters
> 
> Approx. Mass: $M_{\rm BH} \lesssim 1 \; {\rm M_{\rm moon}}$ 
> Approx. Schwarzschild Radius: $R_{\rm S} \lesssim 0.1 \; {\rm mm}$ 

Current area of research, though no candidate yet. David Keiser (MIT, CTP) is working with many others (Salvodor Vitali, Noah Wolfe, Peter Fisher, etc.) on potentially detect astroid-sized or smaller within the solar system, or nearby. Potential methods of detection include:
- Measuring gravitational shifts in planetary bodies over time
	- We have very accurate tracking systems
	- With radial velocity, resolution is $\sim 0.3 \; {\rm m/s}$ (pushing to $\sim 0.1 \; {\rm m/s}$)
- Measuring the Hawking Radiation (AMS-02)

### Stellar Black Hole

> [!measure] Typical Parameters
> 
> Approx. Mass: $M_{\rm BH} \lesssim 2 - 150 \; {\rm M_{\odot}}$
> Approx. Schwarzschild Radius: $R_{\rm S} \lesssim 30 \; {\rm km}$

**Mass Measurements:**
- For the EM observations: (XRBs)
	- If we have radial velocity measurements, we can find constraints on the mass through the [[Binary Stars#For a Spectroscopic Binary|binary mass function]]. $$v_{\rm 1,r} = \fpar{2 \pi G}{P}^{1/3} \fpar{M_{2} \sin i}{(M_{1} + M_{2})^{2/3}} \frac{1}{\sqrt{1-e^{2}}}$$ 
	- We can infer the mass though X-ray [[Methods#Reverberation Mapping]] (*x-ray timing*)
		- Uses the time lags between correlated X-ray signals to infer information about the environment very close to a black hole, and indirectly, properties of the black hole.
		- Has only been done in one source (Cygnus X-1, Mastroserio+19).

- For GW observations: ([[Instruments#LIGO]], [[Instruments#VIRGO]])
	- For the [[Instruments#LIGO]] observations, we can observe the [[Question 43|gravitational frequency and amplitude]], [[Gravitational Waves#Chirp Mass|chirp mass]], and duration of compact binary merger. Assuming the coalescence of the two masses happens at the ISCO radius ($R_{\rm ISCO}$), we can calculate the orbital frequency ($\omega_{\rm c}$) and gravitational wave frequency ($f_{\rm c} = \omega_{\rm c} / \pi$) at coalescence from [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] as... $$\omega_{\rm c} = \frac{f_{\rm c}}{\pi} = \sqrt{\frac{G M}{a_{c}^{3}}} = \frac{c^{3}}{(6)^{3/2} \, G M}$$...along with the amplitude...$$h_{0} = \fpar{4}{\sqrt{5} c^{4}} \frac{(G M_{\rm c})^{5/3}\omega^{2/3}}{R}$$Once we have $M$ and $M_{\rm c}$, we can combine them to find the individual binary mass before merging.


**Spin Measurement:**

> [!space] Spinning Objects
> It has been [observed](https://www.annualreviews.org/doi/abs/10.1146/annurev-astro-112420-035022) that....
> - Due to angular momentum conservation of the progenitor star, it's expected that a stellar mass black hole are spinning.
> - [[Binary Stars#X-Ray Binary|X-ray binaries]] (XRBs) are rapidly spinning. 
> - LIGO has discovered many slowly-spinning black holes with $\chi_{\rm{eff}}\simeq 0$ (the [[Gravitational waves#Mass-weighted effective spin|mass-weighted effective spin]]).

- For the EM observations: (XRBs)
	- **[[Methods#Reflection Spectroscopy]]** 
		- Use the shape of spectral lines emitted from the [[Active Galactic Nuclei#Corona|corona]] and reflected off the accretion disk to constrain $R_{\rm{ISCO}}$ (dependent on spin parameter $a$)
		- Key feature in the spectrum to measure this feature is the [[Spectral Features#Fe K-alpha Line|Fe K-alpha line]].
			- The line is blurry (fluorescent) due to [[Spectral Features#Relativistic Effects on Profiles|relativistic effects]] (i.e. transverse Doppler, gravitational redshifting) *([source](https://www.semanticscholar.org/paper/Broad-iron-lines-in-Active-Galactic-Nuclei-A.C.Fabian-K.Iwasawa/13654e12a16c49dae1353238fc7e6bbc7e715810))*
			- The shape of resulting line constrains the GR effects, and thus $R_{\rm{ISCO}}$ 

	- **Thermal continuum fitting**
		- Spin influences temperature of inner disk by [[#Innermost Stable Circular Orbit (ISCO)|changing ISCO radius]] such that: 
			-  Higher spin $\implies$ smaller $R_{\rm{ISCO}}$ $\implies$ more gravitational PE converted to KE $\implies$ hotter temperature of inner accretion disk. 
		- Requires good understanding of disk modelling and radiative transfer modelling of XRBs.
- For GW observations: ([[Instruments#LIGO]], [[Instruments#VIRGO]])
	- LIGO is constrained by using matched filtering techniques applied to the GW waveform at inspiral and merger.
	- Constrain [[Black Hole#Spin|spin parameter]] ($a$) via the [[Gravitational waves#Mass-weighted effective spin|mass-weighted effective spin]] ($\chi_{\rm eff}$) and [[Gravitational waves#Effective precession spin|effective precession spin]] ($\chi_{\rm p}$).
		- If we only constrain $\chi_{\rm{eff}}$,  there is a degeneracy due to the projection along direction of orbital angular momentum. This degeneracy can be broken by identifying $\chi_p$, but it can only be constrained for unequal mass ratio binaries.

### Intermediate-Mass Black Hole
*(Abbrev. as **IMBH**)*

> [!measure] Typical Parameters
> 
> Approx. Mass: $M_{\rm BH} \lesssim 10^{2} - 10^{5} \; {\rm M_{\odot}}$
> Approx. Schwarzschild Radius: $R_{\rm S} \lesssim 10^{3} \; {\rm km} \approx R_{\oplus}$

### Supermassive Black Hole
*(Abbrev. as **SMBH**)*

> [!measure] Typical Parameters
> 
> Approx. Mass: $M_{\rm BH} \lesssim 10^{6} - 10^{9} \; {\rm M_{\odot}}$
> Approx. Schwarzschild Radius: $R_{\rm S} \lesssim 0.001 - 400 \; {\rm AU}$

**Mass Measurement:**
- Special Case: 
	- In the Milky Way we can resolve individual stellar orbits around the BH [[Active Galactic Nuclei#Sagittarius A*]] and infer the mass from the dynamics. Found $M\sim4\times 10^6\,M_\odot$ 
- The M-$\sigma$ Relation ([[Velocity Dispersion#M-Sigma Relation|here]]):
	- The mass of SMBH ($M$) is related to velocity dispersion ($\sigma$) of stars in the bulge.
	- If we measure $\sigma$ from spectral line widths, we can infer the SMBH mass.
	- See [[Question 124]].
- [[Methods#Reverberation Mapping]] in the [[Active Galactic Nuclei|AGN]]:
	- Measure the timing delay between optical broad lines with respect to the continuum to get the location of the "broad line region" (BLR). Then, relate the SMBH mass to the velocity widths of the lines $$M_{\rm BH} = \frac{f (\Delta v)^{2} r_{\rm BLR}}{G} \hWhere \underbrace{f \equiv \text{BLR scaling factor} \sim 5}_{\text{dependent on geometry and kinematics}}$$
	- Requirements:
		- High time resolution ($\lesssim 1 \; {\rm day}$)
		- Long duration monitoring ($\lesssim 1 \; {\rm day}$)
		- Moderate spectral resolution ($\lesssim 1 \; {\rm day}$)
		- High signal-to-noise ratio
- [[Instruments#EHT]] uses [[Methods#Long baseline interferometry|(very) long baseline interferometry]] to measure the size of [[Black Hole#Photon Sphere|BH shadow]], which is dependent on mass.

**Spin Measurement:**
- [[Methods#Reflection Spectroscopy]] as with [[Binary Stars#X-Ray Binary|XRBs]] (similar to [[#Stellar Black Hole]] spin measurements)
- Cannot use spectral continuum fitting because $k_{\rm B} T \lesssim 0.05 \; {\rm keV}$ for SMBH
	- This is because much of the [[Blackbody Radiation|blackbody]] disk emission is absorbed and inaccessible.

Looking at the overall population of SMBH, there appears that the spin is very high on average. 
- Accretion (coherent) onto a SMBH seems to be a big contributor to increasing the spin.
- Mergers on the other hand could increase the spin, but could also cancel it out. (imagine combining two vectors pointing in random directions). That means, if BH mergers contributed more to the mass growth of a SMBH, then it's likely to have a lower spin.
	- One might think the orbital frequency at coalescence would contribute to the overall spin, but it tends to significantly lower given the physical size of the SMBH and the defined point of "coalescence"

For the biggest of the big, merger events must have been important for them to growth to such large masses. Given the age of the universe, accretion alone cannot account for the size of the largest SMBH.

In the image below, we show that we observe a larger population of SMBH that have high spins ($a$ closer to 1), though there is an overall trend downwards that the largest SMBH has lower spins (left plot).

![[BH_smbh_spin_mass.png|align:center|600]]

That said, given our limits in instrumentation, we are biased toward measuring high-spin BH (right plot). Spins are typically measured by X-ray [[Methods#Reflection Spectroscopy]], but we can't use this methodology for lower spin BH due to the observation gap in the [[Electromagnetic Spectrum|EM spectrum]] (UV) caused by hydrogen absorption. Given that to the disk's [[Blackbody radiation#Blackbody radiation|blackbody radiation]] emits in this gap for low spin BH, the radiation is being absorbed prior to reaching us, and is inaccessible. (i.e. can't use continuum fitting)
   
### Ultramassive Black Hole
*(Abbrev. as **UMBH**)*

> [!measure] Typical Parameters
> 
> Approx. Mass: $M_{\rm BH} \lesssim 10^{9} - 10^{11} \; {\rm M_{\odot}}$
> Approx. Schwarzschild Radius: $R_{\rm S} \gtrsim 1000 \; {\rm AU}$

## Spin-Charge Classification

Beyond the [[#Mass Classifications]] above, one can also define 4 other classifications based on the spin (angular momentum) and the charge of the black hole.

|                    |        Non-Rotating ($J=0$)        |      Rotating ($J>0$)       |
| :----------------: | :--------------------------------: | :-------------------------: |
| Uncharged ($Q=0$)  |   [[#Schwarzschild Black Hole]]    |    [[#Kerr Black Hole]]     |
| Charged ($Q\ne 0$) | [[#Reissner-Nordström Black Hole]] | [[#Kerr-Newman Black Hole]] |

### Schwarzschild Black Hole

A non-rotating, non-charged black hole.

*(Originating from a solution of Einstein field equation, solved with the [[General Relativity#Schwarzschild Metric]].)*

### Kerr Black Hole

A rotating, non-charged black hole.

*(Originating from a solution of Einstein field equation, solved with the [[General Relativity#Kerr Metric]].)*

### Reissner-Nordström Black Hole

A non-rotating, charged black hole.

### Kerr-Newman Black Hole

A rotating, charged black hole.


