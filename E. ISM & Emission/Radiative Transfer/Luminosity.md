---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - luminosity
  - luminosities
---

**Luminosity** is an intrinsic property of a source measuring the total amount of radiant power (electromagnetic energy emitted per unit of time) by an astronomical object.

Luminosity is quoted in units of 
- solar luminosity ($L_{\odot}$)
- Watts ($W = J/s$) for the SI unit system
- erg per sec (${\rm erg/s}$) in the CGS unit system
- electron volts ($eV$) for high energy physics/phenomenology

## Relationship to Flux

The relationship of luminosity is closely related to the [[Flux#Specific Flux|flux density]] of a source. If a source emits isotropically with a constant luminosity ($L$), then as the distance to the observing surface increases, there is a decrease in observed [[Intensity|surface brightness/flux]].
$$L = \int F \; \rd A$$
If you take the observed [[flux]] to be constant from an isotropically emitting source...
$$
L = (F \cdot A) = F \left[ 4 \pi D_{\rm L}^{2} \right] = F \left[ 4 \pi (a_{0} r (1 + z))^{2} \right] \hRightarrow F = \frac{L}{4 \pi D_{\rm L}^{2}}
$$
where
$$\begin{aligned}
	D_{\rm L} &\equiv \text{Luminosity Distance} = a_{0} r (1 + z) \\
	a_{0} &\equiv \text{Friedmann Scale Factor (present day)}
\end{aligned}$$

...then we can express the luminosity in terms of the [[Distances#Luminosity Distance|luminosity distance]], where the correction is related to the conversion of [[Distances#Comoving Distance|comoving distance]] to the [[Distances#Proper Distance|proper distance]].

## Relationship to Intensity

In terms of specific intensity, we can define this quantity as an integral.

$$
    L = \td{E}{t} = \int I_{\nu} \; \rd A \, \rd \Omega \, \rd \nu \hWhere \left[ L \right] \equiv {\rm erg \; s^{-1}} = {\rm Watts}
$$

Intrinsic property of a source.

## Relationship to Magnitude

The difference in [[Magnitude#Bolometric Magnitude|bolometric magnitude]] between two sources is related to their luminosity ratio according to:

$$M_{\rm bol,1}-M_{\rm bol,2}=-2.5\log _{10}{\fpar{L_{1}}{L_{2}}}$$

## Eddington Limit

The **Eddington Limit** (or **Eddington Luminosity**) is the maximum luminosity a spherical astrophysical body can achieve when in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]], where the gravitational pressure is balanced with the radiation pressure. 

$$
L_{\rm Edd} = \frac{4 \pi G M c}{\kappa} \approx 3.2 \times 10^{4} \; \fpar{M}{M_{\odot}} \fpar{\kappa_{\odot}}{\kappa} \; L_{\odot}
$$

When a star exceeds the Eddington luminosity, it develops very intense, radiation-driven, stellar wind on its outer layers.

> [!derivation]-
> 
> To derive the limit, we assume the luminous mass ($M$) is composed purely of ionized hydrogen and that the opacity ($\kappa = \sigma_{\rm T} / m_{\rm p}$) is constant (originating entirely from [[Thomson Scattering]] with cross-section $\sigma_{\rm T}$).
> 
> Beginning with the [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]] relationship and the radiation pressure gradient, we will equate the two to find the maximum luminosity when the two forces are balanced.
> 
> $$
> \td{P_{\rm grav}}{r} = - \frac{G M \rho}{r^{2}} \hspace{2cm} \td{P_{\rm rad}}{r} = - \frac{\rho \, \kappa}{c} \, F_{\rm rad}  = - \frac{\rho \, \kappa}{c} \, \fpar{L}{4 \pi r^{2}}
> $$
> $$
> \begin{align}
> 	\td{P_{\rm rad}}{r} &= \td{P_{\rm grav}}{r} \\
> 	- \frac{\rho \, \kappa}{c} \, \fpar{L}{4 \pi r^{2}} &= - \frac{G M \rho}{r^{2}} \\
> 	L &= 4 \pi r^{2} \fpar{G M \rho}{r^{2}} \fpar{c}{\rho \, \kappa} \\
> 	L &= \fpar{4 \pi G M c}{\kappa} \\
> \end{align}
> $$
> 
> Converting to [[Sun|solar]] units, we define the **Eddington Luminosity**.
> 
> $$
> L_{\rm Edd} \equiv \underbrace{\fpar{4 \pi G M_{\odot} c}{\kappa_{\odot} \, L_{\odot}}}_{\rm constant} \fpar{M}{M_{\odot}} \fpar{\kappa_{\odot}}{\kappa} \, L_{\odot} \; \approx \; 3.2 \times 10^{4} \fpar{M}{M_{\odot}} \fpar{\kappa_{\odot}}{\kappa} \, L_{\odot}
> $$
> 
> Any luminous source that exceeds this limit ($L > L_{\rm Edd}$) will start loosing mass through radiation. If the luminosity is less than this limit ($L < L_{\rm Edd}$) will being gravitationally contracting until hydrostatic equilibrium is reached.

