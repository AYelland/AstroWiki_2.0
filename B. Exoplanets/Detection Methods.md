---
banner: "![[exoplanets.png]]"
banner_y: 0.6
aliases:
---
**Total Number of Exoplanets Observed:** 5587 *(02/21/2024)* 

![[exoplanet_overview.png|align:center]]

*(From https://exoplanetarchive.ipac.caltech.edu/exoplanetplots/)*

## Transit Method
*(~3500 confirmed as of 2022)*

![[transit_method.gif|align:center|500]]
![[transit_method.png|align:center|500]]

Analyzing the changes in the light curve caused by the planet blocking the emitted light. If the planet passes in front of the star along the line of sight, we see a dip in the flux of light. The shape of the dip is approximately a trapezoidal form with curvy edges.

> [!note]
> *"primary transit"* - the planetary body passes in front of the star
> *"secondary transit"* - the planetary body passes behind the star

**Direct Observables:**
- Period
	- Measure the time between two transits
- Size of Planet
	- Determined from the primary transit
	- Compare the change in luminosity to the fraction of the observing disk covered by the planet
- Temperature of Planet (can in theory be observed)
	- Determined from the secondary transit
	- When the planet goes behind star, should see the subtraction of a [[Blackbody Radiation|blackbody spectrum]] at a certain temperature.
	- See [[Bonus#Bonus - Measuring the Planet's Temperature]].
- Density of Star
	- Can be calculated from the period and duration of a transit, by assuming that that the planet's orbit is circular and $M_{\rm p} \ll M_{*}$.
	- See [[Bonus#Bonus - Measuring the Stellar Density]].

**Biases:**
- Biased towards detecting larger planets with a smaller orbital radius.
	- Chance of getting a transit along a particular line-of-sight is very small for a planet far away
	- Larger planets produce significantly larger flux dips
- Increasing sensitivity in [[Photometry|photometric measurements]] reduces effect of biases
- Can only detect edge-on binary systems

## Radial Velocity Method
*(~1000 confirmed as of 2022)*

![[radial_velocity_method.gif|align:center|500]]

Measure the wobble of star (caused by gravitational influence of the planets) through the Doppler shifts in the spectra. First planet discovered with this method was 51 Peg b ($\sim {\rm M_{Jup}}$).

**Direct Observables:**
- Period
- Semi-Amplitude of Velocity Shift (i.e. radial velocity)
	- Gives a lower bound on mass (see [[Question 8]])
	- Helps determines obliquity of orbit (see [[Question 10]])

**Biases:**
- Biased toward large planetary masses.
	- Requires spectroscopy and measuring the shift of spectral lines $\implies$ Planets have to be large enough to significantly influence the host star's motion
- If low planetary mass, then we are biased to close in orbits
- Can't measure Earth-mass planets yet (see [[Question 9]]).

## Direct Imaging Method
*(~25 confirmed as of 2022)*

| ![[direct_imaging_method1.gif\|300]] | ![[direct_imaging_method2.gif\|300]] |
| :----------------------------------: | ------------------------------------ |
 *(\*\*\The two GIFs are of different systems)*

Directly observing the reflected light from a planet (coronagraphy). We assume that the star and planet emit as a [[Blackbody Radiation|blackbody]]. Then, we can then subtract the star's light from the image to observe the planet's spectrum (+ temperature).

**Direct Observables:**
- Radius of Orbit / Semi-Major Axis (if distance to system is known)
- Period of Orbit (if proper motion can be determined)

**Biases:**
- Biased towards detecting large and/or hot planets
	- Requires a high planet:star contrast.
	- The more blackbody flux a planet can emit $\implies$ the easier it is to observe.
	- Current observations are limited to [[Electromagnetic Spectrum|IR]] (in future, [[Instruments#Roman]] should allow [[Electromagnetic Spectrum|optical]])
- Biased toward long-period planets
	- Requires large separations to be able to resolve planet individually

## Microlensing Method
*(~100 confirmed as of 2022)*

| ![[microlensing_magnifcation.gif\|https://www.astronomy.ohio-state.edu/gaudi.1/movies.html\|250]] | ![[microlensing_lightcurve.gif\|https://www.astronomy.ohio-state.edu/gaudi.1/movies.html\|400]] |
| :--------------------------------: | :-------------------------: |
![[microlensing_method.jpg|align:center|550]]

> [!image] Image Caption
> 
> In the GIF on the top left, we are observing the progression the the background star (the red circle) from the perspective of the foreground star (yellow star). This is done such that the host/foreground star, the Einstein Ring (green circle) and the planet (the purple dot) is stationary in the image. The blue color represents the distortion of the background image as it is being lensed.

When a background source is lensed by a foreground star, a planet (which is inside or near the Einstein Ring of the foreground/host star) can briefly increase the brightness of the lensed light by the planet's own Einstein ring. This results in an additional spike contribution to the normally lensed star.

We need the planet to be close to the Einstein ring because we want the microlensing blip from the planet to show up during the lensing event of the star. If it closer to the host star, it won't produce a distinguishable lensing magnification. Similarly, if it is farther away from the host star, it will not be detected as well. 

*(Also see [[Gravitational Lensing#Microlensing]] for other important comments not here!)*

**Direct Observables:**
- Timescale of Orbit 
	- Requires accurate measurement of relative proper motion of lens-source/foreground system

**Biases:**
- Biased toward large-separation systems
	- Detection probability is maximized when separation of planet-star system is $\sim$ size of Einstein ring at that distance
- Measurements are mostly independent of mass of planet (also a positive)
- Highly transient systems, and thus, harder to observe


## Pulsar Timing Method

When there are small periodic changes in the [[Neutron Star#Pulsar|pulsar]] period, this can indicate the gravitational influence of a companion, such as an exoplanet. By taking precise measurements of the periodic changes, you can calculate some of the properties of the planetary kinematics.

Any exoplanet discovered by this method are poor candidates for life because they live next to a terrifying [[Neutron Star#Pulsar|pulsar]]. The first exoplanet was discovered with this method was in 1992 by Aleksander Wolszczan and Dale Frail.