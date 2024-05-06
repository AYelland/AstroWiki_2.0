---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - cosmic microwave background
  - CMB
---
	## General Information

The **Cosmic Microwave Background** is the most prominent peak of the [[Question 82#^EBL|Extragalactic Background Light (EBL)]]. More specifically, it is the remnant *microwave radiation* from when photons and baryonic matter decoupled during [[Cosmological Timeline#Recombination|recombination]] in the early universe. 

![[EBL.png]]

At [[Cosmological Timeline#Recombination|recombination]], the opacity (from [[Compton Scattering|electron scattering]]) dropped as the universe became cool enough for baryonic matter to recombine and form [[Interstellar Medium#Atomic Hydrogen|atomic, neutral hydrogen]]. ($z_{\rm rec} \sim 1100$, $T_{\rm rec} \sim 3000 \; {\rm K}$)

With a standard optical telescope, the background space between stars and galaxies is almost completely dark. However, a sufficiently sensitive radio telescope detects a faint background glow that is almost uniform and is not associated with any star, galaxy, or other object. This glow is strongest in the microwave region of the radio spectrum.

![[CMB_cosmological_timeline.png|align:center|570]]

*(Image Source: http://background.uchicago.edu/~whu/Papers/HuWhi04.pdf)*

## History of CMB Observations

**1965** 
- Penzias and Wilson discover the CMB (1978 Nobel Prize)
	- Found from $4.2 \; \pu{K}$ excess antenna temperature
- Originally predicted by Alpher and Herman in 1948, but the tidea did not gain much traction at the time

**1980**
- Theoretical limits were placed on CMB inhomogeneities in part by soviet experiment RELKIT-1

**1992**
- NASA launches [[Instruments#COBE|COBE]], which measured CMB anisotropy at $\Delta T/T \simeq 10^{-5}$ precision
	- Essentially measured the low-$l$ (where $l \equiv$ multipole moment) flat part of the [[#CMB Power Spectrum|CMB power spectrum]]
- 2006 Nobel prize

**2001**
- NASA launches [[Instruments#WMAP|WMAP]], which measured out to the third peak of the [[#CMB Power Spectrum|CMB power spectrum]]

**2013**
- NASA launches [[Instruments#Planck|Planck]], which measured with the best angular resolution relative to any previous instrument
- Extremely precise [[#CMB Power Spectrum|power spectrum]] measurement.

**2014**
- [[Instruments#BICEP|BICEP2]] announces detection of B mode [[#CMB Polarization|CMB polarization]] and claim this is evidence of inflationary gravitational waves. Later revealed that [[Interstellar Medium#Dust|dust]] was the real culprit (see [[Question 79]])

*(There has been a number of ground-based and balloon experiments since, but the main results are summarized below.)* 

![[CMB_instrument_comparison.png|align:center]]


**What are the well-measured quantities today?**
1. The almost perfect CMB [[Blackbody radiation#Blackbody radiation|blackbody]] spectrum ($T_{\rm peak} =2.73 \; \pu{K}$). 
	- The anisotropies are on the order of $\Delta T/T \sim 10^{-5}$, which corresponds to temperature differences of about $30\,\pu{\mu K}$ that result from matter under- and over-densities in the early universe.
2. The [[#CMB Power Spectrum]].
	- measures the amount of variations in $T$ at different angular scales.

**What is left to be measured?**
- A detection of the B-mode [[#CMB Polarization.]]
	- Data would inform the existence of primordial (stochastic) [[Gravitational Waves#Sources of Gravitational Waves|gravitational waves]] from the big bang. 

## Inhomogeneity of CMB

The inhomogeneity of the CMB can be broken down into three terms, as deviations from a perfect [[Blackbody Radiation|blackbody]] spectrum.
- **Spectral Distortions** : energy-dependent and direction-independent effects
- **[[#Anisotropies]]** : energy-independent and direction-dependent effects
- **Spectral-Spatial Distortions** : energy-dependent and direction-dependent effects

 In terms of temperatures, we have:
 
$$T(\nu, \vec{n}) = T_{0} + \underbrace{\Delta T(\nu)}_{\text{spectral}} + \underbrace{\Delta T (\vec{n})}_{\text{anisotropy}} + \underbrace{\delta T(\nu, \vec{n})}_{\text{spectral-spatial}}$$

### Anisotropies

![[CMB_PS_sources_megan.png|align:center|450]]

The anisotropy (directional dependency) of the CMB signal is divided into two types: 
1) **Primary Anisotropy** - effects that occur at the surface of last scattering (the spherical shell on the sky in which the photons are now received/observed that were originally emitted at [[Cosmological Timeline#Recombination]]) or before.
2) **Secondary Anisotropy** - effects such as interactions of the background radiation with intervening hot gas or gravitational potentials, which occur between the last scattering surface and the observer.

#### Primary Anisotropies

1. **Non-Integrated Sachs-Wolfe Effect** ($l\lesssim 100$)
	- Composed of two gravitational effects from [[Dark Matter|DM]] potential wells in early universe:
		- [[Redshift#Gravitational Redshift]] - photons escaping the well are redshifted as they climb out of the well (if well deepens) $\implies$ cooler/redder
		- Gravitational Time-Dilation - photons from deeper wells are from earlier times $\implies$ hotter/bluer
	- Together, these effects yield a net redshift of the $1/3$ of the normal [[Redshift#Gravitational Redshift|gravitational redshift]] alone.
		- overdensities $\implies$ cooler/redder
		- underdensities $\implies$ hotter/bluer
	- Caused by occurring at the surface of last scattering. 
	- The effect is not constant across the sky due to differences in the matter/energy density at the time of last scattering
	- On larger scales, the CMB temperature follows matter density profile ([[matter_power_spectrum.png|dark matter power spectrum]]).

2. **Acoustic Oscillations** ($100\lesssim  l \lesssim 1000$)
	- See [[Baryon Acoustic Oscillations|BAO]].

3. **Silk Damping** ($l \gtrsim 1000$)
	- "photon diffusion damping" which washes out scales smaller than $l = 1000$ ($\lesssim 0.1^\circ$, around the third acoustic peak)
	- On small scales, the photons are not coupled to the DM wells, and are able to diffuse (effectively smoothing out the CMB power spectrum)
		- The **silk scale** is distance scale over which photon diffusion is important at $z=1100$. When using the current angular scale of $0.1^\circ$, the silk scale is $\sim 3 \; \pu{Mpc}$. 
		- The mass contained within the scale is the **silk mass**, which we estimate to be $\sim 10^{13} \; {\rm M_{\odot}}$ (i.e. about the mass of a galaxy today 😱). 
		- Smaller scales (and smaller masses) are washed out.
	- [[Cosmological Timeline#Recombination]] $\implies$ photons can "suddenly" travel much farther
	- These photons carry energy from the hot regions and diffuse to the cold regions, also dragging baryons around, such that any anisotropy on a very small scale is quickly washed out. Effect is strongest for smallest scales (largest $l$)
	- There also exists electron diffusion damping for the same reasons, but it is far weaker since the electrons couldn't diffuse nearly as far.

#### Secondary Anisotropies

1. **Integrated Sachs-Wolfe Effect**
	- Same thing as non-integrated but can blueshift if photon passes through a well thats shallowing or redshifted if passing through a well thats deepening.
2. **[[Thomson Scattering]]**
	- Free $e^{-}$ in the universe lead to overall damping of CMB fluctuation amplitudes
	- isotropic and scale-independent
3. **[[Cosmic Microwave Background#Sunyaev-Zeldovich Effect]]**
	- [[Inverse-Compton Scattering]] of CMB photons by high energy electrons
	- Two flavors: thermal (from $e^{-}$ temp) + kinetic (from $e^{-}$ bulk motion)
	- Only applies at very small scales (very high $l$)
4. **[[Gravitational Lensing]]**
	- Large scale structure can lens the CMB, which has the effect of mixing E and B mode polarizations on the sky. 
	- Conserves [[Intensity|surface brightness]] $\implies$ only affects anisotropies
5. Late-time integrated Sachs–Wolfe Effect
	- Informs expansion of universe and thus $\Omega_\Lambda$ 

Theres also the [[Cosmic Microwave Background#CMB Polarization]] signal.

## CMB Power Spectrum

We see small deviations across the sky ($\Delta T/T \sim 10^{-5}$) in the CMB from a perfect [[Blackbody Radiation|blackbody]] which result from matter under- and over-densities in the early universe. 

To study the angular scales of these fluctuations one decomposes the temperature signal$^1$ on the 2D sky into a summation of [[Spherical Harmonics#The Spherical Harmonics|spherical harmonics]]$^2$ (similar to quantum mechanics when treating the hydrogen atom).

To measure the effective weight of a specific harmonic's contribution to the [[#Anisotropies|CMB anisotropies]], we can calculate the coefficients ($C_{l}$) of the signal $\delta T = \Delta T/T$ in this orthonormal basis.

$$\delta T(\theta,\phi) = \sum_{l=0}^{\infty}\sum_{m=-l}^{+l} a_{ml} Y_{ml}(\theta,\phi) \hRightarrow a_{ml} = \int_{\rm{sky}} \rd \Omega\, Y_{ml}^\star(\theta,\phi)\, \delta T(\theta,\phi)$$

From the orthogonality of the basis we have...

$$\langle a_{ml} \, a_{m'l'}^\star\rangle = \delta_{ll'}\delta_{m m'} C_l$$

...which can be recast as an expression for the coefficient $C_l$ (for a given $l$ averaged over the index $m$ by summing over both $l'$ and $m'$).

$$C_l = \frac{1}{2l+1}\sum_{m=-l}^{+l}\langle |a_{ml}|^2 \rangle$$

Making a plot of the quantity $l(l+1)C_l/2\pi$ versus $l$ (this normalization chosen just so the low $l$ side where the Sachs-Wolfe effect takes over is flat, and the acoustic peaks are visually emphasized), we obtain the **CMB power spectrum**.

![[CMB_PS_sources_megan.png|align:center|450]]

...where the $l$ of the first peak is calculated in [[#Sound Horizon]] to be $l\sim 220$ (i.e. $\theta \sim 1^{\circ}$) and real measurements from [[Instruments#Planck|Planck]] look like the following: jhhj

![[planck_PS.png|align:center|500]]

> [!note]
> 
> $^1$ The signal *after* subtracting the monopole signal arising from the motion of your detector relative to the CMB, which effectively amounts to the relative motion of the [[Galaxy Group#Local Group]] relative to the rest frame of the CMB. Interestingly, fitting the CMB monopole direction (the direction we are moving in relative to CMB rest frame) gives a very different answer than other measurements, treated as another [[Dark Matter#LCDM]] tension.
> 
> $^2$loosely, we have a discrete basis because compact spaces like the 2D sphere on the sky admit discrete decompositions, as with the spin operator in QM. In fact, depending on the paper they may may decompose into lagrange polynomials rather than spherical harmonics.

### Origin of the Peaks

See [[Baryon Acoustic Oscillations]].

In summary...
- Gravity acts on the baryons and pulls them in towards over densities, making then denser and compressing the fluid in potential wells set by [[dark matter]].
- Photon radiation pressure resists the compression and pushes the fluid back out, making the regions less dense and causing another rarefaction.
- This created conditions for "acoustic" oscillations (sound/pressure waves) of the photon-baryon fluid.
- At [[Cosmological Timeline#Recombination]], these acoustic oscillations are "frozen-in" as the photon-baryon fluid decouples, allowing the photons to free-stream with an imprinted image of the universe's energy density at the time of recombination. $\implies$ CMB

### Relation to Cosmological Density Parameters

![[CMB_PS_param_megan.png|align:center|650]]

The relative densities ($\Omega_{i}$) defined in [[Friedmann Equation]] have the following effects on the power spectrum, with more details below.

- $\Omega_{k}$ : sets the location and spread of the first peak in power spectrum
- $\Omega_{M}$ : sets amplitude scale of the power spectrum
- $\Omega_{b}$ : sets the difference in even/odd peak heights between expansions and compressions

**Curvature Density** ($\Omega_{k}$)

Since we use the [[Distances#Angular Diameter Distance|angular distance diameter]] to measure the length scales/angles of the CMB, the location of the peaks changes with the curvature of spacetime ($k$). 

If we compare different curvatures ($k$) for open/flat/closed universes ($\theta_{o/f/c}$ , $l_{o/f/c}$), then we would see:

| Curvature                   | Sign             | Shape                         | Effect on Angular Size                                          |
| --------------------------- | ---------------- | ----------------------------- | --------------------------------------------------------------- |
| Open ($k<0$)                | $\Omega_{k} > 0$ | <nobr>Hyperbolic Space</nobr> | Measure a smaller angle $\theta$ (bigger $l$)                   |
| Flat ($k=0$)                | $\Omega_{k} = 0$ | Flat Space                    | <nobr>Measure a simple angle $\theta$ (intermediate $l$)</nobr> |
| <nobr>Closed ($k>0$)</nobr> | $\Omega_{k} < 0$ | Spherical Space               | Measure a bigger angle $\theta$ (smaller $l$)                   |

That is, $l_{c} < l_{f} < l_{o}$. We can think of it like "in an open universe, a cone opens up between you and the object, so the cone angle at the tip where you are is thinner" and converse for a closed universe.

$$\ell \; \propto \; \frac{180^{\circ}}{\theta} \hWhere \theta_{\rm open} < \theta_{\rm flat} < \theta_{\rm closed}$$

![[CMB_omegaK.png|align:center|650]]
![[curvature_observation_shape.jpg|align:center|550]]


**Matter Density** ($\Omega_{M}$)

The measure of the power spectrum's overall amplitude. The matter density sets the rate of expansion/collapse, and thus, the time for the universe to reach [[Cosmological Timeline#Recombination|recombination]].

![[CMB_matterdensity_comparison.png|align:center|300]]

Essentially, *the more matter there is, the faster we reach [[Cosmological Timeline#recombination]].* If we reach recombination faster, there is less time for structure to grow in the early universe, and we see weaker power across the whole spectrum. (Similarly, less matter means stronger structure.)

$$t = \frac{2}{3 H(z)} = \frac{2}{3 H_{0} \sqrt{\Omega_{M} (1+z)^{3}}} \propto \frac{1}{\Omega_{M}^{1/2}}$$

|          Mass?          |                               |                                  |                             |                         | Effect?           |
|:-----------------------:|:-----------------------------:|:--------------------------------:|:---------------------------:|:-----------------------:| ----------------- |
|  $\Omega_{M} \uparrow$  | faster to reach recombination | younger universe ($t\downarrow$) | less time to grow structure |  weaker power spectrum  | peaks go **down** |
| $\Omega_{M} \downarrow$ | slower to reach recombination |   older universe ($t\uparrow$)   | more time to grow structure | stronger power spectrum | peaks go **up**   |


![[CMB_omegaM.png|align:center|650]]

**Baryon Density** ($\Omega_{b}$)

Baryons (or ordinary matter) load down the photon-baryon plasma and add inertial (and gravitational) mass to the oscillating system. 

Their effect on the acoustic peaks is similar to what happens when you add mass to a spring and let it fall in the gravitational field of the Earth. With more mass loading the spring, it falls further before pulled back by the spring. On the other hand, it rebounds to the same position it started from. 

Therefore...
- The odd numbered (first, third, fifth...) acoustic peaks are associated with how far the plasma "falls" into gravitational potential wells (how much the plasma compresses).
- The even numbered peaks (second, fourth, sixth) are associated with how far the plasma "rebounds" (how much the plasma rarefies).

With increase in the amount of baryons in the universe, the odd peaks are enhanced over the even peaks. For example, baryons make the first acoustic peak much larger than the second. The more baryons the more the second peak is relatively suppressed. If we had almost no baryons at all, the first two peaks would be about the same size.

![[CMB_omegaB.png]]

**Dark Matter Density** ($\Omega_{\rm DM}$)

A higher proportion of dark matter will enhance the height of the third peak of the CMB power spectrum, relative to the second. 

The third peak comes from oscillations that have had time to reach maximum density, then minimum density, and then maximum density. The minimum density is reached after the photon pressure catapults the baryonic matter out of the potential well. Therefore, the dark matter that does not interact with photons remains. The more dark matter there is left in a region, the denser it can become as gravity takes over again. Therefore, more dark matter means a higher third peak.

By changing the $\Omega_{M}$ density parameter...
- $\Omega_{\rm DM} \uparrow \implies$ lowers overall power spectrum amplitude (same as $\Omega_{M}$)
- $\Omega_{\rm DM} \downarrow \implies$ eliminates the [[Baryon Acoustic Oscillations|BAO]] effects, leading to higher 3rd peak amplitude 
	- Indication of dark matter without baryons

> [!image] Changing the DM Density
> 
> ![[CMB_DMeffect.gif|align:center|350]]
> 
> As we can see, as the [[Dark Matter|dark matter]] increases and decreases, the overall amplitude of the power spectrum changes (in association with the $\Omega_{M}$ parameter). When we lower the DM density, the [[Baryon Acoustic Oscillations|baryon-loading]] effect is reduced such that the 3rd peak is enchanced.


**Dark Energy / Cosmological Constant Density** ($\Omega_{\Lambda}$)

We define $\Omega_{\Lambda} = 1-\Omega_{k} - \Omega_{M} - \Omega_{r}$ , but I thought the fact that they all sum to 1 was confusing? Not sure. If we assume $\Omega_{k} \sim 0$ can use location of first peak to get $H_0$ . This one is unclear.

**Radiation Density** ($\Omega_{r}$)

Actually doesn't show up here, but if we know $H_0$ then we can calculate this directly from the CMB temperature since we know how radiation energy density scales with $T$.

## Sunyaev-Zeldovich Effect

[[Inverse-Compton Scattering|Inverse-Compton scattering]] of the CMB photons by high-energy electrons. The biggest effect occurs on small scales (large $l$) as the CMB photons pass through some object with a small angular size on the sky. (like a galaxy cluster).

This scattering causes a deficit in the expected CMB signal at these scales, since the photons aren't CMB [[Blackbody radiation#Blackbody radiation|blackbody]] energies anymore.

![[sz.png|align:center|500]]

![[SZ_infographic.gif|align:center|500]]

#### Thermal SZ-Effect
*(from $e^-$ temp)*

The upscattering of CMB photons by electrons in hot, ionized gas (e.g. in [[Intracuster Medium|ICM]] of a [[Galaxy Cluster|galaxy cluster]]) by [[Inverse-Compton Scattering|inverse-compton scattering]]. This effect results in redshift-independent temperature fluctuations of...

$$\delta T / T_{CMB}\simeq 10^{-3}$$

The shift moves the spectrum to higher frequencies as follows (from Megans notes)
 
 ![[SZ_thermal.png|align:center|650]]
 
 **Usage?**
- Easy to detect high $z$ galaxy clusters (with [[Instruments#SPT|SPT]] for example).
- Used to estimate cluster masses and pressure profiles.

#### Kinetic SZ-effect
*(from bulk $e^-$ motion)*

When photons scatter off electrons (as with the thermal SZ) moving relative to the CMB rest frame, the doppler shift due to this relative motion induces an additional change in power. However, this change in power is on such a small scale in comparison to the thermal SZ effect, its hard to disentangle them.

In principle can determine peculiar velocities of the galaxy clusters; peculiar meaning 'with respect to the CMB rest frame'. The magnitude of this effect is... 

$$\frac{\delta T}{T} = - \frac{v_p}{c}\tau$$

...where $v_p$ is the peculiar velocity and $\tau$ is the [[Optical depth]].

![[SZ_kinectic.jpeg|align:center|400]]

**Usage?**
- probe cosmology and apply constraint to [[Hubble#Hubble Constant]]?
- Study large scale structure

## Sound Horizon

Here, we are calculating of the size of the sound horizon relating to the [[#CMB power spectrum]]. Before [[Cosmological Timeline#Recombination|recombination]], the photon-baryon fluid was dominated by [[Stellar Structure#Radiative Energy Transport|radiation pressure]] (but not necessarily a radiation-dominated universe), so the sound speed is...

$$P_{rad} = \frac{1}{3}\rho c^2 \implies c_s = \sqrt{\frac{\partial P}{\partial \rho}} = \frac{c}{\sqrt{3}}$$

However, this ignores a factor of the ratio of baryon and radiation energy densities that makes it really $\sim c/\sqrt{6}$. 

We can estimate the [[Distances#Comoving distance|comoving size]] of the sound horizon ($\chi_{\rm s}$) by the distance that sound can travel from the Big Bang ($t = 0$) to the time of recombination ($t_{\rm rec}$). Here, we substitute the [[Friedmann Equation]] into the relation.

$$\chi_{\rm s} \simeq \int_{0} ^{t_{\rm rec}} \frac{\rd t}{a(t)} \, c_{\rm s} \simeq \int_{0}^{t_{\rm rec}} \frac{\rd t}{a(t)} \fpar{c}{\sqrt{3}} = \frac{d_{H}}{\sqrt{3}} \int_{z_{\rm rec}}^{\infty} \frac{\rd z}{E(z)}$$

If we assume the early universe is matter-dominated ($\Omega_{M}=1$ and $\Omega_{\Lambda}=\Omega_{r}=\Omega_{k}=0$), this results in the following comoving size of the sound horizon.

$$\chi_{\rm s} \simeq \frac{d_{H}}{\sqrt{3}} \int_{z_{\rm rec}}^\infty \frac{\rd z}{\sqrt{\Omega_{M}}}(1+z)^{-3/2} = \frac{2 d_{H}}{\sqrt{3 \Omega_{M}}} (1 + z_{\rm rec})^{-1/2}$$

The [[Distances#Proper Distance|proper length]] of the sound horizon at recombination is then...

$$L_{\rm s}(z_{\rm rec}) = a(z_{\rm rec})\chi_{\rm s}(z_{\rm rec}) = \frac{2 d_{H}}{\sqrt{3 \Omega_{M}}}(1 + z_{\rm rec})^{-3/2}$$

...where the associated angular size that could be measured today (at $z=0$) is given in terms of the [[Distances#Angular diameter distance|angular diameter distance]].  $d_{\rm sls}$ is the [[Distances#Comoving distance|comoving distance]] to the *surface of last scattering* at $z_{\rm rec}$.

$$\theta_{\rm s} = \frac{L_{\rm s}}{d_{A}(z_{\rm rec})} = \frac{L_{\rm s} (1+z_{\rm rec})}{d_{\rm sls}} \hRightarrow d_{\rm sls}(z_{\rm rec}) =  \frac{c}{H_{0}} \int_{0}^{z_{\rm rec}} \frac{\rd z}{E(z)}$$

This yields an angular size of (see [this](https://physics.stackexchange.com/questions/54124/relation-between-multipole-moment-and-angular-scale-of-cmb) for relationship between $l$ and $\theta$)...

$$l_{\rm s} \sim \frac{\pi}{\theta_{\rm s}} \sim \text{(a number less than 220)}$$

***Note:** We get a speed sound ($c_{\rm s}$) that is too big, and thus, so is our $L_{\rm s}$ and $\theta_{\rm s}$. This leads to a "too small" $l_{\rm s}$. The right answer is about $l_{\rm s} \sim 220$. (see [this stackoverflow answer](https://physics.stackexchange.com/questions/450517/how-did-the-planck-study-calculate-the-angular-size-of-the-sound-horizon) or [caltech source](https://ned.ipac.caltech.edu/level5/Sept02/Reid/Reid5_2.html) )*

$$\boxed{ \; l_{\rm s} \simeq 220 \hspace{1cm} \theta_{\rm s} \simeq 1 \degree \;}$$


## CMB Polarization

An overview of the polarization of CMB photons we measure:
- Density perturbations ("scalar perturbations" arise from energy density fluctuations, see [these pages](https://w.astro.berkeley.edu/~mwhite/polar/node4.html) for overview) in the early universe produce **E modes** in the [[#CMB]] polarization map. Arise naturally from [[Thomson Scattering]] in a heterogeneous plasma. 
- There are also **B modes** in the CMB polarization map ("tensor perturbations" which are essentially gravitational waves). They can be created by two mechanisms: 
	1. [[Gravitational Lensing]] of E-modes, which has been measured by the [[Instruments#SPT|SPT]] in 2013
	2. [[Gravitational Waves]] arising from [[Cosmological Timeline#Cosmic Inflation]]
  
  Detecting the B-modes is extremely difficult, particularly as the degree of foreground contamination is unknown, and the weak gravitational lensing signal mixes the relatively strong E-mode signal with the B-mode signal

The names derive from an analogy to the decomposition of a vector field into curl-less  $\nabla \times \mathbf{E} = 0$ (here "E" for electric field) and divergence-less $\nabla \cdot  B = 0$ ("B" for magnetic field) components. The vector field of CMB polarization vectors on the sky is a vector field, and we decompose it (see Helmholtz decomposition) into curl-less and divergence-less components:

![[E_B_modes.png|aling:center|400]]

Performing this decomposition on the CMB polarization map gives us two panels, a mock map would look like the following, where red is CMB temperature hotspots and blue is cold spots.

![[e-mode-b-mode_measurement.png]]

> [!note]
> (Very) loosely, the B modes couple to gravitational waves because they have a quadrupole moment, but the E modes are too symmetric.

