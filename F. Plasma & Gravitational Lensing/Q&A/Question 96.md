### Question
---
Qualitatively, how does a gravitational lens work? Explain what needs to be measured to use a gravitational lens system to measure the Hubble constant. What is the current status of these determinations of $H_{0}$?

### Answer
---
##### Qualitatively, how does a gravitational lens work?

![[Gravitational Lensing#How does it work?]]

##### Explain what needs to be measured to use a gravitational lens system to measure the Hubble constant.

Using our geometric image above, we can imagine a pulse of light being emitted from the source. As the observer, we will experience a time delay between arrival of the light on the red path and the light on the blue path. 

There are two sources for this time delay:
1. Geometry of the System - the light paths have different lengths (unless lens and source are aligned on line-of-sight)
2. Shapiro time delay (see [[Question 97|97]]) - gravitational time dilation due to the presence of massive objects

The overall net delay can be expressed as...

$$\Delta t = \underbrace{\frac{1 + z_{\rm lens}}{c} \left(\frac{D_{L} D_{LS}}{D_{S}}\right)}_{D_{\Delta t} \, \propto \, H_{0}^{-1}} \bigg( \; \underbrace{\frac{1}{2} \left(\theta - \theta_{S} \right)^{2}}_{\rm geometric} - \psi_{\rm 2D} \bigg)$$

...where $\psi_{2D}$ is the 2D lensing potential related to the Shapiro time delay ([[Question 97]]). The term outside the parentheses is related to the [[Redshift#Cosmological Expansion|cosmological redshift]] where the "effective luminosity distance" a similar to the [[Distances#Angular diameter distance|angular diameter distance]], which depends on the Hubble Constant ($H_{0}$).

##### What is the current status of these determinations of $H_{0}$?

The current estimates come from HoLiCOW, which measures time delays from lensed [[Active Galactic Nuclei#Quasar|quasars]]. Their current value is...

$$H_{0} = 73.3_{-1.8}^{+1.7} \; \pu{km s^{-1} Mpc^{-1}}$$

...which has $5.3\sigma$ tension with the [[Cosmic Microwave Background|CMB]] measurements made from [[Instruments#Planck]]. 

HOLiCOW uses the following observatories:
- [[Instruments#HST|Hubble Space Telescope]]
- [[Instruments#Spitzer|Spitzer Space Telescope]]
- [[Instruments#Subaru|Subaru Telescope]]
- Canada-France-Hawaii Telescope
- [[Instruments#Gemini|Gemini Observatory]]
- [[Instruments#Keck|W. M. Keck Observatory]]