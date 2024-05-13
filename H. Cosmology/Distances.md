---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
---
Sources:
- https://arxiv.org/abs/astro-ph/9905116
- https://www.wikiwand.com/en/Comoving_and_proper_distances


> [!key-idea] Quick Reference
> 
> $$\mathrm{d} x = c \; \mathrm{d} t \quad , \quad \mathrm{d} x  = a(t) \; \mathrm{d} \chi \hspace{1cm} \text{where} \hspace{1cm} \begin{aligned} \mathrm{d} x &\equiv d_{p} \equiv \text{proper distance} \\ \mathrm{d} \chi &\equiv d_{C} \equiv \text{comoving distance} \end{aligned}$$

## Comoving Distance

The **comoving distance** ($\mathrm{d} \chi \equiv d_{C}$) is the distance between two points in spacetime after we have factored out the expansion of universe.

The comoving coordinate system is invariant under the [[Hubble#Hubble Law|Hubble Flow]], such that it evolves "with"  the expansion of the universe. Meaning, if two objects only moving with the [[Hubble#Hubble Law|Hubble Flow]] (relative to each other) in proper space, they they will have constant comoving distance over cosmological time. Hence, it is **not measurable through observations.**

The comoving distance is related to the [[#Proper distance|proper distance]] by...

$$\mathrm{d} x = a(t) \, \mathrm{d} \chi \hspace{1cm} \Longleftrightarrow \hspace{1cm} d_{p} = a(t) \, d_{C}$$

...where the scale factor ($a(t)$) is determined by the [[Friedmann Equation#Friedmann Equation]] at the time ($t$) of observation.

> [!note] 
> We define $a$ such that in the present day, the comoving and proper distances are equal.
> $$\text{Today's Values:} \hspace{1.5cm} a = 1 \hspace{1cm},\hspace{1cm} z = 0$$

To calculate the comoving distance, we can integrate over time ($t$), the scale factor ($a$), or the redshift ($z$), where $d_{H}=c/H_{0}$ is the [[Hubble#Hubble Distance]]. 

$$d_{C} = \int_{t_{\rm emt}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)} \hspace{1.5cm} d_{C} = d_{H} \int_{a_{\rm emt}}^{a_{\rm obs}} \frac{\mathrm{d} a}{a^{2} \, E(a)} \hspace{1cm} \underbrace{d_{C} = d_{H} \int_{z_{\rm obs}}^{z_{\rm emt}} \frac{\mathrm{d} z}{E(z)}}_{\text{note the switched integration bounds}}$$

> [!derivation]-
> 
> The comoving distance is equivalent of the $r$ coordinate in the [[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric|FLRW metric]] (in a flat universe) measured along a null geodesic between points in spacetime where $t_{\rm emt}$ and $t_{\rm obs}$ are the time coordinate values when the light is emitted and observed, respectively.
> 
> We'll do the derivation for a flat universe, but it holds (with more complicated expressions, see [this page](https://www.wikiwand.com/en/Comoving_and_proper_distances)) even for a non-flat universe. 
> 
> For a radial light ray ($d\mathbf{\Omega} = 0$, $d\tau = 0$) in the [[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric|FLRW metric]] in a flat universe, we have...
> 
> $$c \; \mathrm{d} t = a(t) \; \mathrm{d} r$$
> 
> ...such that the comoving distance $d_{C} \equiv r$ between light emitted at $t_{\rm emt}$ and observed today at $t_{\rm obs}$ is...
> 
> $$d_{C} \equiv r = \int_{t_{\rm emt}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)}$$
> 
> Using the definition of the [[Friedmann Equation#With the Cosmological Density Parameters...|Hubble parameter]], we can express this integral in terms of the scale constant ($a$).
> 
> $$H = \frac{\dot{a}}{a} = \frac{\mathrm{d} a}{\mathrm{d} t} \frac{1}{a} \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} t= \frac{1}{H} \frac{\mathrm{d} a}{a}$$
> $$r = \int_{t_{\rm emt}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)} = \int_{a_{\rm emt}}^{a_{\rm obs}} \frac{c \; \mathrm{d} a}{a^{2} H(a)} = \frac{c}{H_{0}} \int_{a_{\rm emt}}^{a_{\rm obs}} \frac{\mathrm{d} a}{a^{2} E(a)}$$
> 
> And similarly, by using the relationship between the [[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric|scale factor and redshift]], we can express this integral in terms of the redshift ($z$).
> 
> $$a(z) = \frac{1}{1+z} \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} a = -\frac{\mathrm{d} z}{(1+z)^{2}} = -a^{2} \; \mathrm{d} z$$
> $$r = \frac{c}{H_{0}} \int_{t_{\rm emt}}^{t_{\rm obs}} \frac{\mathrm{d} a}{a^{2} E(a)} = - \frac{c}{H_{0}} \int_{z_{\rm emt}}^{z_{\rm obs}} \frac{\mathrm{d} z}{E(z)} = \frac{c}{H_{0}} \int_{z_{\rm obs}}^{z_{\rm emt}} \frac{\mathrm{d} z}{E(z)}$$
> 
> In summary, we can express the comoving distance in terms of time ($t$), scale factors ($a$), or redshift ($z$), where $d_{H}. = c/H_{0}$ is the [[Hubble#Hubble Distance]].
> 
> $$\boxed{d_{C} = \int_{t_{\rm emt}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)}} \hspace{1.5cm} \boxed{d_{C} = d_{H} \int_{a_{\rm emt}}^{a_{\rm obs}} \frac{\mathrm{d} a}{a^{2} \, E(a)}} \hspace{1cm} \underbrace{\boxed{d_{C} = d_{H} \int_{z_{\rm obs}}^{z_{\rm emt}} \frac{\mathrm{d} z}{E(z)}}}_{\text{note the switched integration bounds}}$$

The comoving distance between two events at the same redshift or distance but separated on the sky by some angle $(\delta \theta)$ can be defined using the **transverse comoving distance** or **curvature function**; a function describing the curvature of spacetime ($k$).

$$f_{k}(\chi) = \begin{cases}
	\frac{1}{\sqrt{k}} \, \sin \left( \chi \,\sqrt{k} \right) &\quad {\rm for} \quad k>0 \quad , \quad \Omega_{k}<0 \quad {\rm (closed)} \\
	\chi &\quad {\rm for} \quad k=0 \quad , \quad \Omega_{k}=0 \quad {\rm (flat)} \\
	\frac{1}{\sqrt{|k|}} \, \sinh \left( \chi \,\sqrt{|k|} \right) &\quad {\rm for} \quad k<0 \quad , \quad \Omega_{k}>0 \quad {\rm (open)}
\end{cases}$$
^curvature-function

Here, I have used $\chi \equiv d_{C}$.

## Proper Distance

The **proper distance** ($\mathrm{d} x \equiv d_{p}$) is the *instantaneous* distance between points in an expanding universe, which changes with the [[Hubble#Hubble Law|Hubble flow]]. 

The proper distance is related to the [[#Comoving Distance|comoving distance]] by...

$$\mathrm{d} x = a(t) \, \mathrm{d} \chi \hspace{1cm} \Longleftrightarrow \hspace{1cm} d_{p} = a(t) \, d_{C}$$

...where the scale factor ($a(t)$) is determined by the [[Friedmann Equation#Friedmann Equation]] at the time ($t$) of observation.

> [!note] 
> We define $a$ such that in the present day, the comoving and proper distances are equal.
> $$\text{Today's Values:} \hspace{1.5cm} a = 1 \hspace{1cm},\hspace{1cm} z = 0$$

If we go into the past, then $a$ is smaller, but the comoving distance is the same (as it is invariant under the Hubble flow). Therefore, the proper distances get smaller as we go into the past, similar to the [[#angular diameter distance]] in a flat universe.

## Angular Diameter Distance

The **angular diameter distance** ($d_{A}$) is defined as the ratio of an object’s [[#Proper Distance|proper]] transverse size ($\ell$) to its angular size ($\delta \theta$). 

![[angular_diameter_distance.png|align:center|350]]

At redshift ($z$) and using the *[[#^curvature-function|transverse comoving distance]]*, the angular diameter distance can be defined as...

$$d_{A} = \frac{\ell}{\delta \theta} = \frac{a(z) \, f_{k}(\chi) \, \delta\theta}{\delta \theta} = \frac{f_{k}(\chi)}{1+z} \hspace{1cm} \text{where} \hspace{1cm} \chi = d_{C}$$
$$f_{k}(\chi) = (1+z) \; d_{A}$$
In a flat universe ($k=0$), the angular diameter distance is simply given in terms of the [[#Comoving Distance|comoving distance]].

$$f_{k}(\chi) = \chi \equiv d_{C} \hspace{1cm} \Rightarrow \hspace{1cm} d_{A} = \frac{d_{C}}{1+z}$$

This distance measurement is commonly used to observe so called "standard rulers" (e.g. [[Cosmic Microwave Background|CMB]], [[Baryon Acoustic Oscillations|BAO]]). 

![[angular_diameter_redshift.jpg|align:center|400]]

The apparent angular size ($\delta \theta$) of an object at a fixed [[#Comoving Distance|comoving distance]] ($d_{C}$) exhibits a turnover at about redshift $z=1$. We can understand this turnover by thinking about the appearances of objects at different redshifts, in relation to the state of the expanding universe.

At low redshifts ($z \lesssim 1$), when objects move further away, they appear to the observer to become smaller and smaller, but eventually we get to a redshift ($z\sim 1$) where the universe was small enough that the object encompassed a significant portion of the sky, and so it starts to look larger again.

## Luminosity Distance

The **luminosity distance** is defined by the relationship between the intrinsic  [[Luminosity#Relationship to Flux|bolometric luminosity]] ($L$) of a distant object and its measured [[Flux#Bolometric Flux|bolometric flux]] ($F$).

$$L = F \cdot A = F \left( 4 \pi R^{2} \right) \hspace{1cm} \Rightarrow \hspace{1cm} d_{L} \equiv R = \sqrt{\frac{L}{4 \pi F}}$$

In terms of the [[#Comoving Distance|comoving distance]] and [[#Angular Diameter Distance|angular diameter distance]]...

$$d_{L} = (1+z) \; f_{k}(\chi) = (1+z)^{2} \; d_{A} \hspace{1cm} \text{where} \hspace{1cm} \chi \equiv d_{C}$$

If universe if flat ($k=0$), then this simplifies as $f_{k=0}(\chi) = \chi \equiv d_{C}$

$$d_{L} = (1+z) \; d_{C} = (1+z)^{2} \; d_{A}$$

> [!derivation]-
> 
> The [[Luminosity|luminosity]] can be defined in terms of wavelengths/frequencies by...
> $$L_{\rm obs} \sim \frac{h \nu_{\rm obs}}{\delta t_{\rm obs}}$$ 
> 
> Therefore, it is affected by the expanding universe via:
> 1. The energy of the photons is reduced with [[Redshift|redshift]] as $$\frac{\nu_{\rm emt}}{\nu_{\rm obs}} = \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \frac{a_{\rm obs}}{a_{\rm emt}} = 1+z$$
> 2. The arrival time between photons emitted at $t_{\rm emit}$ and $t_{\rm emt}+\delta t_{\rm emt}$ is adjusted as $$\frac{\delta t_{\rm obs}}{\delta t_{\rm emt}} = \frac{a_{\rm obs}}{a_{\rm emt}} = 1+z$$ since the light has a slightly different distance to travel.
> 
> The net effect is then...
> 
> $$L_{\rm obs} = \frac{h \nu_{\rm obs}}{\delta t_{\rm obs}} = L_{\rm emt} \left(\frac{a_{\rm emt}}{a_{\rm obs}}\right)^{2} = L_{\rm emt} (1+z)^{2}$$
> 
> ...such that the observed flux and the square root lead to the factor above.

