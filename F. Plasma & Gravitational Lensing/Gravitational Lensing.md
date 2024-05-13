---
banner: "![[plasma.png]]"
banner_y: 0.5
aliases:
---
> [!note] Sources:
> - https://arxiv.org/pdf/astro-ph/9606001.pdf
> - https://lweb.cfa.harvard.edu/~dfabricant/huchra/ay202/lectures/lecture12.pdf

## How does it work?

When we see light, we assume its source is in the direction the light came from; however, light can be bent by optics like lenses and mirrors. So if we identify a lens along the path of propagation, we can infer that the source may not be where it appears to be.

For tabletop optics, this is simple enough, but General Relativity tells us that light doesn't travel in "straight lines" in the way we are used to. Instead, light follows the contours of spacetime, such that it can be bent around gravitational wells from large masses. 

Therefore, large collections of mass like [[Galaxy Cluster|galaxy clusters]] and compact objects can thus act as massive astronomical lenses, making objects appear in positions they are not (if we had erroneously made the assumption that light is not bending). 

![[lensing_spactimeCurve.jpeg|align:center|500]]

In a more geometric picture...

![[lensing_diagram.png|align:center]]

...we can define a set of characteristic angles and lengths in a gravitational lensing system.

$$
\begin{aligned}[t]
	\theta_{1} &\equiv \text{image 1 angle} \\
	\theta_{2} &\equiv \text{image 2 angle} \\
	\theta_{S} &\equiv \text{true source angle} \\
	\theta~ &\equiv \text{angular lens size}
\end{aligned}
\hspace{2cm}
\begin{aligned}[t]
	r &\equiv \text{size of lens} \\
	D_{L} &\equiv \text{distance to lens} \\
	D_{S} &\equiv \text{distance to source} \\
	D_{LS} &\equiv \text{distance between source and lens}
\end{aligned}
$$
$$\alpha \equiv \text{deflection angle} = \frac{4 G M}{r \, c^{2}}$$

The "deflection angle" ($\alpha$) is set by the [[General Relativity#Schwarzschild Metric]] in general relativity (derivation found [here, chp 1.2](https://www.ita.uni-heidelberg.de/~jmerten/misc/meneghetti_lensing.pdf)). For most of these angles, the distance scales are large enough compared to the objects' sizes such that we can use the small angle approximation.

$$
\begin{aligned}[t]
	r &= D_{L} \, \tan \theta \\
	r &\approx D_{L} \, \theta
\end{aligned} 
\hspace{2cm} 
\begin{aligned}[t]
	D_{LS} \, \tan \alpha &\approx D_{S} \, \tan \theta_{1} \\
	D_{LS} \, \alpha &\approx D_{S} \, \theta_{1}
\end{aligned}
$$

If the "true source angle" is zero ($\theta_{S} = 0$) such that the source and lens are aligned along the line-of-sight, then we see a perfect ring of images of the source around the lensing object called the **Einstein Ring** with radius ($r=R_{E}$) and angular size ($\theta_{E}$, "Einstein angle"). Through some geometry, we can define these quantities in terms of distance parameters.

$$\theta_{1} = \left(\frac{D_{LS}}{D_{S}}\right) \alpha = \left(\frac{D_{LS}}{D_{S}}\right)\frac{4 G M}{r \, c^{2}} = \left(\frac{D_{LS}}{D_{S} \, D_{L}}\right)\frac{4 G M}{c^{2}} \frac{1}{\theta}$$

$$
\theta = \cancelto{0}{\theta_{S}} + \theta_{1} \equiv \theta_{E}\hspace{1cm} \Rightarrow \hspace{1cm} \theta_{E}= \left(\frac{D_{LS}}{D_{S} \, D_{L}}\right)\frac{4 G M}{c^{2}} \frac{1}{\theta_{E}}
$$
$$\boxed{ \; \theta_{E} \equiv \sqrt{\left(\frac{D_{LS}}{D_{S} \, D_{L}}\right)\frac{4 G M}{c^{2}}} \; } \hspace{2cm} R_{E} = \theta_{E} D_{L}$$

We can also express an approximation of the Einstein angle as... 

$$\theta_{E} \; {\rm [mas]} \simeq \sqrt{\frac{M \; {\rm [M_{\odot}]}}{10 \, D \; {\rm [kpc]}}} \hspace{1cm} \text{where} \hspace{1cm} D = \left(\frac{D_{L}D_{S}}{D_{LS}}\right) \equiv \text{effective lensing distance}$$

If we re-write the lens equation in terms of $\theta_{E}$ ...

$$
\frac{\theta_{E}^{2}}{\theta_{1}} = \left[ \; \frac{\left(\frac{D_{LS}}{D_{S} \, D_{L}}\right)\frac{4 G M}{c^{2}}}{\left(\frac{D_{LS}}{D_{S} \, D_{L}}\right)\frac{4 G M}{c^{2}} \frac{1}{\theta}} \; \right] = \theta
\hspace{1cm} \Rightarrow \hspace{1cm}
\boxed{ \; \theta_{S} = \left( 1 - \frac{\theta_{E}^{2}}{\theta^{2}} \right) \,\theta \; }
$$

...then we can categorize the strength of the lensing based on the angular position of the source strength.

- [[#Weak Lensing|Weakly Lensed]] ($\theta_{S} > \theta_{E}$) :
	- There are small deflections angles that distort the image's position and shape. (invertible, one-to-one mapping)
- [[#Strong Lensing|Strongly Lensed]] ($\theta_{S} < \theta_{E}$) :
	- There are large deflections angles that generate multiple images of the source. (non-invertible, one-to-many mapping)

## Types of Lensing

### Microlensing
*(Also see Exoplanet Detection Methods: [[Detection Methods#Microlensing Method]])*

**Microlensing** occurs when a compact/massive object passes in front of a background source, lensing it to the observer. Often, the lens mass is too low (mass of a planet or a star) for the image displacement and time delay *(see [[Question 96]])* of light to be observed easily, but the apparent brightening of the source may still be detected.

The method is commonly used to find an exoplanets, brown dwarfs, and compact objects ([[Black Hole|BH]] & [[Neutron Star|NS]], [[Dark Matter#MACHOs]]) we wouldn't have been able to see otherwise.

> [!bonus] Why "microlensing"?
> 
> The name "microlensing" comes from the fact that it's applied to sources with angular size of $\theta \sim (10^{-6})'' \; {\rm \left[ microarcseconds \right]}$.
> 
> For galaxy sized objects, angular size is $\sim (10^{-3})'' \; {\rm \left[ milliarcseconds \right]}$.
> 
> For galaxy cluster objects, angular size is $\sim 1'' \; {\rm \left[ arcseconds \right]}$

> [!image] Lensing Diagram
> 
> ![[lensing_micro.gif|align:center|550]]
> 
> In the image above, the gravitational lensing would be small enough that the "image" sources would appear to approximately be the same position as the "true" source, such that the light bending would not resolvable as in the animation. However, the Lorentzian light curve could still be visible as the background source it brightened.

**Observational Results:**
- Discovered the first isolated [[Black Hole|black holes]].
- Discovered that lensing effects are achromatic, meaning that we can observe in multiple frequency bands to break degeneracy with stellar variability observations.
- It can be used in [[Detection Methods#Microlensing Method|exoplanet detection]], provided the planets is near the Einstein angle of the lensing (foreground) star. 
	- Learn about orbital timescale (period)
	- Learn (maybe) about planet's mass from height of light curve peak, but this is degenerate with the semi-major axis and the orbital speed
- Microlensing is relatively rare and highly time-sensitive
	- Must do large surveys of many stars with high cadence to find microlensing events
		- EKOS - search of bulge, spiral arms, [[Galaxies - General#Large Magellanic Cloud|LMC]], and [[Galaxies - General#Small Magellanic Cloud|SMC]] (1993 - 2002)
		- MACHOS - search of bulge and [[Galaxies - General#Large Magellanic Cloud|LMC]] (1993-1999)
		- OGLE - search of bulge, [[Galaxies - General#Large Magellanic Cloud|LMC]], and [[Galaxies - General#Small Magellanic Cloud|SMC]] (1992 - current)
	- There are dedicated follow-up groups that provide dedicated and coordinated observations of selected events (e.g. PLANET)

> [!image] GAIA Observations
> 
> ![[lensing_microGAIA.gif|align:center|450]]
> 
> [[Instruments#GAIA]] sees microlensing events in the [[Galaxies - General#The Milky Way|Milky Way]], but not nearly enough to explain all the "missing mass" we attribute to [[Dark Matter]].

### Weak Lensing

**Weak Lensing** is the small deflection and distortion of lensed objects. It is not observable in a single source, but is found as a statistical effect on a distribution of background sources.

This is because the degree of lensing on any individual background source is not detectable, given they can have a variety of shapes and orientations. However, the statistical impact of many minor lensing events (e.g. way too many galaxies looking elliptical and stretched in one area) can be quantified over an image to constrain the distribution of smaller mass halos (lumps) in the foreground. The background source may also appear to be "lined up" along circles or arcs in a way that would be otherwise highly unlikely.

![[lensing_weak.png|align:center|450]]

> [!image] Caption
> The "shape noise" above refers to adding on a combination of real expected galaxy shapes and projection effects in a random way. Many galaxies will tend to look highly elongated or elliptical even without lensing, but this distribution of shapes is very well-understood from galactic observations and mathematical projections with random orientations.

**What do astronomers use weak lensing for?**
- Primarily, used in measuring [[Galaxy Cluster|galaxy cluster]] masses
	- Independent of mass type, and thus, sensitive to total mass distributions (baryon + dark matter)
	- Measurements exhibit a degeneracy (called the "mass sheet degeneracy") which can be broken with independent measurements of the magnification
- Measuring ellipticities of background galaxies in clusters and the "shear" from gravitational lensing
	- Need an accurate understanding of the "point spread function" (PSF) of the observing instrument
	- Need distance estimates for background sources (i.e. [[Redshift#Relativistic Doppler Effect|Relativistic Doppler Effect/Spectroscopic Redshift]])

> [!note]- [[Galaxy Cluster#Bullet Cluster|The Bullet Cluster]]
> 
> ![[lensing_weak_bulletCluster.png|align:center]]
> 
> A major result from weak lensing was the surface mass density mapping in the [[Galaxy Cluster#Bullet Cluster|bullet cluster]]. [[Instruments#CHANDRA]] provided strong evidence for an alternative massive and abundant species not coupled (in a detectable way currently) to electromagnetism (i.e. [[Dark Matter]]). Being able to distinguish the two species allows one to constrain the self-interaction cross section.

### Strong Lensing

**Strong Lensing** is the large deflection and distortion of lensed objects that allow background sources to have multiple images and arcs along the Einstein Ring around a large foreground gravitational lens.

In the example below, a [[Galaxy Cluster|galaxy cluster]] in the foreground is lensing many background objects, but produces clear multiple images of a background [[Active Galactic Nuclei#Quasar|quasar]] and a background galaxy.

![[lensing_strong.jpg|align:center|550]]

Strong lensing can also produce rings and arcs such as:

![[lensing_einsteinRing.JPG|align:center|550]]


The lensing "power" of a system can be thought of in terms of a mass density projected along the line of sight (like a column density). When the lens is thin compared to the observer-lens distance ($D_{L}$) and the lens-source distance ($D_{LS}$), we can define this projected, surface mass density ($\Sigma$) as...

$$\Sigma(\vec{r}) = \int \rho(\vec{r}, z) \; \mathrm{d} z \hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}
	\left[ \Sigma \right] &\equiv \text{surface mass density} = {\rm kg\ m^{-2}} \\
	\vec{r} &\equiv \text{radius from center of lens} \\
	\rho &\equiv \text{volume mass density}
\end{aligned}$$

The deflection angle (see [[#How does it work?|geometric diagram]]) is then expressed as...

$$\vec{\alpha}(\vec{r}\,) = \frac{4 G}{c^{2}} \int \frac{\left( \vec{r} - \vec{r}^{\ \prime} \right) \; \Sigma \left( \vec{r}^{\ \prime} \right)}{\left| \vec{r} - \vec{r}^{\ \prime} \right|^{2}} \; \mathrm{d}^{2} r^{\prime}$$

...where the angle is represented as a vector ($\vec{\alpha}$) because lensing effect is not only dependent on size of the lens ($\vec{r}$) by its magnitude, but by its direction. This expression becomes a scalar when assuming more symmetry.

It is common to discuss discuss the surface density ($\Sigma$) relative to some critical density ($\Sigma_{\rm crit}$), above which, "we expect lensing" and below which, "we don't expect lensing". *This critical density is the mean surface density enclosed within the Einstein radius.* 

$$
\Sigma_{\rm crit} = \frac{c^{2}}{4 \pi G} \left(\frac{D_{S}}{D_{LS} D_{L}}\right)
\hspace{1cm} \Rightarrow \hspace{1cm}
\begin{cases}
	\Sigma > \Sigma_{\rm crit} &\quad \text{expect lensing} \\
	\Sigma < \Sigma_{\rm crit} &\quad \text{don't expect lensing}
\end{cases}
$$

The relative mass density is called the *"convergence"*. 

$$
\kappa(\vec{\theta}) = \frac{\Sigma(\vec{\theta})}{\Sigma_{\rm crit}}
\hspace{1cm} \Rightarrow \hspace{1cm}
\begin{cases}
	\kappa > 1 &\quad \text{expect lensing} \\
	\kappa < 1 &\quad \text{don't expect lensing}
\end{cases}
$$

> [!image] Strong Lensing of a Single Object
> 
> ![[lensing_strong_lightcurve.gif|align:center|450]]
> 
> Here, we are observing the progression the the background star (the red circle) from the perspective of the foreground star (yellow star). This is done such that the host/foreground star, the Einstein Ring (green circle) is stationary in the image. The blue color represents the distortion of the background image as it is being lensed.
> 
> This perspective could be reversed of course, such that the foreground star is moving and a similar effect is produced.

> [!bonus]- Fun Facts!
> 
> 1) The number of images produced is governed by the "odd number theorem"  of differential topology. It states *"the number of multiple images produced by a bounded transparent lens must be odd"*.
> 
> 2) This theorem was not believed to be observable back in the 1930s when galaxies were believed to have masses of $10^{9} \; {\rm M_{\odot}}$. Zwicky then demonstrated that their mass was much larger by the [[Virial Theorem]] in the [[Stellar Clusters|cluster]], arguing this would produce images at a sufficient distance from the lens to be resolvable.
> 
> 3) Zwicky predicted that (I cant find the reference actually) about 1 in 100 bright high-redshift sources would be lensed in a manner detectable in principle by a foreground galaxies. Turns out to be pretty much correct. More distant means more intervening galaxies, increasing chances of lensing (but has to be bright so a [[Active Galactic Nuclei#Quasar|quasar]] is an ideal candidate, also because it is compact and so multiple images can more easily be resolved).

**What do astronomers use strong lensing for?**
- To constrain the masses of objects acting as gravitational lenses
	- Parametric Fitting: one method is to assume there are $N$ halos and let their masses and positions be fit parameters
- Act as cosmological magnifying glasses, allowing us to see much fainter objects if they happen to lie behind lenses, since more of their light is focused toward us. 
	- Most effective when the background objects lie on curves of very high magnification. 
- To map out the spatial distribution of underlying dark matter that we could not see otherwise
	- This can be less powerful than [[#Weak Lensing]] for large scale mapping