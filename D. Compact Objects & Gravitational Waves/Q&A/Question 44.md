### Question
---
A double neutron star system in M31 is about to merge. What is the approximate energy emitted in gravitational radiation and what is the corresponding amplitude (strain) h observed here on Earth? Would LIGO be able to detect it?

### Answer
---
##### A double neutron star system in M31 is about to merge. What is the approximate energy emitted in gravitational radiation and what is the corresponding amplitude (strain) h observed here on Earth?

Using the calculation done in [[Question 43]] when calculating the [[Question 43#^freq-dependence|GW frequency time-dependence]], we can express the gravitational wave radiation ($L_{\rm GW}$) as...

$$
\begin{aligned}[t]
	&L_{\rm GW} = \frac{32 G^{7/3}}{5 c^{5}} (M_{\rm c} \, \omega)^{10/3} \\
	\\
	&\textcolor{gray}{L_{\rm GW} \simeq 10^{87} \left( \frac{M_{\rm c}}{M_{\odot}} \, \omega \right)^{10/3} \; {\rm [W]}}
\end{aligned}
\hWhere
\begin{aligned}[t]
	M_{\rm c} &\equiv \text{chirp mass} = \mu^{3/5} M^{2/5} \\
	\mu &\equiv \text{reduced mass} \\
	M &\equiv \text{total mass} \\
	\omega &\equiv \text{orbital frequency} \\
	f &\equiv \text{GW frequency} = \omega/\pi
\end{aligned}
$$

We approximate the two [[Neutron Star|neutron stars]] to have typical masses ($1.4 \; {\rm M_{\odot}}$) and that they coalesce at their ISCO radii. From [[Question 43]], the orbital frequency and gravitational frequency at coalescence is...

$$\omega_{c} = \sqrt{\frac{G M}{a^{3}}} = \frac{c^{3}}{(6)^{3/2} \, G \,(2.8 \; {\rm M_{\odot}})} \simeq 4933 \; {\rm rad \, s^{-1}} \hRightarrow f = \frac{\omega}{\pi} \sim 1570 \; {\rm Hz}$$

...and the [[Gravitational Waves#Chirp Mass|chirp mass]] is...

$$M_{\rm c} = \mu^{3/5} M^{2/5} \quad \xrightarrow{\rm M_{*} = M_{1} = M_{2}} \quad M_{\rm c} = \frac{M_{*}}{2^{1/5}} \simeq 0.9 M_{*} \hRightarrow M_{\rm c} \simeq 1.2 \; {\rm M_{\odot}}$$

Applying these values to GW radiation equation, we can get the total energy output during the coalescence period ($\delta t_{\rm c} \simeq 10 \; {\rm ms}$). We see that this event outputs energy levels similar to a supernova ($E_{\rm SN} \sim 10^{44} \; {\rm J}$).

$$L_{\rm GW} = \frac{E_{\rm GW}}{\delta t_{\rm c}} = \left[ \frac{32 G^{7/3}}{5 c^{5}} (M_{\rm c} \, \omega)^{10/3} \right] \sim 10^{48} \; {\rm W} \sim 10^{21} \; {\rm L_{\odot}} \hRightarrow \boxed{E_{\rm GW} \sim 10^{46} \; {\rm J} }$$

For the scaling amplitude (strain), we can take the distance to M31 as $R \sim 800 \; {\rm kpc}$, such that plugging in the values...

$$h_{0} \simeq \sqrt{\frac{G L_{\rm GW}}{2 R^{2} \omega^{2} c^{3}}} \quad \simeq \fpar{4}{\sqrt{5} c^{4}} \frac{(G M_{\rm c})^{5/3}\omega^{2/3}}{R} \hRightarrow \boxed{h_{0} \sim 10^{-20}}$$

##### Would LIGO be able to detect it?

![[GW_sensitivity_curves.png|600]]

With strain $h_{0} \sim 10^{-20}$ (y-axis) and gravitational wave frequency of $f \sim 2 \; {\rm kHz}$ (x-axis), this is well within the [[Instruments#LIGO]] sensitivity.

> [!note] Contributions to Noise
> 
> On the lower end, the primary noise comes from seismic activity of the earth and the tectonic plates. On the upper end, the primary noise comes from "shot" noise, the effects the photons have on the mirrors of the interferometer.
> 
> ![[GW_LIGOnoise.png|align:center|500]]

