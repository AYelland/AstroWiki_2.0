---
banner: "![[galaxies.jpg]]"
banner_y: 0.35
aliases:
---
## Summary Table

| Name                                                          | Form                                                                                                                                                     | Use                                                                                                                                                                                                                                                                                                       |
| ------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [[#Sersic Profile\|Sérsic]]                                   | $$I(r) = I_{0} \, e^{-(r/r_{\rm s})^{1/n}}$$                                                                                                             | Models the [[Intensity\|surface brightness/intensity]] profiles of galaxies. $I_0$ is central surface brightness, $r_{\rm s}$ is scale length and $n$ is the "Sersic index".                                                                                                                              |
| [[#Exponential Profile\|Exponential]]                         | $$I(r) = I_{0} \, e^{-(r/r_{\rm s})}$$                                                                                                                   | Models the [[Intensity\|surface brightness/intensity]] profiles of [[Galaxy Classification#Disk Galaxy\|disk galaxies]] and [[Galaxy Classification#Spiral Galaxy\|spiral galaxies]]. (Sersic with $n=1$)                                                                                                 |
| <nobr>[[#de Vaucouleurs Profil\|de Vaucouleurs]]</nobr>       | $$I(r) = I_{0} \, e^{-(r/r_{\rm s})^{1/4}}$$                                                                                                             | Model the [[Intensity\|surface brightness/intensity]] profiles of [[Galaxy Classification#Elliptical Galaxy\|elliptical galaxies]] and [[Anatomy of a Galaxy#Galactic Bulge\|galactic bulges]]. (Sersic with $n=4$)                                                                                       |
| $\alpha\beta\gamma$ [[#$ alpha beta gamma$ Profile\|Profile]] | $$\rho(r) = \rho_{0} \left[\fpar{r}{r_{\rm s}}^{\gamma} \left( 1 + \fpar{r}{r_{\rm s}}^{\alpha} \right)^{\frac{(\beta - \gamma)}{\alpha}} \right]^{-1}$$ | Density profile for DM halos in [[Dark Matter\|CDM]]. Generalized family of NFW-like profiles.                                                                                                                                                                                                            |
| [[#Navarro-Frenk-White Profile\|NFW]]                         | $$\rho(r)= \rho_{0} \left[ \frac{r}{r_{\rm s}}\left( 1 + \frac{r}{r_{\rm s}} \right)^{2} \right]^{-1}$$                                                  | Density profile for DM halos in [[Dark Matter\|CDM]]. Exhibits a divergent central density and doesn't have a well-defined total mass. Originates from N-body simulations with a cuspy central region shape, giving rise to core/cusp problem when comparing to observational data (see [[Question 125]]) |
| [[#Einasto Profile\|Einasto]]                                 | $$\rho(r) = \rho_{\rm s} \, \exp \left[-\frac{2}{\alpha}\left(\frac{r}{r_{\rm s}}\right)^{\alpha} \right]$$                                              | Density profile for DM halos in [[Dark Matter\|CDM]]. Does not exhibit a divergent central density. People define in different ways, $r_s$ is a scale radius. [Source](https://cluster-toolkit.readthedocs.io/en/latest/source/density_profiles.html)                                                     |


## Surface Brightness Profiles
### Sersic Profile

$$I(r) = I_{0} \, e^{-(r/r_{\rm s})^{1/n}} \hWhere
\begin{aligned}
	I_{0} &\equiv \text{central intensity} \\
	r_{\rm s} &\equiv \text{scale length} \\
	n &\equiv \text{Sérsic Index} \\
\end{aligned}$$

Used to describe and model the [[Intensity|surface brightness/intensity]] profiles of galaxies. The variable ($n$) allows the profile to be applied to a larger variety of galaxy types.
- For $n=1$, we recover the [[#Exponential Profile]] - appropriate for [[Galaxy Classification#Disk Galaxy|disk galaxies]] and [[Galaxy Classification#Spiral Galaxy|spiral galaxies]].
- For $n=4$, we recover the [[#de Vaucouleurs Profile]] - appropriate for [[Galaxy Classification#Elliptical Galaxy|elliptical galaxies]] and [[Anatomy of a Galaxy#Galactic Bulge|galactic bulges]].

> [!note] Another Formulation
> In terms of "half-light"...
> $$I(r) = I_{\rm e} \exp \left[ -b_{n} \left( \fpar{R}{R_{\rm e}}^{1/n} - 1 \right) \right]$$

### Exponential Profile

$$I(r) = I_{0} \, e^{-(r/r_{\rm s})} \hspace{1.5cm} \text{Sersic Index:} \; n=1$$

Used to describe and model the [[Intensity|surface brightness/intensity]] profiles of [[Galaxy Classification#Disk Galaxy|disk galaxies]] and [[Galaxy Classification#Spiral Galaxy|spiral galaxies]]. *(same as [[#Sersic Profile]] with $n=1$)*

### de Vaucouleurs Profile

$$I(r) = I_{0} \, e^{-(r/r_{\rm s})^{1/4}} \hspace{1.5cm} \text{Sersic Index:} \; n=4$$

Used to describe and model the [[Intensity|surface brightness/intensity]] profiles of [[Galaxy Classification#Elliptical Galaxy|elliptical galaxies]] and [[Anatomy of a Galaxy#Galactic Bulge|galactic bulges]]. *(same as [[#Sersic Profile]] with $n=4$)*

## DM Halo Density Profiles

![[DMhalo_profiles.png|align:center|500]]

### $\alpha\beta\gamma$  Profile
*(Also known as the **The "Generalized" NFW Profile**)*

$$\rho(r) = \rho_{0} \left[\fpar{r}{r_{\rm s}}^{\gamma} \left( 1 + \fpar{r}{r_{\rm s}}^{\alpha} \right)^{(\beta - \gamma)/\alpha} \right]^{-1} \hWhere \begin{aligned}
	\rho_{0} &\equiv \text{central density} \\
	r_{\rm s} &\equiv \text{scale radius}
\end{aligned}$$

The $\alpha\beta\gamma$ profile is a generalization of the [[#Navarro-Frenk-White Profile]] with different free parameters, yielding a double power-law density profile.
- At small radii: $\rho \propto r^{-\gamma}$
- At large radii: $\rho \propto r^{-\beta}$

![[alphabetagamma_profile.png|align:center|500]]

#### Navarro-Frenk-White Profile

$$\rho(r) = \rho_{0} \left[ \frac{r}{r_{\rm s}}\left( 1 + \frac{r}{r_{\rm s}} \right)^{2} \right]^{-1} = \rho_{0} \left[ c \, \left( 1 + c \right)^{2} \right]^{-1} \hWhere \begin{aligned}
	\rho_{0} &\equiv \text{central density} \\
	r_{\rm s} &\equiv \text{scale radius} \\
	c &\equiv \text{concentration of halo}
\end{aligned}$$

Used to describe and model [[Dark Matter#CDM]] density profiles. This is an empirical model developed over a series of papers in the 90’s through N-Body simulations of [[Dark Matter#CDM]] halos.

- Showed the mass density ($\rho_{0}$) and scale radii ($r_{\rm s}$), are strongly correlated for [[Dark Matter#CDM]] halos, such halos are approximately members of a $1$-parameter family.
- A conventional choice for this parameter is $r = r_{200}$, the [[Virial Theorem|Virial Radius]] (the distance that encloses a 200 times the cosmic critical density ($\rho_{c}$) of the universe). In terms of the [[Virial Theorem|Virial Mass]] and the present day critical density: $$M_{200} = 200 \cdot \left( \frac{4}{3} \pi r_{200}^{3} \right) \cdot \rho_{c} \hWhere \rho_{\rm c, 0} = \frac{3 H_{0}^{2}}{8 \pi G} \approx 1.8 \times 10^{-29} h^{2} \; {\rm g/cm}$$

**Properties:**
 - Exhibits a divergent central density: $\rho \propto r^{-1}$ as $r \to 0$
 - Total mass not bound or well-defined: $\rho \propto r^{-3}$ as $r \to \infty$

**Related Topics:**
- Core-Cusp Problem: *(see [[Question 125]])*
	From observations of stellar dynamics, the inner profile of DM halos are more core-like, flattening to a constant slope $\sim 0$ ($r \to r^{0} \sim {\rm constant}$). The NFW overpredicts the central density such that it it more "cuspy", with a slope of $\sim -1$ ($r \to r^{-1}$). This is possibly due to stellar core formation leading to supernova feedback, but it could also be resolved through modifications of cold dark matter. Specifically, self-interacting dark matter (SIDM) could lead to core formation.

- Missing Satellite Problem: *(see [[Question 125]])*
	Simulations produce more satellite halos than there are observed satellite galaxies.  It's possible that not all subhalos form stars, so we need to be able to find "dark subhalos."  This could be done by looking for disruptions in stellar streams or through gravitational lensing.
	
#### Generalized NFW Profile

After finding strong degeneracies between these parameters, $\alpha$ and $\beta$ are fixed such that...

$$\begin{aligned}
	\alpha &= 1 \\
	\beta &= 3
\end{aligned}
\hRightarrow 
\rho(r) = \rho_{0} \left[\fpar{r}{r_{\rm s}}^{\gamma} \left( 1 + \frac{r}{r_{\rm s}} \right)^{(3 - \gamma)} \right]^{-1}$$

...the free parameter $\gamma$ can describe a cored ($\gamma=0$) or cusped ($\gamma=1$) density profile.

#### Pseudo-Isothermal Profile
*(Also known as **Perfect Sphere** profile in table above)*

$$\begin{aligned}
	\alpha &= 2 \\
	\beta &= 4 \\
	\gamma &= 0
\end{aligned}
\hRightarrow 
\rho(r) = \rho_{0} \left[ 1 + \fpar{r}{r_{\rm s}}^{2} \right]^{-1}$$

This profile provides a good fit to most rotation curve data; however, it cannot be a complete description
- The enclosed mass fails to converge to a finite value as the radius tends to infinity. 
- Collapse may never reach an equilibrium state in the outer region of a dark matter halo.
- Does not account for non-radial motion that could be important.
- Mergers associated with the (hierarchical) formation of a halo may render the spherical-collapse model invalid.

### Einasto Profile

$$\td{\ln \rho(r)}{\ln r} = -2 \fpar{r}{r_{-2}}^{\alpha}\hRightarrow \rho(r) = \rho_{\rm s} \, \exp \left[-\frac{2}{\alpha}\left(\frac{r}{r_{\rm s}}\right)^{\alpha} \right]$$
where 
- $r_{\rm s}$ and $\rho_{\rm s}$ are taken to be the scale radius and associated density $\rho_{\rm s} = \rho(r_{\rm s})$. These scale values are often taken a different values, but sometimes quotes as...
	- $r_{−2}$ is the radius at which the logarithmic slope of the density distribution is equal to −2
	- $\rho_{−2}$ is the density are the $r=r_{-2}$ radius $\implies \rho_{-2} = \rho(r_{−2})$
- $\alpha$ profile index (best-fit values: $0.12 \lesssim \alpha \lesssim 0.25$ , increase systematically with mass)

Used to describe and model [[Dark Matter#CDM]] density profiles. Unlike the [[#Navarro-Frenk-White Profile]], this model does not have a divergent central density. It is primarily described by its power-law fit to the logarithmic slope of the density profile (left equation above),

https://cluster-toolkit.readthedocs.io/en/latest/source/density_profiles.html

## Isothermal Sphere

[Helpful Source for Derivation](https://courses.physics.ucsd.edu/2019/Winter/physics141/Lectures/Lecture7/lecture7.pdf)

> [!note] 
> Potential-Density pairs are related via Poisson's Equation. In a spherically symmetric system, this reduces to:
> $$\nabla^{2} \Phi(\vec{r}) = 4 \pi G \rho(\vec{r}) \hRightarrow \frac{1}{r^{2}} \td{}{r} \left[ r^{2} \td{\Phi}{r} \right] = \frac{1}{r} \tdd{}{r} \bigg[ r \Phi \bigg] = 4 \pi G \rho(r)$$

For a self-gravitating isothermal gas sphere ($T = \text{const}$), we will utilize [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]] and [[Stellar Structure#Mass Continuity|mass continuity]] to express the density profile ($\rho(r)$) in terms of the velocity dispersion ($\sigma$), assuming that the density profile follows the power law:  $\rho(r) = \rho_{0} r^{-\alpha}$. 

1. [[Stellar Structure#Hydrostatic Equilibrium]] + [[Thermodynamics#Ideal Gas Law]]
   Beginning with hydrostatic equilibrium, we will assume that the ideal gas law holds, such that $P= n k_{\rm B} T = k_{\rm B} T (\rho/m)$ , where $m \equiv$ mean particle mass. 
   $$\td{P}{r} = -\frac{G M_{r} \rho}{r^{2}} \hRightarrow \td{\rho}{r} = -\fpar{G M_{r} m}{k_{\rm B} T} \frac{\rho}{r^{2}}$$
   We also will assume the velocity in the system is given by the [[Velocity Dispersion|velocity dispersion]] $\sigma$, such that by equating the thermal energy and kinetic energies...
   $$m \sigma^{2} \propto k_{\rm B} T \hRightarrow \td{\rho}{r} = -\frac{GM_r}{\sigma^2}\frac{\rho}{r^2}$$
   This is the differential equation a density profile must satisfy for a self-gravitating ideal gas with constant temperature in hydrostatic equilibrium. This can be rewritten as
   $$r^2 \frac{d\ln\rho}{dr} = -\frac{GM_r}{\sigma^2}$$
   
1. [[Stellar Structure#Mass Continuity]]
   Differentiating the equation above with respect to ($r$) and applying mass continuity... 
   $$\td{}{r} \left[ r^{2} \td{\ln \rho}{r} \right] = -\frac{G}{\sigma^{2}} \td{M_{r}}{r} = -\frac{G}{\sigma^{2}} \left( 4 \pi r^{2} \rho \right) \textcolor{gray}{\hWhere \left[ \; \td{M_{r}}{r} = 4 \pi r^{2} \rho \; \right]}$$
   
3. Power-Law Density Profile (Anstaz)
   We now make the assumption that the density profile will follow a power-law in radius. 
   $$\rho(r) = \rho_{0} r^{-\alpha}$$
   This is motivated by the known solutions of the Laplacian Equation (homogeneous Poisson Equation). There could also be some correlation with the [[Polytropes|polytropic EoS]] and the [[Polytropes#Lane-Emden Equation]] as well, given they source from similar assumptions.
   
   From this, our differential equation becomes:
   $$\begin{align}
	   \td{}{r} \left[ r^{2} \td{\ln \rho}{r} \right] &= -\frac{G}{\sigma^{2}} \left( 4 \pi r^{2} \rho \right) \\
	   \frac{1}{r^{2}} \td{}{r} \left[ r^{2} \td{\ln \rho}{r} \right] &= -\fpar{4 \pi G}{\sigma^{2}} \rho \\
	   \frac{1}{r^{2}} \td{}{r} \left[ r^{2} \td{\ln \left( \rho_{0} r^{-\alpha} \right)}{r} \right] &= -\fpar{4 \pi G}{\sigma^{2}} \left( \rho_{0} r^{-\alpha} \right) \\
	   \frac{1}{r^{2}} \td{}{r} \left[ r^{2} \fpar{- \alpha \rho_{0} r^{-\alpha-1}}{\rho_{0} r^{-\alpha}} \right] &= -\fpar{4 \pi G \rho_{0}}{\sigma^{2}} \,r^{-\alpha} \\
	   \frac{1}{r^{2}} \td{}{r} \left[ - \alpha r \right] &= -\fpar{4 \pi G \rho_{0}}{\sigma^{2}} \,r^{-\alpha} \\
	   - \frac{\alpha}{r^{2}}  &= -\fpar{4 \pi G \rho_{0}}{\sigma^{2}} \,r^{-\alpha} \hRightarrow \alpha = 2
   \end{align}$$
   By matching powers of $r$, we find that $\alpha = 2$. Thus, the central density of the isothermal sphere is defined, and the density profile is in terms of the velocity dispersion.
   $$\rho_{0} = \frac{\alpha \sigma^{2}}{4 \pi G} = \frac{\sigma^{2}}{2 \pi G} \hRightarrow \boxed{ \; \rho(r) = \rho_{0} r^{-2} = \frac{\sigma^{2}}{2 \pi r^{2} G} \;}$$

