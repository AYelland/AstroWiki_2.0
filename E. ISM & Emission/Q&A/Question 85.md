### Question
---
What is "brightness temperature"? What is a “Jansky”? How are these different?

### Answer
---
##### What is "brightness temperature"?

***Brightness Temperature*** is the temperature at which a [[Blackbody Radiation|blackbody]] (in thermal equilibrium with its surroundings) would be able to reproduce the observed [[Intensity#Specific Intensity|specific intensity]] of a source.

Rearranging the [[Blackbody Radiation|blackbody]] spectrum for temperature in terms of wavelength $(T_{\lambda})$ and frequency $(T_{\nu})$, we find the relationship the "brightness temperature" the [[Blackbody Radiation#Blackbody Specific Intensity|blackbody specific intensity]]...

$$
I_{\nu} = B_{\nu}=  \frac{2 h \nu^{3}}{c^{2}} \fpar{1}{\exp \left[ \frac{h \nu}{k_{\rm B} T} \right] - 1}
\hRightarrow 
T_{\nu} = \frac{h \nu}{k_{\rm B} \ln \left( 1 + \frac{2 h \nu^{3}}{c^{2} I_{\nu}} \right)}
$$
$$
I_{\lambda} = B_{\lambda}=  \frac{2 h c^{2}}{\lambda^{5}} \fpar{1}{\exp \left[ \frac{h c}{\lambda k_{\rm B} T} \right] - 1}
\hRightarrow 
T_{\lambda} = \frac{h c}{\lambda \, k_{\rm B} \ln \left( 1 + \frac{2 h c^{2}}{\lambda^{5} I_{\lambda}} \right)}
$$

**Important Notes:**
- Commonly used in radio astronomy, where the low-frequency / "Rayleigh-Jeans" limit $(h \nu \ll k_{\rm B} T)$ is applicable such that the blackbody spectrum reduces$$I_{\nu} \simeq \frac{2 \nu^{2} k_{\rm B} T_{\nu}}{c^{2}} \hRightarrow T_{\nu} \simeq \frac{I_{\nu} \, c^{2}}{2 k_{\rm B} \nu^{2}}$$ $$I_{\lambda} \simeq \frac{2 k_{\rm B} \, c \, T_{\lambda}}{\lambda^{4}} \hRightarrow T_{\lambda} \simeq \frac{I_{\lambda} \, \lambda^{4}}{2 k_{\rm B} \, c}$$
- This is a measure of *[[Intensity#Specific Intensity|specific intensity]]*. So, though actually measured in Kelvins ($\rm{K}$), it is quoted in specific intensity units (${\rm W} \cdot {\rm m^{-2}} \cdot {\rm Hz^{-1}} \cdot {\rm sr^{-1}}$)

> [!note]
> I am labelling the blackbody spectrum (intensity) with $I_{\nu/\lambda}$ instead of $B_{\nu/\lambda}$ to emphasize that the source is not a perfect blackbody. 

##### What is a “Jansky”? How are these different?

A **Jansky** (${\rm Jy}$) is a unit of [[Flux#Specific Flux|specific flux]], **not** a measurement of [[Intensity#Specific Intensity|specific intensity]] (or *brightness temperature*). 

$$
\begin{align}
	1 \; {\rm Jy} &= 10^{-23} \; {\rm erg} \cdot {\rm s^{-1}} \cdot {\rm cm^{-2}} \cdot {\rm Hz^{-1}} \\
	1 \; {\rm Jy} &= 10^{-26} \; {\rm W} \cdot {\rm m^{-2}} \cdot {\rm Hz^{-1}}
\end{align}
$$

If you measure a [[Flux#Specific Flux|specific flux]] $(F_{\nu})$ expressed in Janskys with a detector that has a field of view of $\Omega$ steradians, then we can convert to a *brightness temperature* by...

$$
F_{\nu} = \int_{\Omega} I_{\nu} \cos \theta \; \rd \Omega' \approx I_{\nu} \, \Omega\hRightarrow I_{\nu} \propto \frac{F_{\nu}}{\Omega}
$$

Using the low-frequency / "Rayleigh-Jeans" limit $(h \nu \ll k_{\rm B} T)$ as in radio astronomy...
$$
F_{\nu} \approx I_{\nu} \, \Omega \hRightarrow F_{\nu} = \frac{2 \nu^{2} k_{\rm B} \, \Omega \,  T_{\nu}}{c^{2}} \hRightarrow T_{\nu} \simeq \frac{I_{\nu} \, c^{2}}{2 k_{\rm B} \, \Omega \, \nu^{2}}
$$
> [!note] 
> For a Radio Telescope, the solid angle is $\Omega \equiv$"beam", such that ${\rm Jy/beam}$ are the units of a *brightness temperature*.
