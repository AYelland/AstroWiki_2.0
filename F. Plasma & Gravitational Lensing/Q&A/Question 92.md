### Question
---
What is “dispersion measure” for electromagnetic waves in a plasma? How is it used in astronomy?

### Answer
---
##### What is “dispersion measure” for electromagnetic waves in a plasma?

The **dispersion measure (DM)** quantifies the dispersion of light along the path of propagation. It is defined as the integrated free electron density (i.e. column density) between the source and the observer.

$$
{\rm DM} = \int_{0}^{d} n_{\rm e}(z) \; \rd z
\hWhere
\begin{aligned}
	z &\equiv \text{path of propagation} \\
	n_{\rm e}(z) &\equiv {\rm e^{-}\ number\ density\ at\ } z \\
\end{aligned}
$$

**Basic Overview:**
- The refractive index varies along the light's path of propagation depending on the medium the light passes through. In particular, we are concerned with ionized material and its affect on the propagation.
- The refractive index is a frequency-dependent quantity. $$n = \frac{c}{v} = \frac{c}{\nu \lambda} = \frac{2 \pi c}{\omega \lambda} \hWhere n \equiv \text{refractive index}$$
- If we shine a spectrum of many frequencies through an ionized region, the light which experiences a lower refractive index will exit first ($v = c/n$).
- This leads to a ***frequency-dependent time delay*** of the observed light, and the further the light travels through an ionized medium, or the denser the medium, the greater the effect.
- The **dispersion measure** quantifies this dispersion of light by integrating the free electron density along the direction of propagation, and thus is effectively a column density.

> [!derivation] The Time Delay
> 
> The frequency-dependent time delay can be derived from the group velocity ($v_{\rm g}$) and dispersion relationship for plasma. *([stackexchange](https://astronomy.stackexchange.com/questions/37100/how-to-determine-arrival-time-delay-given-dispersion-measure))*
> 
> $$
> \textcolor{gray}{ \left[ \; 
> \text{Dispersion Relation:} \hspace{1cm} \omega^{2} = \omega_{\rm p}^{2} + c^{2} k^{2}
> \hWhere
> \begin{aligned}
> 	\omega &\equiv \text{wave ang. frequency} \\
> 	\omega_{\rm p} &\equiv \text{plasma ang. frequency} \\
> 	k &\equiv \text{wave number}
> \end{aligned}
> \; \right]}
> $$
> $$v_{\rm g} = \td{\omega}{k} = \frac{2 c^{2} k}{2 \sqrt{\omega_{\rm p}^{2} + c^{2} k^{2}}} = \frac{c^{2} k}{\omega} = c \; \sqrt{1 - \fpar{\omega_{\rm p}}{\omega}^{2}}$$
> 
> $$
> \begin{aligned}[b]
> 	t(\omega) &= \left[ \int_{0}^{d} \frac{\rd z}{v_{\rm g}} \right] - \frac{d}{c} \\
> 	&= \left[ \int_{0}^{d} \frac{\rd z}{c \sqrt{1 - (\omega_{\rm p}/\omega)^{2}}} \right] - \frac{d}{c} \\
> 	\\
> 	&\hspace{0.5cm} \textcolor{gray}{\Downarrow \quad(\omega \, \gg \, \omega_{\rm p})} \\
> 	\\
> 	&\approx \left[ \int_{0}^{d} \frac{1}{c} \, \left( 1 + \frac{1}{2} \fpar{\omega_{\rm p}}{\omega}^{2} \right) \; \rd z \right] - \frac{d}{c} \\
> 	&\approx \left[ \frac{d}{c} + \int_{0}^{d} \frac{1}{2 c}\fpar{\omega_{\rm p}}{\omega}^{2} \; \rd z \right] - \frac{d}{c} \\
> 	&\approx \frac{1}{2 c} \frac{1}{\omega^{2}} \int_{0}^{d} \omega_{\rm p}^{2} \; \rd z \hspace{4cm} \textcolor{gray}{\left[ \omega_{\rm p} \equiv \sqrt{\frac{e^{2} n_{\rm e}}{\epsilon_{0} \,m_{\rm e}}} \right]} \\
> 	&\approx \fpar{e^{2}}{2 \epsilon_{0} \, m_{\rm e} c} \; \frac{1}{\omega^{2}} \left( \int_{0}^{d} n_{\rm e} \; \rd z \right) \hspace{1.5cm} \textcolor{gray}{\left[ \nu \equiv \frac{\omega}{2 \pi} \right]}\\
> 	&\approx \underbrace{\fpar{e^{2}}{8 \pi^{2} \epsilon_{0} \, m_{\rm e} c}}_{k_{\rm DM}} \; \frac{1}{\nu^{2}}\; \underbrace{\left( \int_{0}^{d} n_{\rm e} \; \rd z \right)}_{\rm DM}
> \end{aligned}
> $$
> 
> $$t(\nu) = {\rm DM} \frac{k_{\rm DM}}{\nu^{2}} \hRightarrow \Delta t = {\rm DM} \, k_{\rm DM} \left( \frac{1}{\nu_{2}^{2}} - \frac{1}{\nu_{1}^{2}} \right)$$
> 
> where we have defined the dispersion constant ($k_{\rm DM}$). 
> 
> $$k_{\rm DM} = \frac{e^{2}}{8 \pi^{2} \epsilon_{0} \, m_{\rm e} c} \simeq 4.15 \,\pu{GHz^{2} pc^{-1} cm^{3} ms}$$
> 
> We see from this relationship that higher wave frequencies ($\nu$) yield higher group velocities ($v_{\rm g}$) and shorter time delays, such that higher energy light travels faster and vise versa. (Only noticeable when the [[Question 93|plasma frequency]] is close to the wave frequency.)
> $$\Delta t \propto \nu^{-2} \cdot {\rm DM}$$

##### How is it used in astronomy?

Because we usually don't know when the light from a source was emitted, we can't measure a single time delay. Instead, we use the differences in arrival times ($\Delta t$) between two frequencies, and use that to determine the electron column density ($n_{\rm e}$).

This quantity has been used to demonstrate that [[Fast Radio Burst|FRBs]] must be extragalactic, because they have high ${\rm DM}$ values in comparison to galactic pulsars.

$${\rm DM} = {\rm DM_{MW}} + {\rm DM_{nost}} + \underbrace{\rm DM_{IGM}}_{\substack{\text{increases w/} \\ \text{distance}}}$$

![[DM_FRB.jpg|align:center|500]]

Shape of galactic "cone" in the image above represents objects outside of the disk. The farther the source is from latitude 0 (the disk itself), the less material obstructing the view such that the dispersion measure gets smaller. This cone behavior showcases a stark difference relative to [[Fast Radio Burst|FRB]] dispersion measures; hence, they must be extragalactic.

> [!note] 
> By knowing the distance to a galactic pulsar (blue) we can get an estimate of the column density, or vice versa.