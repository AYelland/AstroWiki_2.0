### Question
---
What is "biased galaxy formation"?

### Answer
---
The.**biased galaxy formation** refers to the fact that galaxies are not perfect tracers of mass in the universe. (i.e. the fluctuations in the galaxy distribution across the universe does not match the fluctuations in mass.)

*Why are galaxies a biased mass tracer?*
- Baryonic physics acts differently than the mass-dominant [[Dark Matter|dark matter]].
- We lack of good understanding of galaxy formation.

The "bias factor" ($b$) is defined as a metric between the galaxy mass distribution (overdensities) and that of all matter, or very similarly, between the [[Question 122|two-point correlation functions]] of galaxies and all matter.

$$b = \frac{\delta_{\rm gal}}{\delta_{\rm m}} \hspace{1cm} \text{or} \hspace{1cm} b^{2} = \frac{\xi_{\rm gal}}{\xi_{\rm m}} \hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}
	\delta_{\rm gal} &\equiv \text{overdensity of galaxies' mass} \\
	\delta_{\rm m} &\equiv \text{overdensity of underlying mass}
\end{aligned}$$

> [!note] If $b=1$, galaxies are perfect tracers of the matter distribution of the universe.

In the context of a linear bias model, the bias factor can be correlated to the amplitude of the linear primordial power spectrum ($\sigma_{8}$). Observationally, we measure the number of fluctuations in galaxy surveys within a sphere of $\sim 8 \, h^{-1} \; {\rm Mpc}$ (scale chosen by convention).

$$\sigma_{\rm 8,gal} = b \,\sigma_{\rm 8,m} \hspace{2cm} {\rm or} \hspace{2cm} \frac{\delta n_{\rm gal}}{\bar{n}_{\rm gal}} = b \left( \frac{\delta \rho}{\bar{\rho}} \right)$$

where
- $\sigma_{\rm 8} \equiv$ normalization of the power spectrum, related to, but not equal to $A$ in the power spectrum definition below ($\sigma_{\rm 8,m}$ constrained by [[Cosmic Microwave Background|CMB]] measurements and $\sigma_{\rm 8,gal}$ constrained by large galaxy surveys)
- $\delta n_{\rm gal} \equiv$ fluctuations in galaxy number density
- $\bar{n}_{\rm gal} \equiv$ mean galaxy number density
- $\delta \rho \equiv$ fluctuations in mass density
- $\bar{\rho} \equiv$ mean mass density

> [!note] Primordial Power Spectrum
> 
> The primordial power spectrum describes the initial perturbations in the universe leading to the structure-formation we observe today.
> 
> ![[DMpowerspectrum.jpeg|align:center|450]]
> 
> $$P(k) = A k^{n} \hspace{1cm} \Rightarrow \hspace{1cm} \sigma^{2} = \frac{V}{2 \pi^{2}} \int_{0}^{\infty} P(k) k^{2} \; \mathrm{d} k \quad \propto k^{n+3}$$
> 
> When $n=1$, the spectrum is "scale invariant", meaning that all perturbations enter the horizon at the same time.
> 
> From [[Instruments#WMAP]] and [[Catalogs#SDSS]], we have: $n = 0.953 \pm 0.016$, $\sigma_{8} = 0.756 \pm 0.035$

Dark matter simulations have found that halos are anti-biased with respect to the overall mass ($b < 1$). This means that the fluctuations in galaxy number density are smaller than that of mass due to the excessive merging of halos compared with real galaxies. This results in very large halos.

Alternatively, [[Cosmic Microwave Background|CMB]] measurements (from variations of the matter power spectrum on $8\,\pu{Mpc/h}$ scales, $\sigma_8$) have yielded a very different value of $b \simeq 1.5$ with the opposite conclusion; galaxies are more tightly clustered (higher number overdensities) than all mass.

