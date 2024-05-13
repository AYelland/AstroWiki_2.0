### Question
---
Qualitatively, how does a density fluctuation grow over cosmic history and how does the answer differ for dark matter and baryons?

### Answer
---
There are two major factors to consider when discussing the cosmic density fluctuations:

- The [[Jeans Formalism#Jeans Length]] in each epoch
	- The Jeans Length ($\lambda_{J}$) is the length scale above which a body will gravitationally collapse.
- The "Sound Horizon" at different times. 
	- The sound horizon ($\chi_{\rm s}$) is the length scale that sound (pressure/density waves) can travel at a particular time, and thus the length scale over which overdensities can be washed out at any given time. 

Conceptually, we consider some perturbation (density fluctuation) moving through the universe. When the spatial size of that perturbation is larger than the sound horizon, it will grow as the universe grows, since it cannot be stabilized/washed out at such early times. Additionally, if it is smaller than the [[Jeans Formalism#Jeans Length]], it will also not collapse. 

That said, once the sound horizon grows big enough, it will be able to stabilize the perturbation. 

> [!note] 
> The below is closely related to calculation is similar to sound horizon size at [[Cosmological Timeline#Recombination|recombination]]. (see [[Cosmic Microwave Background#Sound Horizon|CMB sound wave]])

##### Jeans Length

Given the [[Jeans Formalism|Jeans stability criteria]] depends on the [[Fluid Mechanics#Speed of Sound|speed of sound]], we can use the general definition to analyze how it changes in the early universe.

$$c_{\rm s} = \sqrt{\frac{\partial P}{\partial \rho}}$$

- **Radiation-Dominated:**
	Before [[Cosmological Timeline#Recombination]], the fluid is dominated by [[Stellar Structure#Radiative Energy Transport|radiation pressure]].
	
	$$P_{rad} = \frac{1}{3} \rho c^{2} \hspace{1cm} \Rightarrow \hspace{1cm} c_{\rm s} = \sqrt{\frac{\partial P}{\partial \rho}} = \frac{c}{\sqrt{3}}$$

- **Matter-Dominated:**
	After [[Cosmological Timeline#Recombination]], the baryons are effectively an [[Thermodynamics#Ideal Gas Law|ideal gas]], where we use $T  = T_{0} (1+z_{\rm rec}) \simeq 2.7 (1100) \; {\rm K} \simeq 3000 \; \pu{K}$ and $\mu$ is the [[Mean molecular weight#Mean molecular weight|mean molecular weight]]. 
	
	$$P = \frac{\rho}{\mu m_{\rm p}} k_{\rm B} T \hspace{1cm} \Rightarrow \hspace{1cm} c_{\rm s} = \sqrt{\frac{\partial P}{\partial \rho}} = \sqrt{\frac{k_{\rm B} T}{\mu m_{\rm p}}} \ll c$$
	
This means $c_{\rm s}$ drops dramatically at recombination, and thus, so does the [[Jeans Formalism#Jeans Length]] and [[Jeans Formalism#Jeans Mass]].

$$M_{J} \sim 10^{16} \;{\rm M_{\odot}} \hspace{1cm} \xrightarrow{\text{at recombination}} \hspace{1cm} M_{J} \sim 10^{5} \; {\rm M_{\odot}}$$

This implies most of the structure we see today formed after recombination. As a result, lets only consider overdensity growth due to expansion and ignore the Jeans criteria for now.

##### Sound Horizon

 Similarly, we can analyze how sound horizon evolves in different epochs by which term dominates the evolution in the [[Friedmann Equation]] at early times, high $z$ and low $a$. *(See [[Question 137]] for the time-dependence of $a(t)$ in each era, or the [[Mnemonics#Cosmology Epoch Scaling-Dependence|Mnemonics]])*

- **Radiation-Dominated:** $$H(t) = H_{0} \sqrt{\Omega_{r} (1+z)^{4}} \hspace{3cm} a(t) \propto t^{1/2}$$
	The [[Distances#Comoving Distance|comoving length]] ($\chi_{\rm s}$) and [[Distances#Proper Distance|proper length]] ($L_{\rm s}$) of the sound horizon is...
	
	$$\chi_{\rm s} \simeq \int_{0}^{t} \frac{c_{\rm s} \; \mathrm{d} t'}{a(t')} \propto 2 c_{\rm s} \, t^{1/2} \hspace{1cm} \Rightarrow \hspace{1cm} L_{\rm s} = a \, \chi_{\rm s} \propto 2 c_{\rm s} \, t$$
	
	If we plug in the expression for $t$ from the [[Friedmann Equation]], we would find is smaller than the [[Jeans Formalism#Jeans Length]] ($\lambda_{J}$), and thus, there would be no collapsing.
	
	$$H = \frac{\dot{a}}{a} = \frac{1}{2 t} = \sqrt{\frac{8 \pi G \rho_{r}}{3}} \hspace{1cm} \Rightarrow \hspace{1cm} t = \frac{1}{2} \sqrt{\frac{3}{8 \pi G \rho_{r}}} \hspace{1cm} \Rightarrow \hspace{1cm} L_{\rm s} = \underbrace{\sqrt{\frac{\pi c_{\rm s}^{2}}{G \rho_{r}}}}_{\lambda_{J}} \; \cdot \; \sqrt{\frac{3}{8 \pi^{2}}}$$

- **Matter-Dominated:** $$H(t) = H_{0} \sqrt{\Omega_{M} (1+z)^{3}} \hspace{3cm} a(t) \propto t^{2/3}$$
	Using the same equations as above with a different $a(t)$ expression, we find...
	
	$$\chi_{\rm s} \simeq \int_{0}^{t} \frac{c_{\rm s} \; \mathrm{d} t'}{a(t')} \propto 3 c_{\rm s} \, t^{1/3} \hspace{1cm} \Rightarrow \hspace{1cm} L_{s} = a\, \chi_{s} \propto 3 c_{\rm s} \, t$$
	...where similarly, if we plug in the expression for $t$ from the [[Friedmann Equation]], we would find is smaller than the [[Jeans Formalism#Jeans Length]] ($\lambda_{J}$), and thus, there would be no collapsing.
	
	$$H = \frac{\dot{a}}{a} = \frac{2}{3 t} = \sqrt{\frac{8 \pi G \rho_{M}}{3}} \hspace{1cm} \Rightarrow \hspace{1cm} t = \frac{2}{3} \sqrt{\frac{3}{8 \pi G \rho_{M}}} \hspace{1cm} \Rightarrow \hspace{1cm} L_{\rm s} = \underbrace{\sqrt{\frac{\pi c_{\rm s}^{2}}{G \rho_{M}}}}_{\lambda_{J}} \; \cdot \; \sqrt{\frac{3}{2 \pi^{2}}}$$
##### Bringing it All Together...

Given that for some perturbation with length scale $L$, we have found that the system will remain stabilized if...

$$L < L_{\rm s} < \lambda_{J}$$

Therefore, if the length scale of the perturbation exceeds the length scale of the sound horizon ($L_{\rm s}$), then we will see the beginning of gravitational collapse for the unstable system. This does **not** happen during the time in which the universe is radiation-dominate or matter-dominate.

So, if we choose a particular length scale for a perturbation $L$. 
- When the sound horizon is equal to length scale ($L_{\rm s} = L$), we say the perturbations "enter the horizon".
- Prior to entering the horizon, all perturbations on the scale $L$ grow as with time-dependence calculated in [[Question 137]] and the perturbation is washed out.
- Once this length scale has "entered the horizon", then the sound waves exceed the horizon and destabilize the system causing gravitational collapse. 
- Upon collapse, the [[Baryon Acoustic Oscillations]] will begin as the photon pressure pushes the baryons back out, reducing their overdensity in the potential well.
- When recombination is reached, the [[Baryon Acoustic Oscillations|BAO]] cease and are frozen into the [[Cosmic Microwave Background|CMB]]

> [!note] 
> We note that the [[Dark Matter|dark matter]] and photons are not meaningfully coupled, such that the DM clouds will continue to collapse as the baryons oscillate.

The picture is as below (Megans notes), where the oscillating portion is illustrated with animations in [[Cosmic Microwave Background#CMB Power Spectrum]]. The exact position of "entering the sound horizon" can only be calculated by assuming a particular overdensity spatial scale $L$, with smaller sizes "entering the horizon" earlier and thus spending more time oscillating.

![[overdensity_growth.png|align:center]]

> [!note]
> The scaling of densities (and thus overdensities) in time in each of these epochs is given in [[Question 137]], where one finds that for radiation dominated epochs $\delta \propto a^2$ and for matter-dominated $\delta \propto a$.