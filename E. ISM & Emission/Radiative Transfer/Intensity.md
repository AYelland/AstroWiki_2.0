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
I \propto \frac{\rd E}{\rd A_{\perp} \, \rd t \, \rd \Omega} \hWhere [ \, I \, ] \equiv \fpar{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm steradian}} = \fpar{{\rm flux}}{{\rm steradian}} = MT^{-3}
$$

## Specific Intensity
*(Also known as **spectral intensity** or **intensity density**)*

More often in astronomy, we discuss the **specific intensity** that refers to the **intensity density** in frequency space. Similar to the [[Flux#Specific Flux|flux density]], we use $I_{\nu}$ to represent the intensity in the frequency band from $[\nu,\nu + d\nu]$.

$$
I = \int_{0}^{\infty} I_{\nu} \; \rd \nu \hWhere [ \, I_{\nu} \, ] \equiv \fpar{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm steradian} \times {\rm Hertz}}  = M T^{-2} St^{-1}
$$

From an observational perspective, we can write the follow *foundational equation* for deriving the other intensity/flux relationships. This expression is composed by simply trying to account for the major contributions that can affect specific intensity.

$$\rd E_{\nu} = I_{\nu} \; ( \rd A \, \cos \theta ) \; \rd \Omega \; \rd \nu \; \rd t \hWhere \rd A_{\perp} = \mathbf{\rd A} \cdot \mathbf{\hat{n}} = \rd A \cos \theta$$

Carefully rearranging, we can easily define a relationship between [[Flux#Specific Flux|specific flux]] and specific intensity.

$$F_{\nu} = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t \, \rd \nu} = \int_{\Omega} I_{\nu} \cos \theta \; \rd \Omega $$

> [!measure] Intensity Scaling
> After showing that [[Flux#^fdb0f0|flux scales with the inverse-square law]], we can use this result to show that **intensity is an intrinsic property** of a source, such that it is not dependent on the parameters of the observer.
> 
> $$
> F_{\nu} \propto \frac{1}{r^2}
> \hspace{1cm}
> \rd \Omega = \frac{\rd A}{r^2}
> \hRightarrow
> I_{\nu} = \frac{F_{\nu}}{\rd \Omega} \propto {\rm constant}
> $$
> 
> In other words, we can state that $I_{\rm \nu}$ is conserved along any ray in empty space.
> $$\td{I_{\nu}}{s} = 0$$
> *(See the [[Radiative Transfer Equation]] for non-empty space)*

## Related Definitions

### Specific Flux Density

$$F_{\nu} = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t \, \rd \nu} = \int_{\Omega} I_{\nu} \cos \theta \; \rd \Omega \hWhere [ \, F_{\nu} \, ] \equiv \fpar{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm hertz}} = MT^{-2}$$

*(See [[Flux#Specific Flux]] for more details...)*

### Specific Mean Intensity

The **specific mean intensity** ($J_{\nu}$) is the average intensity density in all directions from an observing surface. To calculate this quantity, we integrate over the solid angle and divide by $4\pi$ (since there are $4\pi$ steradians on a sphere).
$$J_{\nu} = \frac{\int_{\Omega} I_{\nu} \; \rd \Omega}{\int_{\Omega} \rd \Omega} = \frac{1}{4 \pi} \int_{\Omega} I_{\nu} \; \rd \Omega$$

If a source has an isotropic emission: $J_{\nu} = I_{\nu}$.

### Specific Energy Density

The **specific mean energy** ($U_{\nu}$) is the average energy density in all directions from an observing surface. To calculate this quantity, we integrate over the solid angle and divide by the speed of light ($c$).

$$U_{\nu} = \int_{\Omega} \frac{\rd E_{\nu}}{(\rd A \, \cos\theta) \, (c \, \rd t) \, \rd \nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \; \rd \Omega$$

If a source has an isotropic emission: $U_{\nu} = \frac{4 \pi}{c} I_{\nu}$

### Specific Radiation Pressure

The **specific radiation pressure** ($P_{\nu}$) is pressure of the radiation field over a surface. It is given by the perpendicular force ($\rd E_{\nu} \cos \theta / (c \, \rd t)$) over the observing surface ($\rd A$) in the specific frequency band ($\rd \nu$). After integrating over all directions...

$$
\underbrace{\fpar{\rd E_{\nu} \, \cos \theta}{c \, \rd t}}_{\rm force} \cdot \underbrace{\fpar{1}{\rd A}}_{\rm area} \cdot \frac{1}{\rd \nu} = \frac{I_{\nu} \cos^{2} \theta}{c} \; \rd \Omega 
\hRightarrow
P_{\nu} = \frac{1}{c} \int_{\Omega} I_{\nu} \, \cos^{2} \theta\; \rd \Omega
$$

If a source has an isotropic emission: $P_{\nu} = \frac{4 \pi}{3 c} I_{\nu} =  \frac{1}{3} U_{\nu}$


## Frequency-Wavelength Conversion

$$\nu = \frac{c}{\lambda} \hRightarrow \rd \nu = -\frac{c}{\lambda^{2}} \; \rd \lambda$$

We can convert all of the prior relationships into terms of wavelength by using the above relationship between $\lambda$ and $\nu$. To do the conversion, we need to remember that to convert *densities*, such that we perform a change of variables under an integral sign.

For example, here we convert the specific flux under the integral of the associated frequency band.
$$
\begin{aligned}[b]
	F &= \int_{\nu_{\rm A}}^{\nu_{\rm B}} F_{\nu}(\nu,T) \; \rd \nu \\
	&= \int_{\nu_{\rm A}}^{\nu_{\rm B}} F_{\nu}(\nu,T) \; \left(\td{\nu}{\lambda}\right) \; \rd \lambda \\
	&= \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} F_{\nu}(\nu,T) \left(-\frac{c}{\lambda^{2}}\right) \; \rd \lambda \\
	&= - \int_{\lambda_{\rm A}}^{\lambda_{\rm B}} F_{\lambda}(\lambda,T) \; \rd \lambda \\
	&= \int_{\lambda_{\rm B}}^{\lambda_{\rm A}} F_{\lambda}(\lambda,T) \; \rd \lambda \\
\end{aligned}
\hRightarrow
F_\lambda(\lambda,T) = \frac{c}{\lambda^{2}} F_{\nu} \left(\frac{c}{\lambda},T\right)
$$

> [!note]
> We drop the minus sign because we integrate in the opposite direction for $\lambda$ so the definition of $X_\lambda$ is nice. 
