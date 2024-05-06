---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - magnitude
  - magnitudes
---
> [!measure] Typical Magnitudes
> 
> | Source | Apparent Magnitude ($m$) | Absolute Magnitude ($M$) |
> | :---: | :---: | :---: |
> | Sun | -27 | 4 |
> | Moon | -13 | 31 |
> | Sirius | -1.4 | 1.5 |
> | Quasar (Mrk 231) | 14 | -22 |
> 
> **Other orders of mangtiude:**
> - $6^{\rm th}$ Magnitude is the faintest star a human eye can see
> - $5^{\rm th}$ Magnitude for white dwarfs and exoplanets
> - $15^{\rm th}$ Magnitude for galaxy targets
> - $27^{\rm th}$ Magnitude limit for ground-based telescopes
> - $30+$ Magnitude is where [[Instruments#HST]] and [[Instruments#JWST]] observe at


## Apparent Magnitude

The **apparent magnitude** ($m$) is defined as how bright a source object appears relative to reference object. It is a measure of *"how much [[Flux]] do we observe"*. Since this quantity is depends on both the brightness of the object and its distance, it is *not* and intrinsic characteristic of a source.

$$\Delta m = m_{1} - m_{2} = -2.5 \log_{10} \fpar{(F_{\nu})_{1}}{(F_{\nu})_{2}}
\hWhere
\begin{aligned}
	(F_{\nu})_{1} &\equiv \text{source object flux} \\
	(F_{\nu})_{2} &\equiv \text{reference object flux}
\end{aligned}$$
$$\textcolor{gray}{\left[ \; \frac{(F_{\nu})_{1}}{(F_{\nu})_{2}} = 10^{-(m_{1} - m_{2})/2.5} \approx 2.512^{(m_{1} - m_{2})} \; \right]}$$

- If a source object is **brighter** (higher flux) than a reference object (lower flux), then is has a **lower** apparent magnitude.
- If a source object is **dimmer** (lower flux) than a reference object (higher flux), then is has a **higher** apparent magnitude.

There are two main reference object systems utilized in astronomy that allow us to specify a "zero-point" magnitude.
- [[#Vega Reference System]]
- [[#AB Reference System]]

Since the apparent magnitude of an object is dependent on the wavelength/frequency of light its being observed with, astronomers have also defined the...

- **monochromatic magnitude** - the magnitude of an object at a single wavelength
	$$\ m_{\nu, 1} - m_{\nu, 2} = -2.5 \log_{10} \fpar{(F_{\nu})_{1}}{(F_{\nu})_{2}}$$
	
- **band magnitude** - the magnitude spectrum of an object across many wavelengths. For these spectrum observations that use a a filter bandpass (such as the [[Photometry#UBVRI System]]), fluxes must integrated over the frequency band $X$ with a transmission function $T_X(\nu)$.
	$$\ m_{X, 1} - m_{X, 2} = -2.5 \log_{10} \fpar{ \int (F_{\nu})_{1} T_{X}(\nu) \; \rd\nu}{\int (F_{\nu})_{2} T_{X}(\nu) \; \rd\nu} = -2.5 \log_{10} \fpar{(F_{X})_{1}}{(F_{X})_{2}}$$
	Since in most observations you cannot single out a specific wavelength/frequency of light, the band magnitude is much more practical.

### Vega Reference System

The Vega reference system is calibrated using the flux of the AO V star Vega, $(F_{\nu})_{\rm Vega}$, which has a non-flat, flux distribution (i.e. the flux changes for different frequencies). With this calibration, the star Vega at magnitude of zero in all frequency bands. ($m_{\rm \nu, Vega} = 0$ and $m_{\rm X, Vega} = 0$)

$$
m_{\nu} = -2.5 \log_{10} \fpar{F_{\nu}}{(F_{\nu})_{\rm Vega}}
\hspace{2cm}
m_{X} = -2.5 \log_{10} \fpar{ F_{X}}{(F_{X})_{\rm Vega}}
$$

### AB Reference System

The AB reference system is calibrated to a hypothetical source with flux with a flat, flux distribution.

$$(F_{\nu})_{\rm AB} = 3.63\times10^{-20} {\rm erg}\ {\rm s}^{-1} {\rm cm}^{-2} {\rm Hz}^{-1}$$

Because the AB reference object gives a flat, flux distribution, $(F_{\nu})_{\rm AB} =$ constant, we can pair this with the normalization principle for the transmission function, $\int T_X(\nu)\rd\nu = 1$ such that...

$$\int (F_{\nu})_{\rm AB} T_X(\nu) \rd\nu = (F_{\nu})_{\rm AB} \int T_X(\nu) \rd\nu = (F_{\nu})_{\rm AB}$$

 This means, using this calibration allows us to immediately extract a constant in the apparent magnitude expression.
 
$$
\begin{align}
	m_{\nu} &= -2.5 \log_{10} \fpar{F_{\nu}}{(F_{\nu})_{\rm AB}} \\
	&= -2.5 \log_{10} (F_{\nu}) - 48.6
\end{align}
$$
$$
\begin{alignat}{2}
	m_{X} &= -2.5 \log_{10} \fpar{F_{X}}{(F_{\nu})_{\rm AB}} &\quad&\textcolor{gray}{= -2.5 \log_{10} \fpar{\int F_{\nu} T_X(\nu)\rd\nu}{(F_{\nu})_{\rm AB}}} \\
	&= -2.5 \log_{10} \left( F_{X} \right) - 48.6 &&\textcolor{gray}{= -2.5 \log_{10} \left( \int F_{\nu} T_X(\nu)\rd\nu \right) - 48.6}
\end{alignat}
$$

 > [!note] 
 > The spectral energy density of Vega is non-flat, flux distribution, it makes a weird magnitude system, so the AB magnitude system with a flat flux distribution makes a bit more sense.

### Converting between Vega and AB Systems

The value of the hypothetical source flux ($(F_{\nu})_{\rm AB}$)in the [[#AB Reference System]] was chosen such that the source has the same magnitude in the *V-band*.
$$m_{\rm X, AB} = m_{\rm X, Vega}$$
Therefore, to convert between the magnitude reference systems in other optical frequency bands, we can apply the conversion: 
$$m_{\rm X, AB} - m_{\rm X, Vega} = -2.5\log_{10}\left(\frac{\int (F_{\nu})_{\rm AB} \, T_{X}(\nu) \; \rd\nu}{(F_{\nu})_{\rm Vega} \, T_{X}(\nu) \; \rd\nu}\right)$$

For example, this gives us...
$$
\begin{align}
    U_{\rm AB} &= U_{\rm Vega} - 0.8 \\
    B_{\rm AB} &= B_{\rm Vega} - 0.11 \\
    V_{\rm AB} &= V_{\rm Vega} \\
\end{align}
$$

## Absolute Magnitude

The **absolute magnitude** ($M$) is defined as the [[#apparent magnitude]] ($m$) if the source were measured at a distance of $10\,\pu{pc}$ away from the observer. With removing the issue of observational effects, the absolute magnitude is related to the intrinsic brightness of the source.

$$\underbrace{M - m}_{\text{dist. modulus}} = -2.5 \log_{10} \fpar{F_{10 {\rm pc}}}{F_{\rm D}}$$

With [[Flux#^fdb0f0|flux scaling with the inverse-square law]], we can express the [[#apparent magnitude]] measured at a distance $D$ and vise versa.
$$
\begin{align}
	M - m &= -2.5 \log_{10} \fpar{F_{10 {\rm pc}}}{F_{\rm D}} \\
	&= -2.5 \log_{10} \left( \frac{L}{4 \pi (10 \; {\rm pc})^{2}} \cdot \frac{4 \pi D^{2}}{L} \right) \\
	&= -2.5 \log_{10} \fpar{D}{10 \; {\rm pc}}^{2} \\
	&= -5 \left(\log_{10}D - 1 \right) \hspace{1.5cm} \hRightarrow D = 10^{\frac{m - M + 5}{5}}
\end{align}
$$

## Bolometric Magnitude

The **bolometric magnitude** ($M_{\rm bol}$) is defined as the [[#absolute magnitude]] across all wavelengths/frequencies. 

$$(M_{\rm bol,1} - M_{\rm bol,2}) = - 2.5 \log _{10} \left( \frac{L_{1}}{L_{2}} \right)$$

> [!derivation]-
> Begin with the equations for [[#Absolute Magnitude]] for two different sources.
> $$
> \begin{align}
	> (M_{\rm bol,1} - m_{1}) - (M_{\rm bol,2} - m_{2}) &= -2.5\log _{10} \left( \frac{F_{10,1}}{F_{D,1}} \right) + 2.5\log _{10} \left( \frac{F_{10,2}}{F_{D,2}} \right) \\
	> (M_{\rm bol,1} - M_{\rm bol,2}) + (m_{2} - m_{1}) &= - 2.5 \log _{10} \left( \frac{F_{D,2} \cdot F_{10,1}}{F_{10,2} \cdot F_{D,1}} \right) \\
	> (M_{\rm bol,1} - M_{\rm bol,2}) - \cancelto{0}{(m_{1} - m_{2})} &= - 2.5 \log _{10} \left( \frac{F_{10,1}}{F_{10,2}} \right) + \cancelto{0}{2.5 \log _{10} \left( \frac{F_{D,1} }{F_{D,2}} \right)} \\
	> &\Downarrow \\
	> (M_{\rm bol,1} - M_{\rm bol,2}) &= - 2.5 \log _{10} \left( \frac{F_{10,1}}{F_{10,2}} \right) \hspace{1cm} \textcolor{gray}{L = F \; (4 \pi D_{\rm L}^{2})}\\
	> (M_{\rm bol,1} - M_{\rm bol,2}) &= - 2.5 \log _{10} \left( \frac{L_{1}}{L_{2}} \right)
> \end{align}
> $$

For a star labelled $\star$ , then we can relate the bolometric magnitude of the star relative to bolometric magnitude of the [[Sun]]

$$ M_{bol,\star} - M_{bol,\odot} = -2.5\log _{10}\left(\frac{L_\star}{L_\odot}\right)$$

Overall, the bolometric magnitude tends to be a less practical quantity as we cannot observe the electromagnetic emission of a source with perfect efficiency (i.e. no filter, absorption, extinction etc.).

## Photographic Magnitude

The **photographic magnitude** is defined as measure of the relative brightness of a star or other astronomical object as imaged on a photographic film emulsion with a camera attached to a telescope. 

Photographic observations have now been superseded by electronic photometry such as Charge-Couple Devices ([[Tools#CCD]]) and alternative magnitude systems such as [[Photometry#UBVRI System]].


## Color Index

A **color index** is defined by taking the difference in [[Magnitude|magnitudes]] (a flux ratio) at two different wavelengths or through two different [[Photometry#Bandpass Systems|bandpass]] filters. The most common filters used are the [[Photometry#UBVRI Filters]].

$$
\lambda_{\rm short} - \lambda_{\rm long} \quad \equiv \quad M_{\rm short \lambda} - M_{\rm long \lambda} = -2.5\log_{10} \fpar{F_{\rm short \lambda}}{F_{\rm long \lambda}}
$$

$$$$

> [!recall] 
> Magnitudes **decreases** when brightness **increases**. 
> - If a source object is **brighter** (higher flux) than a reference object (lower flux), then is has a **lower** apparent magnitude.
> - If a source object is **dimmer** (lower flux) than a reference object (higher flux), then is has a **higher** apparent magnitude.

The value of this index tells us how the star is emitting, relative to the different frequency bands.
- If $m_{\rm short \lambda} - m_{\rm long \lambda} < 0$ :
	- The shorter-wavelength filter is transmitting more light than the longer-wavelength filter, and we will see more of the shorter-wavelength radiation.
	- This correlates to seeing **hotter** and **bluer** stars.
- If $m_{\rm short \lambda} - m_{\rm long \lambda} = 0$ :
	- The filters transmit light equally.
- If $m_{\rm short \lambda} - m_{\rm long \lambda} > 0$ :
	- The longer-wavelength filter is transmitting more light than the shorter-wavelength filter, and we will see more of the longer-wavelength radiation.
	- This correlates to seeing **cooler** and **whiter** stars.

For the HR diagram, as a replacement of temperature, the B-V color index is classically used. The V-K tends to have a better spread in $\lambda$, but the V-band is ill-defined. The G-K is better because G works will in space.

$$B-V \quad \equiv \quad m_{\rm B} - m_{\rm V} = -2.5\log_{10} \fpar{F_{\rm B}}{F_{\rm V}}$$

> [!example]-
> - If a star has the magnitudes of $B = m_{\rm B} = 6.7$ and $V = m_{\rm V} = 8.2$, then $B - V = > -1.5$.
> 	- This means the light is passing through the $B$ filter more than the $V$ filter.
> 	- The star emits more blue light than green, and will appear more *blue*.
> - If a star has the magnitudes of $B = m_{\rm B} = 6.7$ and $V = m_{\rm V} = 5.8$, then $B - V = 0.9$.
> 	- This means the light is passing through the $B$ filter lass than the $V$ filter.
> 	- The star emits more green light then blue, and will appear more *white*.



