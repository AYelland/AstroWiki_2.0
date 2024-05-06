---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - flux
  - fluxes
  - flux density
  - radiant flux
  - spectral flux density
---
*(Helpful Resource: https://www.cv.nrao.edu/~sransom/web/Ch2.html)*

![[flux.png|align:center|450]]

**Flux** ($F$) is generally defined as a measurable quantity of "something" ($\rd N$) traveling through or moving past a surface or substance ($\rd A$) over some period of time ($\rd t$).

$$
F \propto \frac{\rd N}{\rd A \ \rd t} \hWhere [ \, F \, ] \equiv \fpar{{\rm quantity}}{{\rm area} \times {\rm time}}
$$

For astronomy, we typically use **radiant flux** when observing an astronomical source, making energy or light ($\rd N \equiv \rd E$) the measurable quantity. With this in mind, we can also describe flux as *power per area*; however, we have to be careful on how we express radiant flux in terms of other quantities when comparing to [[Intensity|intensity]].
$$
F \propto \frac{\rd E}{\rd A \ \rd t} \hWhere [ \, F \, ] \equiv \fpar{{\rm energy}}{{\rm area} \times {\rm time}} = \fpar{{\rm power}}{{\rm area}} = MT^{-3}
$$

> [!note] Confusion about the $F$ vs $\rd F$?
> Because we are physicist and not mathematians, we try to use math notation in the most confusing way possible. Here is a great example of that! I don't know if it should be $F$ or $\rd F$, but it may make more sense if you imagine everything as $\Delta X$ vs  $\rd X$?

## Specific Flux
*(Also known as the **flux density**)*

Beginning with the fundamental [[Intensity#Specific Intensity|specific intensity]] relationship...

$$\rd E_{\nu} = I_{\nu} \cos \theta \; \rd A \; \rd \Omega \; \rd \nu \; \rd t$$

...we can rearrange the factors such that we can define the specific flux.

$$
F_{\nu} = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t \, \rd \nu} = \int_{\Omega} I_{\nu} \cos \theta \; \rd \Omega \hWhere [ \, F_{\nu} \, ] \equiv \fpar{{\rm energy}}{{\rm area} \times {\rm time} \times {\rm hertz}} = MT^{-2}
$$

The **specific flux** ($F_\nu$) represents the flux received from a source over some solid angle and defined frequency band from $[\nu,\nu + d\nu]$. *(Since [[Intensity#Specific Intensity|specific intensity]] tends to be the quantity we measure, we define specific flux in terms of $I_{\nu}$ .)*

Our frequency space is usually restricted from our observational equipment; therefore, this quantity becomes is more practical, relative to the [[#Bolometric Flux]] ($F$).

> [!math] Comment on Perpendicular Area & Flux
> In vector calculus, flux is a scalar quantity, defined as the surface integral of the perpendicular component of a vector field over a surface.
> $$
> F = \iint_{S} \mathbf{\vec{V}} \cdot \mathbf{\vec{n}} \; \rd S = \iint_{S} |\mathbf{\vec{V}}| \cos \theta \; \rd S 
> \hWhere 
> \begin{align}
> F &= \text{flux} \\
> \mathbf{\vec{V}} &= \text{quantity vector field} \\
> \mathbf{\vec{n}} &= \text{normal vector to $\rd S$}
> \end{align}
> $$
> In the definition of radiant flux...
> $$F = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t \, \rd \nu}$$
> ...$\rd A$ is **not** the perpendicular area ($\rd A_{\perp} = \rd A \cos \theta$). This is because the definition of the radiant flux comes from the more foundational relationship of [[Intensity#Specific Intensity|specific intensity]] that already includes the $\cos \theta$ factor. Therefore, in this definition, we are instead looking at the **perpendicular component of energy**, such that $\rd E \equiv \rd E_{\perp}$.
> $$F = \int_{\Omega} \frac{\rd E_{\nu, \perp}}{\rd A \, \rd t \, \rd \nu} \hWhere \rd E_{\nu, \perp} \equiv \rd E_{\nu} = I_{\nu} \cos \theta \; \rd A \; \rd \Omega \; \rd \nu \; \rd t$$

> [!measure] Spherically Symmetric Scaling
> Through the conservation of energy (through [[Luminosity]]) between surfaces of two concentric spheres with radii ($r_{1}$, $r_{2}$), we find that flux follows the inverse-square law.
>
> $$
> \begin{align}
> 	L_{1}  = F_{1} \left( 4 \pi r_{1}^{2} \right) &= F_{2} \left( 4 \pi r_{2}^{2} \right) = L_{2} \\
> 	\frac{F_{1}}{F_{2}} &= \left(\frac{r_{2}}{r_{1}} \right)^{2} \hRightarrow F \propto \frac{1}{r^{2}}
> \end{align}
> $$
> 
> ![[Inverse_square_law.svg.png|align:center|400]]
> 
> This shows that **flux is not an intrinsic property** of source since is dependent on parameters of observation.

^fdb0f0

## Bolometric Flux

The **bolometric flux** is the measure of a radiant flux output across all wavelength/frequency bands of light. Relating to the [[#Specific Flux|specific flux]]...
$$F = \int_{0}^{\infty} F_{\nu} \; \rd \nu$$

> [!note] A step further? Not sure if mathematically valid...
> $$
> F = \int_{0}^{\infty} F_{\nu} \; \rd \nu = \int_{0}^{\infty} \int_{\Omega} \fpar{\rd E_{\nu}}{\rd A \, \rd t \, \rd \nu} \; \rd \nu = \int_{\Omega} \int_{0}^{\infty} \fpar{\rd E_{\nu}}{\rd A \, \rd t} \; \frac{\rd \nu}{\rd \nu} = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t}
> $$
> $$\Downarrow$$
> $$
> F = \int_{0}^{\infty} F_{\nu} \; \rd \nu = \int_{\Omega} \frac{\rd E_{\nu}}{\rd A \, \rd t}
> $$
