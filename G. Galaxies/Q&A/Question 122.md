---
aliases:
  - correlation function
---
### Question
---
What is the galaxy correlation function? How do the correlation functions of galaxies and clusters of galaxies differ? How is the galaxy correlation function used to constrain H0?

### Answer
---
*(Source: [Hong et al.](https://arxiv.org/pdf/1202.0640.pdf))*
##### What is the galaxy correlation function?

The **galaxy correlation function** quantifies the likelihood of finding galaxy within a given distance to another galaxy. It is defined as the Fourier Transform of the Matter Power Spectrum $P(k)$, and can be represented through the average of overdensities in some volume of space.

$$1 + \xi(\vec{r}) = \frac{\expval{\rho(\vec{x}) \rho(\vec{x}+\vec{r})}}{\bar{\rho}^{2}} \hWhere \xi(\vec{r}) = \expval{\delta(\vec{x}) \delta(\vec{x} + \vec{r})}$$
where
- $\rho(\vec{x}) \equiv$ mass density at $\vec{x}$
- $\bar{\rho} \equiv$ average mass density in the universe
- $\delta(\vec{x}) \equiv$ overdensities of space at $\vec{x}$ (defined in the derivation)
- $\xi(\vec{r}) \equiv$ the *two-point correlation function* between galaxies.

Here, the bars and angular brackets refer to the average values and integrals over space, respectively. The chosen scale $\vec{r}$ tells us about correlations across a specific length scale, leading to interesting things such as measurements of [[Baryon Acoustic Oscillations|BAO]]

> [!derivation]
> To find this function, we assume that galaxy formation follows the perturbations in the mass density profile ($\rho(\vec{x})$) with respect to the mean density ($\bar{\rho}$). This allows us to define our overdensities ($\delta(\vec{x})$) as...
> 
> $$\delta(\vec{x}) = \frac{\rho(\vec{x}) - \bar{\rho}}{\bar{\rho}} \hspace{2cm} \delta(\vec{x}+\vec{r}) = \frac{\rho(\vec{x}+\vec{r}) - \bar{\rho}}{\bar{\rho}}$$
> 
> We can then ask ourselves *"What is the probability ($\rd P$) that we find two galaxies in volumes ($\rd V_{1}$, $\rd V_{2}$) separated by a distance ($\vec{r}$), with an average number density $(n_{\rm gal})$?"*
> 
> $$\begin{align}
> 	\rd P_{\rm real} = \rd P_{1} \cdot \rd P_{2} &= \left( n_{\rm gal} \cdot \frac{\rho(\vec{x})}{\bar{\rho}} \cdot \rd V_{1} \right) \cdot \left( n_{\rm gal} \cdot \frac{\rho(\vec{x}+\vec{r})}{\bar{\rho}} \cdot \rd V_{2} \right) \\
> 	&= n_{\rm gal}^{2} \bigg[ \left( 1 + \delta(\vec{x}) \right) \left( 1 + \delta(\vec{x}+\vec{r}) \right) \bigg] \; \rd V_{1} \; \rd V_{2} \\
> 	&= n_{\rm gal}^{2} \bigg[ 1 + \underbrace{\delta(\vec{x})}_{\approx \, 0} + \underbrace{\delta(\vec{x}+\vec{r})}_{\approx \, 0} + \underbrace{\delta(\vec{x}) \delta(\vec{x}+\vec{r})}_{\approx \, \xi(\vec{r})} \bigg] \; \rd V_{1} \; \rd V_{2} \\
> 	&= n_{\rm gal}^{2} \bigg[ 1 + \xi(\vec{r}) \bigg] \; \rd V_{1} \; \rd V_{2}
> \end{align}$$
> 
> where $\delta(\vec{x})$ and $\delta(\vec{x}+\vec{r})$ are zero on average, and $\xi(\vec{r})$ is the *two-point correlation function* related to the primordial power spectrum. For galaxies, it is the Fourier Transform of the galaxy power spectrum.
> $$\xi_{\rm gal} (\vec{r}) = \frac{V}{(2 \pi)^{3}} \int P(k) \, e^{i \vec{k} \cdot \vec{r}} \, \rd^{3} \vec{k}$$
> 
> > [!note]- Primordial Power Spectrum
> > The primordial power spectrum describes the initial perturbations in the universe leading to the structure-formation we observe today.
> > $$P(k) = A k^{n} \hRightarrow \sigma^{2} = \frac{V}{2 \pi^{2}} \int_{0}^{\infty} P(k) k^{2} \; \rd k \quad \propto k^{n+3}$$
> > When $n=1$, the spectrum is "scale invariant", meaning that all perturbations enter the horizon at the same time.
> 
> If we compare this probability function of finding a galaxy in the *real* universe relative to a *mock* universe constructed from a random, uniform distribution of galaxies...
> 
> $$\rd P_{\rm mock} = n_{\rm gal}^{2} \; \rd V_{1} \; \rd V_{2}$$
> 
> ...then we can define their ratio as the *galaxy correlation function*, with some separation $\vec{r}$.
> 
> $$\frac{\rd P_{\rm real}}{\rd P_{\rm mock}} = \underbrace{1 + \xi(\vec{r}) = \frac{\expval{\rho(\vec{x}) \rho(\vec{x}+\vec{r})}}{\bar{\rho}^{2}}}_{\text{galaxy correlation function}}$$

##### How do the correlation functions of galaxies and clusters of galaxies differ?

Observational measurements suggest that the two-point correlation function follows a power-law:

$$\xi(\vec{r}) \simeq \left(\frac{|\vec{r}|}{r_0}\right)^{-\gamma}$$

These measurements are made by using data from large surveys (i.e. [[Catalogs#eBOSS]] and [[Catalogs#SDSS]]) and comparing to simulation/mock random distributions matter.

**For Galaxies:**
A good fit for the power-law parameters is given by...

$$\gamma \simeq 1.7 \hspace{2cm} r_{0} \simeq 5 \; {\rm Mpc} \hRightarrow \xi_{\rm gal}(\vec{r}) \simeq \left(\frac{|\vec{r}|}{5 \; {\rm Mpc}}\right)^{-1.7}$$

On all scales, the galaxy two-point correlation function looks like a superposition of multiple power-laws, composed of galactic satellites and larger galactic clustering around/in dark matter halos. There is additional contributions from [[Baryon Acoustic Oscillations|BAO]] and early universe structure.

![[2_point_corr.png|align:center]]

**For Clusters:**
For [[Galaxy Cluster|galaxy clusters]], we can treat them as a single object, such that we use the two-point correlation function between two clusters. A good fit for the power-law parameters is given by...

$$\gamma = 2.1 \hspace{2cm} r_{0} = 17 \; {\rm Mpc} \hRightarrow \xi_{\rm cluster}(\vec{r}) \simeq \left(\frac{|\vec{r}|}{17 \; {\rm Mpc}}\right)^{-2.1}$$

This shows clusters are found to be much more strongly correlated in space than galaxies.

$$\xi_{\rm cluster} \simeq 20 \xi_{\rm gal}$$

Effectively, this means large-scale structure of the universe follows cluster formation as *more massive objects are more clustered* (modulo [[#120|galaxy bias]], which is less biased for clusters than for individual galaxies).

**For both fits:**

![[two-point-corr.png|align:center|500]]

##### How is the galaxy correlation function used to constrain H0?

If we measure the [[Distances#Angular Diameter Distance|angular size]] ($d_{\rm A}$) of the [[Baryon Acoustic Oscillations|BAO]] peak in a narrow range of [[Redshift|redshifts]] (i.e. $\Delta z \sim 0$ for roughly the same distance), then we can constrain $H_0$ using other parameters ($\Omega_{\rm M}$, $\Omega_{\Lambda}$) from [[Cosmic Microwave Background|CMB]] studies.

$$d_{\rm A}(z) = \frac{d_{\rm C}(z)}{1+z} = \frac{c}{H_{0}(1+z)} \int_{0}^{z} \frac{\rd z}{\sqrt{\Omega_{\rm M}(1+z)^{3} + \Omega_{\Lambda}}}$$

We can associate this measurement because the BAO scale is [[Distances#Comoving Distance|comoving]] with the Hubble flow, making it a standard ruler (similar [[Stellar Explosions#Type Ia|Type-Ia SNe]] "standard candle" or the "standard sirens" of compact object mergers.)