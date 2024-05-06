### Question
---
With what velocity precision must one measure the reflex motion of a sun-like star to detect an Earth-mass planet in a 1-year orbit about it? What astrophysical processes complicate the measurement of radial velocities with this precision?

### Answer
---
##### With what velocity precision must one measure the reflex motion of a sun-like star to detect an Earth-mass planet in a 1-year orbit about it?

Using the **binary mass function** (derived [[Binary Stars#Spectroscopic Binary|here]] and at the end of [[Question 8]]), we can approximate that the planet's mass is much smaller than the star's mass ($M_{\rm p} \ll M_{*}$) and apply the values in the question.

$$
v_{\rm r,*} \sim \fpar{2 \pi G}{P}^{1/3} \fpar{M_{\rm p} \sin i}{M_{*}^{2/3}}
\hWhere \left\{ \; 
\begin{aligned}
	G &= 6.675 \times 10^{-11} \; {\rm \tfrac{N \cdot m^{2}}{kg^{2}}} &\, &\sim 10^{-11} \; {\rm \tfrac{N \cdot m^{2}}{kg^{2}}} \\
	P &= 1 \; {\rm yr} &\, &\sim \pi \times 10^{7} \; {\rm s} \\
	i &= \pi / 2 &\, &= \pi / 2 \\
	M_{*} &= 1 \; {\rm M_{\odot}} = 1.989 \times 10^{30} \; {\rm kg} &\, &\sim 10^{30} \; {\rm kg} \\
	M_{\rm p} &= 1 \; {\rm M_{\oplus}} = 5.972 \times 10^{24} \; {\rm kg} &\, &\sim 10^{24} \; {\rm kg} \\
\end{aligned} \right.
$$
$$v_{\rm r,*} \sim \fpar{10^{-11}}{10^{7}}^{1/3} \fpar{10^{24}}{(10^{30})^{2/3}} \sim 10^{-2} \; {\rm m/s} \sim 1 \; {\rm cm/s}$$

We find that we would need approximately ${\rm cm/s}$ velocity resolution (assuming circular orbit with maximum inclination). Otherwise, we would not be able to see any significant change over an orbit. At the moment, no instrument is able to achieve this precision. 

The best precision we have so far is $\sim 0.3 \; {\rm m/s}$ for ESPRESSO on the [[Instruments#VLT]], with the goal to push to $0.1 \; {\rm m/s}$. That means we could observe a planet with mass $\sim 10 \; {\rm M_{\oplus}}$

##### What astrophysical processes complicate the measurement of radial velocities with this precision?

> [!note]
> Recall that [[Detection Methods#Radial Velocity Method|radial velocities]] are measured with spectrum.

- Stellar Activity: the material within the star is moving, causing noise in the spectra to appear.
- Atmospheric Seeing: turbulence in the earth's atmosphere leads to additional noise in spectrum for ground-based observatories
- Need high-resolution spectrometer
- Very hot stars ([[Spectral Classes#O]], [[Spectral Classes#B]], [[Spectral Classes#A]]) may not have enough narrow lines in their spectra for precise Doppler shift measurements.
- Need to understand the motion of Earth in the Solar system relative to the star down at the $\sim {\rm cm/s}$ precision.