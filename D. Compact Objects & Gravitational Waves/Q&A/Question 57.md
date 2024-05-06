### Question
---
What minimum mass is required for a black hole powering a quasar of luminosity $10^{12} \; {\rm L_{\odot}}$? What accretion rate is required?

### Answer
---
##### What minimum mass is required for a black hole powering a quasar of luminosity $10^{12} \; {\rm L_{\odot}}$?

A [[Active Galactic Nuclei#Quasar|quasar]] is a very luminous [[Active Galactic Nuclei|AGN]]. This means that the [[Black Hole|black hole]] is surrounded by some accretion disk that is feeding the EM radiation (causing the high luminosity). 

The mass of the [[Black Hole|black hole]] (including its accretion disk) will be constrained by the [[Luminosity#Eddington Limit]]. Given that a black hole doesn't emit light itself, we can solely focus on the luminous accretion disk in our calculations.

$$L_{\rm Edd} = \frac{4 \pi G M c}{\kappa} \approx 3.2 \times 10^{4} \; \fpar{M}{M_{\odot}} \underbrace{\fpar{\kappa_{\odot}}{\kappa}}_{=1} \; L_{\odot} \hRightarrow M = \left[ \frac{1}{3.2 \times 10^{4}} \fpar{L_{\rm eff}}{L_{\odot}} \right] \; M_{\odot}$$
$$M_{\rm Edd} \equiv M = \left[ \frac{1}{3.2 \times 10^{4}} \fpar{10^{12} \, L_{\odot}}{L_{\odot}} \right] \; M_{\odot} \sim 3 \times 10^{7} \; {\rm M_{\odot}}$$

If the mass of was smaller than the Eddington Mass (minimum mass), then the radiation pressure would be stronger than the gravitational pressure, causing the system to be unstable. 
##### What accretion rate is required?

From [[Question 47]], we will take that the accretion efficiency as $\eta = 0.1$ (roughly the cosmic average). The accretion rate is the time derivative of the mass.

$$\dot{M} = \td{M}{t} = \frac{L}{\eta c^{2}} \sim 0.7 \; {\rm M_{\odot} / yr}$$
$$\textcolor{gray}{\left[\frac{L}{\eta c^{2}} \simeq \frac{10^{12} \; (4 \times 10^{26})}{(0.1) \cdot (3 \times 10^{8})^{2}}  \simeq (0.\bar{4} \times 10^{-7} \; {\rm kg/s}) \times \fpar{\pi \times 10^{7} \; {\rm s/yr}}{2 \times 10^{30} \; {\rm kg / M_{\odot}}} \sim 0.7 \; {\rm M_{\odot} / yr} \right]}$$

> [!note] On the Accretion Efficiency (copied from [[Question 47]])
> Accretion liberates gravitational potential energy as gas loses angular momentum and falls onto the compact object.
> $$L = \eta \dot{M} c^{2} \hWhere \left( \frac{\text{energy radiated}}{\text{time}} = \frac{\text{efficiency} \times \text{mass-energy gained}}{\text{time}} \right)$$ 
> The accretion efficiency $\eta$ is spin-dependent.
> - $\sim 6 \%$ for [[Black Hole#Schwarzschild Black Hole]]
> - $\sim 40 \%$ for a maximally spinning [[Black Hole#Kerr Black Hole]]
> - Estimating as $10 \% = 0.1$ is fine.
