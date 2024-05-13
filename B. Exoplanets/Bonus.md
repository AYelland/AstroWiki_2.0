---
banner: "![[exoplanets.png]]"
banner_y: 0.6
aliases:
---
## Calculations from Transit Observations
### Bonus - Measuring the Stellar Density
*(D. Berardo)*

We can directly determine the density of the star if we assume the planet's orbit is circular and much smaller than the star (${\rm M_{\rm p} \ll M_{*}}$). If we measure the duration ($T$) and period ($P$) of a transit, then by [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]]...

$$
\begin{align}
	P^{2} = \frac{4 \pi^{2} a^{3}}{G M_{\rm tot}} &\approx \frac{4 \pi^{2} a^{3}}{G M_{*}} \hspace{2cm} \textcolor{gray}{\left[ M_{\rm tot} = (M_{\rm p} + M_{*}) \approx M_{*} \right]}\\
	&= \frac{4 \pi^{2}}{G} \frac{\left[ a^{3} / \left( \frac{4}{3} \pi R_{*}^{3} \right) \right]}{\left[ M_{*} / \left( \frac{4}{3} \pi R_{*}^{3} \right) \right]} \\
	&= \frac{4 \pi^{2}}{G} \left(\frac{3}{4 \pi}\right) \left(\frac{a^{3}}{R_{*}^{3}}\right) \left(\frac{1}{\rho_{*}}\right) \\

	&= \frac{3 \pi}{G} \left(\frac{a}{R_{*}}\right)^{3} \left(\frac{1}{\rho_{*}}\right)
\end{align}
$$

Furthermore, $T/P$ is the ratio of the arc length for the time the planet is passing in front of the star to that of the whole orbit (for circular orbits).

![[transit_arc.png|align:center|400]]

$$\frac{T}{P} \simeq \frac{(2 R_{*})}{\pi (2 a)} \implies \frac{a}{R_*} \simeq \frac{P}{\pi T}$$

...where the $2 R_*$ comes from approximating the transiting arc as a straight line relative to the large distance $a$ (for a relatively small stellar radius, $R_{*}$). Combining and rearranging the above expressions, we can derive a relationship for stellar density with respect to period and duration of the transit (independent of transit depth).

$$\rho_{*}(T, P) = \frac{3 \pi}{G} \left(\frac{P}{\pi T}\right)^{3} \frac{1}{P^{2}} = \frac{3}{G \pi^{2}} \left(\frac{P}{T^{3}}\right)$$

> [!note]
> The circular orbit assumption is not unreasonable given the [[Detection Methods#Transit Method|transit method]] is biased to small orbital radii -- which tend to lead to smaller eccentricities.


### Bonus - Measuring the Planet's Temperature
*(M.Masterson)*

If you assume the star and planet emit (or reflect) like a [[Blackbody Radiation|blackbody]], then we can measure the brightness of the system measured before the secondary transit (planet + star $=F_{\rm *+p}$) and the during the secondary transit when the planet goes behind star (star $=F_{*}$). Constructing a similar expression as before through the luminosity relationship, we can find the percentage dip in the light curve as before, but with the secondary transit.

$$
\delta_{\rm secondary} = \frac{L_{\rm *+p} - L_{*}}{L_{*}} = \frac{\left( F_{*} R_{*}^{2} + F_{\rm p} R_{\rm p}^{2} \right) - F_{*} R_{*}^{2}}{F_{*} R_{*}^{2}} = \frac{F_{\rm p} R_{\rm p}^{2}}{F_{*} R_{*}^{2}} \approx \underbrace{\frac{B_{\lambda}(T_{\rm p}) R_{\rm p}^{2}}{B_{\lambda}(T_{*}) R_{*}^{2}}}_{\rm blackbody} \approx \underbrace{\frac{T_{\rm p} R_{\rm p}^{2}}{T_{*} R_{*}^{2}}}_{\rm long \ \lambda \ limit}
$$

To actually calculate the planet's temperature ($T_{\rm p}$), we need a follow-up measurement from another instrument to get the surface temperature of the star ($T_{*}$),

> [!math] Long Wavelength Limit for [[Blackbody Radiation#Blackbody Specific Intensity]]
> $$
> B_{\lambda}(\lambda,T) = \frac{2 h c^{2}}{\lambda^{5}} \left(\frac{1}{e^{h c / (\lambda k_{\rm B} T)} - 1}\right)
> \hspace{1cm} \Rightarrow \hspace{1cm}
> B_{\lambda}(\lambda,T) \approx \frac{2 c k_{\rm B} T}{\lambda^{4}} \propto \frac{T}{\lambda^{4}}
> $$

> [!note] Another method, but not valid?
> $$T_{\rm p} = \left(\frac{(F_{*} + F_{\rm p}) - F_{*}}{\sigma}\right)^{1/4} = \left(\frac{F_{\rm p}}{\sigma}\right)^{1/4} \hspace{2cm} T_{*} = \left(\frac{F_{*}}{\sigma}\right)^{1/4}$$
> I am not sure if this is a valid method, given that without normalization and corrections, the light curve is not flat. The orbit of the planet gives additional contributions that create a sinusoidal continuum, and it could be affecting how the flux is measured?

