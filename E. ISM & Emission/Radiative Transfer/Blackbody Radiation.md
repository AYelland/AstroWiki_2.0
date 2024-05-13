---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - BB radiation
  - Blackbody radiation
  - blackbody radiation
  - BB
  - blackbody
  - blackbodies
---
*(Helpful Resource: https://www.cv.nrao.edu/~sransom/web/Ch2.html)*

> [!note] Blackbody = Perfect emitter/absorber = Most efficient radiator

## Stefan-Boltzmann Law

The [[flux]] emitted from a blackbody is directly proportional to the fourth power of the temperature times the Stefan-Boltzmann constant ($\sigma$).
$$F_{\rm BB} = \sigma T^{4} \hspace{1cm} \text{where} \hspace{1cm} \sigma \equiv \frac{2 \pi^{5} k_{\rm B}^{4}}{15 h^{3} c^{2}} \quad \textcolor{gray}{\simeq 5.67 \times 10^{-8} \; \frac{{\rm J}}{\rm m^{2} \, s \, K^{4}}}$$

### Blackbody Luminosity

The associated [[Luminosity|luminosity]] of a blackbody emitting isotropically is then:
$$\mathrm{d} L = \mathrm{d} A \; \sigma T^{4} \hspace{1cm} \Rightarrow \hspace{1cm} L = A \sigma T^{4} = \left( 4 \pi R^{2} \right) \sigma T^{4}$$

### Effective Temperature

If we map the observed luminosity of an astrophysical body (i.e. star) to a blackbody, then we can define a non-physical temperature called the **effective temperature** of that body.
$$T_{\rm eff} \equiv \left(\frac{L}{4 \pi \sigma R^{2}}\right)^{1/4} \hspace{1cm} \text{where} \hspace{1cm} L = 4 \pi d^{2} F_{\rm obs}$$

## Blackbody Specific Intensity
*(Also known as **Blackbody Spectral Density**)*

![[blackbody.svg|align:center|450]]
![[blackbody_frequency.png|align:center|550]]

Through **Planck's Law**, we can define the spectral density of electromagnetic radiation emitted by a blackbody in thermal equilibrium at a given temperature. This is equivalent to defining the spectral density energy and the [[Intensity#Specific Intensity|specific intensity]] of a blackbody.

$$u_{\nu}(\nu,T) = \frac{2 h \nu^{3}}{c^{2}} \frac{1}{e^{h \nu / k_{\rm B} T} -1}$$
$$\boxed{ \; B_{\nu}(\nu,T) = \frac{2 h \nu^{3}}{c^{2}} \left(\frac{1}{e^{h \nu / k_{\rm B} T} - 1}\right) \; } \hspace{1cm} \text{where} \hspace{1cm} [ \, B_{\nu} \, ] \equiv \left(\frac{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm steradian} \times {\rm Hertz}}\right)$$

In terms of other units:
![[blackbody_specificIntensity.png|align:center]]

*(If you want to play with an [interactive PHET simulation](https://phet.colorado.edu/sims/html/blackbody-spectrum/latest/blackbody-spectrum_en.html)...)*


> [!cian] Redshifted Temperature
> Effective temperature gets redshifted as $$T_{obs} = \frac{T_{emit}}{1+z}$$Why? When you redshift the blackbody spectrum in a constantly proportional way $\nu_{emit} \rightarrow \nu_{obs} = c\nu_{emit}$ for all $\nu$ (here $c = (1+z)^{-1}$, see [[Redshift|redshift]]) it has the effect of introducing an effective temperature $T_{eff} = T_{emit}/(1+z)$ so redshifts maintain the BB spectrum form with a different temperature (note this will be a contravariant transformation of $\nu$ so even though $\nu \rightarrow c\nu$ we must actually apply the inverse transformation to the variable in the distribution) $$\mathrm{BB}\sim\exp\left(\frac{h\nu}{kT_{emit}}\right) \longrightarrow \exp\left(\frac{h(1+z)\nu}{kT_{emit}}\right)$$ where the RHS is what we observe, such that effectively we have $$\implies T_{obs} = \frac{T_{emit}}{1+z}$$
> isnt it actually that (1+z)Temit = Tobs? It cant be that since Tobs must be less than Temit for z>0. I think its a covariant vs contravariant thing. We're transforming the x axis rather than the curve maybe?

## Wien's Displacement Law

**Wien's displacement law** states that the black-body radiation curve for different temperatures will peak at different wavelengths that are inversely proportional to the temperature.

$$\lambda_{peak} \propto \frac{1}{T}$$

![[wiens_displacementLaw.png|align:center]]

The constant of proportionality (*Wien's Displacement Constant*) depends on the solution of an implicit equation. It is usually quoted as...

$$\lambda_{peak} \simeq \frac{b}{T} \hspace{1cm} \text{where} \hspace{1cm} b \approx 2.89777 \times 10^{-3} \; {\rm m \, K} \textcolor{gray}{\simeq 3 \times 10^{-3} \; {\rm m \, K}}$$

Expressing this peak as energy through the energy-wavelength relation.

$$E_{\rm peak} = h \nu_{\rm peak} = \frac{h c}{\lambda_{\rm peak}} = \left(\frac{h c}{b}\right) T \simeq \left(\frac{10^{-6} \; {\rm eV \ m}}{3 \times 10^{-3} \; {\rm m\ K}}\right) T \simeq \left(3 \times 10^{-4} \; T \right)\,\pu{eV}$$

> [!temperature] At room temperature... 
> If we take room temperature as ($T \sim 300 \; {\rm K}$), peak of the distribution is at:
> $$\lambda_{\rm peak} \sim \frac{0.003 \; {\rm m \, K}}{300 \; {\rm K}} \sim 10^{-5} \; {\rm m} \sim 10 \; {\rm micron}$$

> [!derivation]- Derivation of Wien's Law from Plank's Law
> We us a wavelength parameterization of the [[#Blackbody Specific Intensity|spectral density energy]] and find the maximum of the distribution by differentiating with respect to the wavelength, $\lambda$.
> $$u_{\lambda}(\lambda,T) = \frac{2 h c^{2}}{\lambda^{5}} \frac{1}{e^{h c / \lambda k_{\rm B} T} -1}$$
> $$\frac{\partial u_{\lambda}}{\partial \lambda} = 2 h c^{2} \left( \frac{h c}{k_{\rm B} T \lambda^{7}} \frac{e^{h c / \lambda k_{\rm B} T}}{\left( e^{h c / \lambda k_{\rm B} T} - 1 \right)^{2}} - \frac{1}{\lambda^{6}} \frac{5}{e^{h c / \lambda k_{\rm B} T} - 1} \right) = 0$$
> This is solved by:
> $$\frac{x e^{x}}{e^{x} - 1} - 5 = 0 \hspace{1cm} \Rightarrow \hspace{1cm} x = 5 + W_{0}(-5 e^{-5})$$
> where
> $$x \equiv \frac{h c}{\lambda k_{\rm B} T} \hspace{2cm} W_{0}(z) \equiv \textit{Lambert W function}$$
> $$\Downarrow$$
> $$\text{Wien's Displacement Constant} \equiv b = \lambda_{\rm peak} T = 2.89777 \times 10^{-3} \; {\rm m \, K}$$

## Rayleigh-Jeans Law

Similar to [[#Wien's Displacement Law]], the **Rayleigh–Jeans law** is an approximation for blackbody radiation as a function of wavelength at a given temperature.

$$B_{\lambda}(T) = \frac{2 c k_{\rm B} T}{\lambda^{4}} \hspace{2.5cm} B_{\nu}(T) = \frac{2 \nu^{2} k_{\rm B} T}{c^{2}}$$

The Rayleigh–Jeans law agrees with experimental results at large wavelengths (low frequencies) but strongly disagrees at short wavelengths (high frequencies).

## Related Definitions

### Blackbody Specific Flux Density

$$F_{\nu} = \int_{\Omega} I_{\nu} \cos \theta \; \mathrm{d} \Omega = \int_{\Omega} B_{\nu} \cos \theta \; \mathrm{d} \Omega$$

*(See [[Intensity#Specific Flux Density]] for more details...)*

### Blackbody Specific Mean Intensity

Given that a blackbody emits isotropically, the **specific mean intensity** ($J_{\nu}$) is...
$$J_{\nu} = \frac{\int_{\Omega} I_{\nu} \; \mathrm{d} \Omega}{\int_{\Omega} \mathrm{d} \Omega} = \frac{1}{4 \pi} \int_{\Omega} I_{\nu} \; \mathrm{d} \Omega = B_{\nu}(T)$$

*(See [[Intensity#Specific Mean Intensity]] for more details...)*

### Blackbody Specific Energy Density

Given that a blackbody emits isotropically, the **specific mean energy** ($U_{\nu}$) is...

$$U_{\nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \; \mathrm{d} \Omega = \frac{4 \pi}{c} B_{\nu}(T)$$

*(See [[Intensity#Specific Energy Density]] for more details...)*

### Blackbody Specific Radiation Pressure

Given that a blackbody emits isotropically, the **specific radiation pressure** ($P_{\nu}$) is...

$$
P_{\nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \, \cos^{2} \theta\; \mathrm{d} \Omega = \frac{4 \pi}{3 c} B_{\nu}(T)
$$

*(See [[Intensity#Specific Radiation Pressure]] for more details...)*

## Frequency-Wavelength Conversion

$$\nu = \frac{c}{\lambda} \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} \nu = -\frac{c}{\lambda^{2}} \; \mathrm{d} \lambda$$

We can convert all of the prior relationships into terms of wavelength by using the above relationship between $\lambda$ and $\nu$. To do the conversion, we need to remember that to convert *densities*, such that we perform a change of variables under an integral sign.

$$
\begin{aligned}[b]
	B &= \int_{\nu_{\rm A}}^{\nu_{\rm B}} B_{\nu}(\nu,T) \; \mathrm{d} \nu \\
	&= \int_{\nu_{\rm A}}^{\nu_{\rm B}} B_{\nu}(\nu,T) \; \left(\frac{\mathrm{d} \nu}{\mathrm{d} \lambda}\right) \; \mathrm{d} \lambda \\
	&= \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} B_{\nu}(\nu,T) \left(-\frac{c}{\lambda^{2}}\right) \; \mathrm{d} \lambda \\
	&= - \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} B_{\lambda}(\lambda,T) \; \mathrm{d} \lambda \\
	&= \int_{\lambda_{\rm B}}^{\lambda_{\rm A}} B_{\lambda}(\lambda,T) \; \mathrm{d} \lambda \\
\end{aligned}
\hspace{1cm} \Rightarrow \hspace{1cm}
B_\lambda(\lambda,T) = \frac{c}{\lambda^{2}} B_{\nu} \left(\frac{c}{\lambda},T\right)
$$

> [!note]
> We drop the minus sign because we integrate in the opposite direction for $\lambda$ so the definition of $B_\lambda$ is nice. 
