---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
---
## Hubble Constant

As defined in the [[Friedmann Equation]], the **Hubble constant** represents the rate of expansion of the universe in the present day ($z=0$ || $a=1$).

$$H_{0} = H(z=0) = \frac{\dot{a}}{a}\Bigg|_{z=0} = \dot a(z=0) \hWhere a = \frac{1}{1+z}$$

> [!derivation]- Derivation from Expanding Sphere
> 
> If we consider some sphere with initial radius ($R_{0} \equiv R(t_{0})$) expanding over time to some later radius ($R(t)$), then we can compare the coordinates of some test point before ($\vec{r}_{0}$) and after ($\vec{r}$) the expansion.
> 
> ![[hubble_expandingSphere.png|align:center|350]]
> 
> $$\vec{r} = \underbrace{\fpar{R(t)}{R_{0}}}_{a(t)} \, \vec{r}_{0} = a(t) \, \vec{r}_{0} \hWhere a(t) \equiv \text{cosmic scale factor (today's value = 1)}$$
> 
> Using the time-derivative to only focus on the scale factors, we can define the Hubble parameter.
> $$\vec{r} = a(t) \, \vec{r}_{0} \hspace{1.5cm} \dot{\vec{r}} = \dot{a}(t) \, \vec{r}_{0} \hRightarrow H(t) = \left| \frac{\dot{\vec{r}}}{\vec{r}} \right| = \frac{\dot{a}(t)}{a(t)}$$

## Hubble Law

**Hubble's Law** describes how fast an object should be moving away from us. Given that [[Distances#Proper Distance|proper distances]] are related to [[Distances#Comoving Distance|comoving distances]] through the scale factor...

$$d_{p} = a \,d_{C}$$

...we know the radial velocity will increase as object will moving away from us in association with the Hubble flow (universal expansion).

$$v_{r} = \dot{d_{p}} = \dot{a} \, d_{C} = \left( H(t) a \right) \, d_{C} = H(t) \, d_{p}$$

Evaluating this for today value ($z=0$) and simplifying notation for current-day measurements, we express the Hubble flow as...

$$v = H_{0} d$$

We find this linear relationship and a value for the Hubble Constant when combining measurements of both distance (various methods) and radial velocity (usually spectroscopic redshift) of receding objects. 

![[hubble_law.png|align:center|400]]

We typically report the constant in units of $[ \pu{km s^{-1} Mpc^{-1}} ]$ so its easy to calculate a distance in $\pu{Mpc}$ or speed in $\pu{km s^{-1}}$ if the other is known.

## Hubble Time

![[Timescales#Hubble Time]]

## Hubble Distance

The Hubble distance is the distance spanned by light with the [[#Hubble Law|Hubble flow]].

$$d_{H} = c \, t_{H} = \frac{c}{H_{0}} \simeq 4.3 \; {\rm Gpc} \hspace{1cm} \text{for} \hspace{1cm} H_{0} = 70 \; \pu{km s^{-1} Mpc^{-1}}$$

## Methods of Measurement

### Distance Ladder (Standard Candles)

> [!space] Measured Hubble Constant: $\quad H_{0} \simeq 73 \pm 1 \; \pu{km s^{-1} Mpc^{-1}}$

![[distance_ladder.jpg|align:center|600]]

The most challenging part of measuring the Hubble constant is getting good accuracy on the distances. There are a variety of different methods used to measure distances to various objects on different scales, and many of then are dependent on prior measurement of closer objects. Together, these series of measurements form the "rungs" of the "cosmological distance ladder".

An example measurement involves: 
- Make observations of close objects of type $A$.
- Calibrate a relationship between the observational characteristics and the distances to objects $A$.
- Make observations of objects $A$ near some rarer object $B$.
- Infer distances to $B$ based on calibration of $A$.
- Calibrate $B$ and repeat, getting distances to some very distant objects $C$.

The current state of the cosmological distance ladder depends on...
- Pulsating Objects (like [[Stellar Classes#Cepheids]] and [[Stellar Classes#RR Lyrae]])
- "Standard Candles" of presumably known luminosity (like [[Stellar Explosions#Type Ia|Type Ia supernovae]] and the [[Hertzsprung-Russell Diagram#Helium Flash|helium flash]] at the tip of the [[Hertzsprung-Russell Diagram#Red Giant Branch (RGB)|RGB]])
- [[Velocity Dispersion#Tully-Fisher Relation]]

![[distance_ladder.png|align:center|550]]

> [!image] The diagram is explained in more detail [here](https://en.wikipedia.org/wiki/Cosmic_distance_ladder)

### Strongly-Lensed Quasars

> [!space] Measured Hubble Constant: $\quad H_{0} \simeq 73 \pm 2 \; \pu{km s^{-1} Mpc^{-1}}$

The H0LiCOW team measures time delays between multiple images of a [[Gravitational Lensing#Strong Lensing|strongly lensed]] background [[Active Galactic Nuclei#Quasar|quasar]] by a large foreground object. The time delay  ( $\sim \mathcal{O}({\rm seconds})$ ) can be used to infer a distance, independent of [[Cosmic Microwave Background|CMB]] and [[#Distance Ladder (Standard Candles)|distance ladder]] constraints.

### Standard Sirens

> [!space] Measured Hubble Constant: $\quad H_{0} \simeq 70 \pm 2 \; \pu{km s^{-1} Mpc^{-1}}$

Method co-invented by Scott Hughes here at MKI. 

To make this measurement, we need to compare two things: the distance to an object, and the apparent velocity with which it is moving away from us. 

Measuring the apparent (radial) velocity is the easy part: you measure the [[Redshift|redshift]] of light, given you have an electromagnetic spectrum of an object. This allows us to transform the [[#Chirp Mass|chirp mass]] from the detector frame to the source frame. ($M_{c} \to M_{c} (1 +z)$). *(with gravitational waves alone, you can’t do it — there isn’t enough structure in the spectrum to measure a redshift.)*

Measuring the distance is the tricky part; using the power emitted and the waveform of the merger, we can find the [[Gravitational Waves#Chirp Mass|chirp mass]],  [[Question 43#Give a qualitative description of the frequency and amplitude evolution of the gravitational wave signal from a binary compact star system.|chirp frequency & scaling amplitude]]. This is done through applying "standard" waveform templates (derived from GR) to a GW event. Then we can find the [[Distances#Luminosity Distance|luminosity distance]] ($R = d_{\rm L}$) to a GW merger.

$$h_{0} \propto \frac{\left[ M_{\rm c} (1+z) \right]^{5/3}\omega^{2/3}}{R} \hWhere R \equiv d_{L} = (1+z) \, d_{C}$$

Bringing both the distance and velocity together, we can estimate $H_{0}$.

> [!note] GW170817
> This is the first GW event with precise EM follow-up that allowed up to calculate the redshift and distance to a distant gravitational-wave source. And thus, allows us to use the "standard siren" for the first time.

### CMB Measurements

> [!space] Measured Hubble Constant: $\quad H_{0} \simeq 67 \pm 1 \; \pu{km s^{-1} Mpc^{-1}}$

By fitting the [[Cosmic Microwave Background#Power Spectrum|CMB power spectrum]] with the $\Lambda\rm{CDM}$ model, we can predict $H_0$ within the context of this model. By then combining with [[Baryon Acoustic Oscillations|BAO]] measurements, we can improve constraints on $H_{0}$.

### Hubble Tension

There's tension between different methods and the measured value of the Hubble Constant, $H_{0}$.

![[hubble_tension.png|align:center|600]]





