### Question
---
How does an X-ray telescope image? Why is it necessary to have the reflection take place at grazing angles of incidence?

### Answer
---
[[Electromagnetic Spectrum|X-rays]] don't usually reflect off of materials. For dense materials they get absorbed, and for less dense materials they pass straight through. However, they can be reflected for very large angles of incidence ("grazing incidence"). 

![[angle-of-incidence-cropped.svg|align:center|400]]

![[grazing_incidence.jpg|align:center|400]]

*(In an analogous sense, if you drop a stone in a pond, it will fall down through the water, but if you throw it quickly at grazing incidence, it can skip across the surface.)* 

Therefore, to image X-ray emission, we focus the beams by slowly increasing the angle of the mirrors along the path of propagation. However, by turning the mirrors on the side, the telescope misses a lot of X-rays. To solve this problem, X-ray telescopes use cylindrical mirrors and nest them, one inside the other.

![[xray_telescope_1mirror.jpg|align:center|450]]
![[xray_telescope_multimirror.jpg|align:center|450]]

> [!note] 
> This geometry is the reasoning that x-ray telescopes have such long "booms". They allow the detector/sensor to be much further away from the mirror configuration. For example, [[Instruments#CHANDRA]] has a $\sim 10 \; {\rm m}$ separation.
> 
> ![[chandra.png|align:center]]

There are 3 geometric configurations proposed for x-ray astronomy.

- **Wolter Type I** (most commonly used, [[Instruments#CHANDRA]]) ![[wolter_typeI.jpg|align:center|350]]
- **Wolter Type II** (used as narrow-field imager) ![[wolter_typeII.jpg|align:center|350]]
- **Wolter Type III** (never used) ![[wolter_typeIII.jpg|align:center|350]]

> [!note]
> - The mirrors are often coated in gold or nickel since X-rays reflect best off of high-$Z$ metals. 
> - When observing X-rays with a [[Tools#CCD|CCD]] sensor, the incident photon energy is about equal to the energy released when hitting the detector
> 	- More electrons released upon impact
> 	- We can count the number of electron to get low frequency-resolution spectra for "free".