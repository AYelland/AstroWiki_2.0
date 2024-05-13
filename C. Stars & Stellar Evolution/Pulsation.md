---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
  - pulsating
---
## Why do stars pulsate?

The pulsations in a star originate from variations in the radiation flow that allows energy to escape from the star. Let us look at the steps involved in a pulsating stars:

1. If the pressure outwards exceeds the gravitational force inwards, the outer layers of a star will expand outwards.
2. As the star expands, its gravitational force inwards diminishes but its outwards pressure also drops at an even greater rate.
3. Eventually the star would reach a position at which hydrostatic equilibrium occurs; however, the outward moving layers still have momentum and are resistant to a change in motion. This momentum carries the layer past the equilibrium position.
4. As the gravitational force slows down the expansion to a stop, but the outward gas and radiation pressure is now weaker than the inward-acting gravitational force.
5. The imbalance of forces now causes the star's outer layers to collapse inwards.
6. As the layers collapse gravity increases but the pressure increases at a greater rate.
7. With the pressure outwards exceeding the inwards gravitational force the collapsing layer slows down and eventually stops.
8. We are now back at the start where the outwards pressure is greater than the gravitational force so the pulsation cycle starts again!

A pulsating star is thus not in equilibrium, but is always trying to regain it. It is an harmonic oscillator.

## Pulsation Period

Pulsations in a star are effectively the equivalent of sound waves resonating through the medium. Through this comparison, we can estimate pulsation period from the [[Fluid Mechanics#Speed of Sound|sound crossing time]] by assuming the star can be represented through a [[Polytropes|polytropic]] equation of state.

$$P = \kappa \rho^{\gamma} \hspace{1cm} \Rightarrow \hspace{1cm} c_{s} = \sqrt{\frac{\partial P}{\partial \rho}} = \sqrt{\kappa \gamma \rho^{\gamma -1}} = \sqrt{\frac{\gamma P}{\rho}}$$

If we assume our star has a constant density ($\rho$) in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]] for a rough approximation, then we integrate to find an expression for pressure.

$$
\frac{\mathrm{d} P}{\mathrm{d} r} = -\frac{G M_{r} \rho}{r^{2}} \simeq - \frac{4 \pi G \rho^{2} r}{3} \hspace{1cm} \Rightarrow \hspace{1cm}
\begin{aligned}[t]
	\int_{P(r)}^{P(R)=0} \mathrm{d} P' &= - \frac{4 \pi G \rho^{2}}{3} \int_{r}^{R} r \; \mathrm{d} r \\
	P(r) &= \frac{2 \pi G \rho^{2}}{3} \left( R^{2} - r^{2} \right) \\
\end{aligned}
$$

Applying this to the [[Fluid Mechanics#Speed of Sound|speed of sound]]...  

$$
c_{s}(r) = \frac{\mathrm{d} r}{\mathrm{d} t} \simeq \sqrt{\frac{2 \pi G \gamma \rho^{2}}{3} \left( R^{2} - r^{2} \right)} \hspace{1cm} \Rightarrow \hspace{1cm}
\begin{aligned}[t]
	T = \int_{0}^{T} \mathrm{d} t = \int_{0}^{R} \frac{1}{c_{\rm s}} \; \mathrm{d} r \approx \sqrt{\frac{3 \pi}{2 G \gamma \rho}}
\end{aligned}
$$

...we find that the period is inversely proportional to  density. 

$$T \simeq 2\int_0^R dr\,\frac{1}{v_s} \simeq \sqrt{\frac{3\pi}{2\gamma G \rho}} \propto \frac{1}{\sqrt{\rho}}$$

Therefore, a higher density star pulsates faster. 

## Kappa Opacity Mechanism

The **Kappa Opacity Mechanism** is the driving mechanism behind the changes in luminosity of many types of pulsating variable stars, including [[Stellar Classes#Cepheids]] and [[Stellar Classes#RR Lyrae]] stars. 

Effectively, the pulsation is caused by variations of opacity ($\kappa$) that limit the radiation efficiency inside the star.
 
In a "normal", non-pulsating star...
- An increase in compression of the atmosphere causes an increase in temperature and density
- This decreases opacity of the atmosphere, allowing energy to escape more rapidly
- The result is an equilibrium condition where temperature and pressure are maintained in a balance. 

In a pulsating star...
- An increase in compression of the atmosphere causes an increase in temperature and density
- If the temperature is near the ionization transitions of $\ce{H}$ and $\ce{He}$, opacity increases from the [[Thomson Scattering|electron scattering]], preventing energy and heat from escaping.
- In return, this causes a build-up of pressure that pushes the layer back out beyond the equilibrium point. 
- Gravity draws the layer back in, causing a compression of the atmosphere....
The result is a cyclic process as the layer repeatedly moves inward and then is forced back out again.