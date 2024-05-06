---
banner: "![[instrumentation.png]]"
banner_y: 0.79
aliases:
---
## Bandpass Systems

Each letter in the following systems designate a section of light of the electromagnetic spectrum.

![[bandpassFilters.png|align:center]]

### UBVRI Filters
*(Also known as **Johnson/Bessel system** or **Johnson-Morgan system**)

![[UBVRI.jpg|aling:center|500]]

The UBVRI system utilizes a set of defined photometric filters for source classification in the following frequency bands.

| Abbrev. | Bandpass             |    Wavelength Range     | Effective Wavelength Midpoint |
|:-------:| -------------------- |:-----------------------:|:-----------------------------:|
|    U    | Ultraviolet          | $320 - 400 \; {\rm nm}$ |       $365 \; {\rm nm}$       |
|    B    | Blue                 | $400 - 500 \; {\rm nm}$ |       $445 \; {\rm nm}$       |
|    V    | Vert(Green) / Visual | $500 - 700 \; {\rm nm}$ |       $551 \; {\rm nm}$       |
|    R    | Red                  | $550 - 800 \; {\rm nm}$ |       $658 \; {\rm nm}$       |
|    I    | Infrared             | $700 - 900 \; {\rm nm}$ |       $806 \; {\rm nm}$       |

Each filter has an associated transmission function, $T_{X}(\nu)$, that determines what percent of the [[Flux]] is let through at a given frequency or wavelength.

### Sloan Digital Sky Survey (SDSS) Filters

![[SDSS_filters.jpg|align:center|500]]

Similar to the [[#UBVRI System]], but more modernized and standardized. 


## Spectral Energy Distrbutions

Radio - tends to use frequency
Optical - tends to use wavelength
X-ray / Gamma-Ray - measure in
- photon number density ($F = dN/dE$) in units of $\left[ \pu{photons cm^{-2} s^{-1} keV^{-1}} \right]$
- energy flux ($F_{E} = E \td{N}{E}$) in units off $\left[ \pu{ erg cm^{-2} s^{-1} keV^{-1}} \right]$

Astronomers tend to plot $\log(\nu)$- $\log(\nu F_{\nu})$  (called a spectral energy distribution in x-ray astronomy, other fields use this term more loosely)
- the area under the curve is directly assocaited to the energy within the system
- For wavelength:  $\log(\lambda)$ - $\log(\lambda F_{\lambda})$ 
- For energy:  $\log(E)$ - $\log(E^{2} \td{N}{E})$

With astronomical photometry, we work with integrated flux over some bandpass
$$
F_{\rm bandpass}^{\rm obs} = \int_{\nu_{1}}^{\nu_{2}} F_{\nu}(\nu) R(\nu) \; \rd \nu 
\hWhere 
\begin{aligned}
	F_{\nu}(\nu) &\equiv \text{source spectrum} \\
	R(\nu) &\equiv \text{instrument response} = \prod {\rm efficencies}
\end{aligned}
$$
