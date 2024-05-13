---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - intensity
  - intensies
  - surface brightness
  - Surface Brightness
  - radiant intensity
  - radiation intensity
---
*(Helpful Resource: https://www.cv.nrao.edu/~sransom/web/Ch2.html)*

![[intensity_angles.png|align:center|400]]


![[intensity_perspectives.png|align:center|400]]

**(Radiant) Intensity** or **surface brightness** ($I$) is the [[Flux|radiant flux]] per steradian, where the area is measured on the plane is perpendicular to the direction of energy propagation and the emitting source is contained in the observable solid angle.
$$
I \propto \frac{\mathrm{d} E}{\mathrm{d} A_{\perp} \, \mathrm{d} t \, \mathrm{d} \Omega} \hspace{1cm} \text{where} \hspace{1cm} [ \, I \, ] \equiv \left(\frac{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm steradian}}\right) = \left(\frac{{\rm flux}}{{\rm steradian}}\right) = MT^{-3}
$$

## Specific Intensity
*(Also known as **spectral intensity** or **intensity density**)*

More often in astronomy, we discuss the **specific intensity** that refers to the **intensity density** in frequency space. Similar to the [[Flux#Specific Flux|flux density]], we use $I_{\nu}$ to represent the intensity in the frequency band from $[\nu,\nu + d\nu]$.

$$
I = \int_{0}^{\infty} I_{\nu} \; \mathrm{d} \nu \hspace{1cm} \text{where} \hspace{1cm} [ \, I_{\nu} \, ] \equiv \left(\frac{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm steradian} \times {\rm Hertz}}\right)  = M T^{-2} St^{-1}
$$

From an observational perspective, we can write the follow *foundational equation* for deriving the other intensity/flux relationships. This expression is composed by simply trying to account for the major contributions that can affect specific intensity.

$$\mathrm{d} E_{\nu} = I_{\nu} \; ( \mathrm{d} A \, \cos \theta ) \; \mathrm{d} \Omega \; \mathrm{d} \nu \; \mathrm{d} t \hspace{1cm} \text{where} \hspace{1cm} \mathrm{d} A_{\perp} = \mathbf{\mathrm{d} A} \cdot \mathbf{\hat{n}} = \mathrm{d} A \cos \theta$$

Carefully rearranging, we can easily define a relationship between [[Flux#Specific Flux|specific flux]] and specific intensity.

$$F_{\nu} = \int_{\Omega} \frac{\mathrm{d} E_{\nu}}{\mathrm{d} A \, \mathrm{d} t \, \mathrm{d} \nu} = \int_{\Omega} I_{\nu} \cos \theta \; \mathrm{d} \Omega $$

> [!measure] Intensity Scaling
> After showing that [[Flux#^fdb0f0|flux scales with the inverse-square law]], we can use this result to show that **intensity is an intrinsic property** of a source, such that it is not dependent on the parameters of the observer.
> 
> $$
> F_{\nu} \propto \frac{1}{r^2}
> \hspace{1cm}
> \mathrm{d} \Omega = \frac{\mathrm{d} A}{r^2}
> \hspace{1cm} \Rightarrow \hspace{1cm}
> I_{\nu} = \frac{F_{\nu}}{\mathrm{d} \Omega} \propto {\rm constant}
> $$
> 
> In other words, we can state that $I_{\rm \nu}$ is conserved along any ray in empty space.
> $$\frac{\mathrm{d} I_{\nu}}{\mathrm{d} s} = 0$$
> *(See the [[Radiative Transfer Equation]] for non-empty space)*

## Related Definitions

### Specific Flux Density

$$F_{\nu} = \int_{\Omega} \frac{\mathrm{d} E_{\nu}}{\mathrm{d} A \, \mathrm{d} t \, \mathrm{d} \nu} = \int_{\Omega} I_{\nu} \cos \theta \; \mathrm{d} \Omega \hspace{1cm} \text{where} \hspace{1cm} [ \, F_{\nu} \, ] \equiv \left(\frac{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm hertz}}\right) = MT^{-2}$$

*(See [[Flux#Specific Flux]] for more details...)*

### Specific Mean Intensity

The **specific mean intensity** ($J_{\nu}$) is the average intensity density in all directions from an observing surface. To calculate this quantity, we integrate over the solid angle and divide by $4\pi$ (since there are $4\pi$ steradians on a sphere).
$$J_{\nu} = \frac{\int_{\Omega} I_{\nu} \; \mathrm{d} \Omega}{\int_{\Omega} \mathrm{d} \Omega} = \frac{1}{4 \pi} \int_{\Omega} I_{\nu} \; \mathrm{d} \Omega$$

If a source has an isotropic emission: $J_{\nu} = I_{\nu}$.

### Specific Energy Density

The **specific mean energy** ($U_{\nu}$) is the average energy density in all directions from an observing surface. To calculate this quantity, we integrate over the solid angle and divide by the speed of light ($c$).

$$U_{\nu} = \int_{\Omega} \frac{\mathrm{d} E_{\nu}}{(\mathrm{d} A \, \cos\theta) \, (c \, \mathrm{d} t) \, \mathrm{d} \nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \; \mathrm{d} \Omega$$

If a source has an isotropic emission: $U_{\nu} = \frac{4 \pi}{c} I_{\nu}$

### Specific Radiation Pressure

The **specific radiation pressure** ($P_{\nu}$) is pressure of the radiation field over a surface. It is given by the perpendicular force ($\mathrm{d} E_{\nu} \cos \theta / (c \, \mathrm{d} t)$) over the observing surface ($\mathrm{d} A$) in the specific frequency band ($\mathrm{d} \nu$). After integrating over all directions...

$$
\underbrace{\left(\frac{\mathrm{d} E_{\nu} \, \cos \theta}{c \, \mathrm{d} t}\right)}_{\rm force} \cdot \underbrace{\left(\frac{1}{\mathrm{d} A}\right)}_{\rm area} \cdot \frac{1}{\mathrm{d} \nu} = \frac{I_{\nu} \cos^{2} \theta}{c} \; \mathrm{d} \Omega 
\hspace{1cm} \Rightarrow \hspace{1cm}
P_{\nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \, \cos^{2} \theta\; \mathrm{d} \Omega
$$

If a source has an isotropic emission: $P_{\nu} = \frac{4 \pi}{3 c} I_{\nu} =  \frac{1}{3} U_{\nu}$


## Frequency-Wavelength Conversion

$$\nu = \frac{c}{\lambda} \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} \nu = -\frac{c}{\lambda^{2}} \; \mathrm{d} \lambda$$

We can convert all of the prior relationships into terms of wavelength by using the above relationship between $\lambda$ and $\nu$. To do the conversion, we need to remember that to convert *densities*, such that we perform a change of variables under an integral sign.

For example, here we convert the specific flux under the integral of the associated frequency band.
$$
\begin{aligned}[b]
	F &= \int_{\nu_{\rm A}}^{\nu_{\rm B}} F_{\nu}(\nu,T) \; \mathrm{d} \nu \\
	&= \int_{\nu_{\rm A}}^{\nu_{\rm B}} F_{\nu}(\nu,T) \; \left(\frac{\mathrm{d} \nu}{\mathrm{d} \lambda}\right) \; \mathrm{d} \lambda \\
	&= \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} F_{\nu}(\nu,T) \left(-\frac{c}{\lambda^{2}}\right) \; \mathrm{d} \lambda \\
	&= - \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} F_{\lambda}(\lambda,T) \; \mathrm{d} \lambda \\
	&= \int_{\lambda_{\rm B}}^{\lambda_{\rm A}} F_{\lambda}(\lambda,T) \; \mathrm{d} \lambda \\
\end{aligned}
\hspace{1cm} \Rightarrow \hspace{1cm}
F_\lambda(\lambda,T) = \frac{c}{\lambda^{2}} F_{\nu} \left(\frac{c}{\lambda},T\right)
$$

> [!note]
> We drop the minus sign because we integrate in the opposite direction for $\lambda$ so the definition of $X_\lambda$ is nice. 
