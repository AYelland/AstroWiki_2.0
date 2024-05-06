---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---

> [!key-idea]
> Good Sources:
> - http://spiff.rit.edu/classes/phys440/lectures/optd/optd.html
> - https://www.astro.uvic.ca/~tatum/stellatm/atm5.pdf
> 
> You'll notice many of the things below are just describing the same thing in different ways. In the end, all of them tie back to this core relationship.
> $$\alpha = \frac{1}{l} = \rho\kappa = n \sigma = \td{\tau}{z}$$

## Kirchoff's Law of Radiation

**Kirchoff's Law** makes three statements:

1. A perfect black body in thermodynamic equilibrium is the perfect insulator (absorbs all light that strikes it) and radiator (emits energy according to [[Blackbody Radiation#Stefan-Boltzmann Law]], universal for all perfect black bodies).

2. For an arbitrary body emitting and absorbing thermal radiation in thermodynamic equilibrium, the emissivity is equal to the absorptivity. (see [[Radiative Transfer Equation|RTE]]) $$\td{I_{\nu}}{z} = j_{\nu} - \alpha_{\nu} I_{\nu} = 0 \hRightarrow j_{\nu} = \alpha_{\nu} I_{\nu} = \alpha_{\nu} B_{\nu}(T)$$
3. The emissivity of a source cannot exceed one (because the absorptivity cannot exceed one by conservation of energy), and thus, it is not possible to thermally radiate more energy than a black body, at equilibrium.

## Mean Free Path

$$l = \frac{1}{n \sigma} \hWhere 
\begin{align}
	n &\equiv \text{number (volume) density} \\
	\sigma &\equiv \text{scattering cross sectional area} \\
\end{align}$$

The **Mean Free Path** is the scale length for a scattering process. For a material of size $L$, the probability of a particle scattering while traveling some distance ($\rd x$)...

![[Mean_free_path.png|align:center]]

$$\mathcal{P} = \int \fpar{\text{area of scatterers}}{\text{area of target}} = \int\frac{\sigma \left( n \times L^{2} \; \rd x\right)}{L^{2}} = \int n \sigma \; \rd x$$

For incident flux ($F$) on the differential length of material, we have...

$$\rd F = - F n \sigma \, \rd x$$

...which we can solve to get **Lambert-Beer Law**, which relates the incident flux from a source ($F_{0}$) to the [[#Optical Depth]] ($\tau$).

$$\int \frac{\rd F}{F} = - n \sigma \int \rd x \hRightarrow F = F_{0} e^{-x/l} = F_{0} e^{-\tau}$$^lambert-beer-law

> [!note]
> We use [[Flux|flux]] instead of [[Intensity|intensity]] as one might see on wikipedia. This is done to avoid confusion with the prevalent astronomy usage of these terms.

## Optical Thickness

The **Optical Thickness** is a loosely defined notion of "how difficult it is for light to get through a unit length of this material". Thickness is an appropriate word because when thinking about distance in terms of [[#Optical depth|optical depth]]. A "thick" material is one which has a very short mean free path, and thus a large optical depth. the converse is true for a "thin" material.

- **Optically thick**: Many [[#Mean free path|mean free paths]] per unit length
- **Optically thin**: Few [[#Mean free path|mean free paths]] per unit length

## Extinction Coefficient

$$\alpha = \frac{1}{l} \hWhere l \equiv \text{mean free path}$$

The **Extinction Coefficient** is the inverse of the [[#Mean Free Path|mean free path]], and has dimensions of inverse length. It is a combination of the effects of absorption and scattering. 

A high extinction corresponds to short mean free path, and thus, light has a "harder time" moving through the material.

## Opacity
(also known as the "absorption coefficient"?)

**Rosseland Mean Opacity** ($\kappa$) is the frequency-independent efficiency at which a particular medium absorbs and scatters light, with dimensions of "cross section per mass". It can be defined as:

$$\alpha = \frac{1}{l} = \rho\kappa = n \sigma = \td{\tau}{z}$$

where
- $\kappa \equiv$ Rosseland Mean Opacity $\in [0,1]$ ($0=\text{transparent}$, $1=\text{opaque}$)
- $\rho \equiv$ Mass Density
- $l \equiv$ [[#Mean Free Path]]
- $n \equiv$ number (volume) density
- $\sigma \equiv$ scattering cross section
- $\alpha \equiv$ [[#Extinction Coefficient]]

**Opacity** is usually frequency-dependent though, and thus, the Rosseland Mean Opacity is typically defined terms of the frequency-dependent opacity ($\kappa_{\nu}$).

$$\frac{1}{\kappa} = \frac{\int_{0}^{\infty} \frac{1}{\kappa_{\nu}} \pd{B_{\nu}}{T} \; \rd \nu}{\int_{0}^{\infty} \pd{B_{\nu}}{T} \; \rd \nu} \hWhere B_{\nu} \equiv \text{blackbody spectral density}$$

> [!note]
> In principle, $\kappa$, $\sigma$ and $\alpha$ are all frequency-dependent.

## Kramer's Opacity Law

**Kramer's Opacity Law** directly correlates the density and temperature of the medium to the average opacity. It can be derived from the Rosseland Mean Opacity for [[Bremsstrahlung Radiation|bremsstrahlung radiation]]. (skipped)

$$
\bar{\kappa} \propto \rho T^{-7/2} \hWhere
\begin{aligned}
	\bar{\kappa} &\equiv \text{average opacity} \\
	\rho &\equiv \text{density of medium} \\
	T &\equiv \text{temperature of medium} \\
\end{aligned}
$$

Here, we can see that the opacity higher (more opaque) at lower temperatures.

## Optical Depth

The **Optical Depth** ($\tau \equiv \tau_{\nu}$) is a frequency-dependent measurement that relates a physical distance to the absorptivity of a material over that distance. It can be thought of as the number of [[#Mean Free Path|mean free paths]] transversed in the given medium.

$$\tau(z) = \int_{0}^{z} \alpha \; \rd z = \int_{0}^{z} \kappa \rho \; \rd z = \int_{0}^{z} \sigma n \; \rd z \underbrace{= \; \sigma N}_{\text{uniform material}}$$

where
- $\alpha \equiv$ [[#Extinction Coefficient]]
- $\kappa \equiv$ [[#Opacity]]
- $\rho \equiv$ density of medium
- $\sigma \equiv$ scattering cross section
- $N \equiv$ column number density ($\rm{particles\,m^{-2}}$)

For a uniform material, the optical depth is just the length of the material transversed / mean free path.

*(Note: This is the measure you use when what you care about is "how much light is absorbed".)*

People often define the optical depth using the Rosseland mean [[#Opacity|opacity]], whereby $\alpha = \kappa \rho$ (as above) is frequency-independent. For the **frequency-dependent** optical depth:

$$\tau_{\nu}(z) = \int_{0}^{z} \alpha_{\nu} \; \rd z = \int_{0}^{z} \kappa_{\nu} \, \rho \; \rd z$$

> [!note]- From the Radiative Transfer Equation
> If we only consider the absorption term in the [[Radiative Transfer Equation|RTE]], then we can define optical depth ($\tau_{\nu}(z)$) as the exponential index.
> 
> $$\td{I_{\nu}}{z} = - \alpha_{\nu} I_{\nu} \hRightarrow I_{\nu}(z) = I_{\nu,0} \exp \underbrace{\left[ - \int_{0}^{z} \alpha_{\nu}(z') \; \rd z' \right]}_{- \tau_{\nu}(z) \equiv \text{optical depth}} = = I_{\nu,0} e^{- \tau_{\nu}(z)}$$
> $$\Downarrow$$
> $$\text{optical depth} \equiv \quad \tau_{\nu}(z) = \int_{0}^{z} \alpha_{\nu}(z') \; \rd z' \hRightarrow \rd \tau_{\nu} = \alpha_{\nu} \; \rd z$$



