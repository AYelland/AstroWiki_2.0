---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - Friedmann
  - FLRW
---

![[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric]]

## Friedmann Equation

### With the Curvature Parameter

If we write down the Einstein field equations for the [[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric|FLRW metric]], we can find an expression for the Hubble parameter, $H(a)$.

$$H(a)^{2} \equiv \left( \frac{\dot{a}}{a} \right)^{2} = \frac{8 \pi G \rho}{3} - \frac{k c^{2}}{a^{2}} +\frac{\Lambda c^{2}}{3}$$


where the following values vary with time.
- $\rho = \rho_{M} + \rho_{r}$ is the volumetric mass density. It is often easier to think of this density in terms of the energy density of matter ($\rho = \epsilon/c^{2}$) including rest energy, thermal energy, radiation energy, etc. 
- $\Lambda$ is the cosmological constant with units $\pu{length^{-2}}$.
- $k$ is the curvature parameter of spacetime.

We can rewrite this expression in a convenient form as...

$$H(a)^{2} = \frac{8 \pi G}{3} \bigg( \rho_{M} + \rho_{r} + \underbrace{\frac{3}{8 \pi G} \frac{-k c^{2}}{a^{2}}}_{\rho_{k}} + \underbrace{\frac{\Lambda c^{2}}{8 \pi G}}_{\rho_{\Lambda}} \; \bigg) = \frac{8 \pi G}{3} \underbrace{\left(\rho_{M} + \rho_{r} + \rho_{k} + \rho_{\Lambda} \right)}_{\equiv \, \rho(a)}$$

### Critical Density

The critical density of the universe $\rho_{\rm c}(z) \equiv \rho_{\rm crit}(z)$ is the mass density at a given cosmological time ($z$) with a flat curvature ($k=0$).
- If $\Lambda \neq 0$ , then the "$\rho$" we refer to in $\rho_c$ is $\rho = \rho_{M} +\rho_{r} + \rho_{\Lambda}$
- If $\Lambda = 0$ , then the "$\rho$" we refer to in $\rho_c$ is $\rho = \rho_{M} +\rho_{r}$

In either case, we express critical density as...

$$\rho_{c}(t) = \frac{3 H(t)^{2}}{8 \pi G} \hspace{2cm} \rho_{c} = \frac{3 H_{0}^{2}}{8 \pi G} \quad \textcolor{gray}{\simeq 10^{-29} \; \pu{g/cm^{3}} \simeq 10^{-26}\;{\rm kg/m^{3}}}$$   
Now, for a given section of space with density $\rho$, we can compare that density to the universe's critical density, $\rho_{c}$. 
- If $\rho > \rho_c$ , that section of space acts like a closed universe; the (mini) universe will eventually stop expanding, and then it will collapse. (see [[Spherical Top Hat Model]])
- If $\rho < \rho_c$ , that section of space acts like an open universe; the (mini) universe will continue expanding forever.

This can be discussed in terms of the parameter $\Omega(t):= \rho(t)/\rho_c(t)$ and whether it is larger or smaller than 1. The time-dependence has been made explicit here because when we don't write it, the implication is that it is evaluated at redshift zero ($z=0$). 

### With the Cosmological Density Parameters...

Using the critical density ($\rho_{c}$), we can now define the **cosmological density parameters**; a set of density ratios comparing the density values of some region in space to the critical density of space at some time ($t$) or redshift ($z$ or $a$).

$$\Omega_{M}(t) = \frac{\rho_{M}(t)}{\rho_{c}(t)} \hspace{1.2cm} 
\Omega_{r}(t) = \frac{\rho_{r}(t)}{\rho_{c}(t)} \hspace{1.2cm} 
\Omega_{k}(t) = \frac{\rho_{k}(t)}{\rho_{c}(t)} \hspace{1.2cm} 
\Omega_{\Lambda}(t) = \frac{\rho_{\Lambda}(t)}{\rho_{c}(t)}$$

$$\Omega(t) = \Omega_{M}(t) + \Omega_{r}(t) + \Omega_{k}(t) + \Omega_{\Lambda}(t) = 1$$

The current day values are evaluated at $z=0$ ($a=1$).

$$\begin{alignat}{3}
	\Omega_{M,0} &= \frac{\rho_{M,0}}{\rho_{c,0}} = \fpar{8 \pi G}{3 H_{0}^{2}} \rho_{M,0} &\hspace{2cm} \Omega_{r,0} &= \frac{\rho_{r,0}}{\rho_{c,0}} = \fpar{8 \pi G}{3 H_{0}^{2}} \rho_{r,0} \\
	\Omega_{k,0} &= \frac{\rho_{k,0}}{\rho_{c,0}} = \frac{- k c^{2}}{H_{0}^{2}} &\hspace{2cm} \Omega_{\Lambda,0} &= \frac{\rho_{\Lambda,0}}{\rho_{c,0}} = \frac{\Lambda c^{2}}{3 H_{0}^{2}}
\end{alignat}$$

$$\Omega_{0} = \Omega_{M,0} + \Omega_{r,0} + \Omega_{k,0} + \Omega_{\Lambda,0} = 1$$

> [!note] 
> When we talk about mean densities of the universe (e.g. [[Question 132]]), we are talking about the **matter** density: $\bar{\rho}(z) = \Omega_{M,0}(1+z)^{3} \rho_{c,0}$, where we write the zeroes explicitly for clarity.

With our definition of the Friedmann equation...

$$H(a)^{2} = \frac{8 \pi G}{3} \bigg( \rho_{M} + \rho_{r} + \underbrace{\frac{3}{8 \pi G} \frac{-k c^{2}}{a^{2}}}_{\rho_{k}} + \underbrace{\frac{\Lambda c^{2}}{8 \pi G}}_{\rho_{\Lambda}} \; \bigg) = \frac{8 \pi G}{3} \underbrace{\left(\rho_{M} + \rho_{r} + \rho_{k} + \rho_{\Lambda} \right)}_{\equiv \, \rho(a)}$$

...we can can compare it to today's values ($z=0$) with the current critical density to re-express the Hubble parameter in terms of these cosmological density parameters. Here, we will define a new function $E(a)$. 

$$E^{2}(a) \equiv \frac{H^{2}(a)}{H_{0}^{2}} = \frac{\rho_{M}(a) + \rho_{r}(a) + \rho_{k}(a) + \rho_{\Lambda}(a)}{\rho_{c,0}} \hWhere H_{0}^{2} = \fpar{8 \pi G}{3} \rho_{c,0}$$
$$E^{2}(a) = \underbrace{\fpar{\rho_{M,0}}{\rho_{c,0}}}_{\Omega_{M,0}} (1+z)^{3} 
+ \underbrace{\fpar{\rho_{r,0}}{\rho_{c,0}}}_{\Omega_{r,0}} (1+z)^{4} 
+ \underbrace{\fpar{\rho_{k,0}}{\rho_{c,0}}}_{\Omega_{k,0}} (1+z)^{2} 
+ \underbrace{\fpar{\rho_{\Lambda,0}}{\rho_{c,0}}}_{\Omega_{\Lambda,0}}$$

$$\boxed{\; \begin{align}
	H^{2}(a) &= H_{0}^{2} E^{2}(a) \\
	E^{2}(a) &= \Omega_{M,0} \, a^{-3} + \Omega_{r,0} \, a^{-4} + \Omega_{k,0} \, a^{-2} + \Omega_{\Lambda,0}
\end{align}}$$
$${\rm or}$$
$$\boxed{\; \begin{align}
	H^{2}(z) &= H_{0}^{2} E^{2}(z) \\
	E^{2}(z) &= \Omega_{M,0} \, (1+z)^{3} + \Omega_{r,0} \, (1+z)^{4} + \Omega_{k,0} \, (1+z)^{2} + \Omega_{\Lambda,0}
\end{align}}$$

> [!note] 
> 
> Regarding the source of the redshifts ($a$ and $z$ factors)...
> 
> - For the mass density ($\rho_{M}$), it comes from the volume contribution ($\text{volume}^{-1} \sim a^{-3} \sim (1+z)^{3}$)
> - For the radiation density ($\rho_{r}$),  it comes from the volume contribution in addition to the redshifting of photons. This gives an extra factor of $a^{-1} \sim (1+z)$. 
> - For the curvature density ($\rho_{k}$) and cosmological constant density ($\rho_{\Lambda}$), it comes directly from the original Friedmann equation.

## Cosmological Evolution

The scale factor $a$ evolves differently over time depending on the "type" of universe (choices of the different $\Omega$) and some common examples are shown in the figure below.

$$H^{2}(a) = H_{0}^{2} \Big( \Omega_{M,0} \, a^{-3} + \Omega_{r,0} \, a^{-4} + \Omega_{k,0} \, a^{-2} + \Omega_{\Lambda,0} \Big) = \fpar{\dot{a}}{a}^{2}$$

![[scale_factor_universe_types.png|align:center|500]]


Different terms in the Friedmann equation dominate at different times.

- **Radiation Regime** - radiation term $\propto a^{-4} \Longrightarrow$ dominates at very early times

$$H^{2} = \fpar{\dot{a}}{a}^{2} \propto a^{-4} \hRightarrow \begin{aligned}[t]
	\dot{a} &\propto a^{-1} \\
	a \; \rd a &\propto \rd t \\
	a &\propto t^{1/2}
\end{aligned}
\hRightarrow 
\begin{aligned}[t]
	&H(t) = \frac{1}{2t} \\
	&t_{0} = \frac{1}{2 H_{0}}
\end{aligned}$$

- **Matter Regime** - matter term $\propto a^{-3} \Longrightarrow$ dominates at early times

$$H^{2} = \fpar{\dot{a}}{a}^{2} \propto a^{-3} \hRightarrow \begin{aligned}[t]
	\dot{a} &\propto a^{-1/2} \\
	\sqrt{a} \; \rd a &\propto \rd t \\
	a &\propto t^{2/3}
\end{aligned}
\hRightarrow 
\begin{aligned}[t]
	&H(t) = \frac{2}{3t} \\
	&t_{0} = \frac{2}{3 H_{0}}
\end{aligned}$$

- **Curvature Regime** - curvature term $\propto a^{-2} \Longrightarrow$ dominates at medium times

$$H^{2} = \fpar{\dot{a}}{a}^{2} \propto a^{-2} \hRightarrow \begin{aligned}[t]
	\dot{a} &\propto {\rm constant} \\
	\rd a &\propto \rd t \\
	a &\propto t
\end{aligned}
\hRightarrow 
\begin{aligned}[t]
	&H(t) = \frac{1}{t} \\
	&t_{0} = \frac{1}{H_{0}}
\end{aligned}$$

- **$\Lambda$ Regime** - $\Lambda$ term $\propto {\rm constant} \Longrightarrow$ dominates at late times

$$H^{2} = \fpar{\dot{a}}{a}^{2} \propto \fpar{\Lambda}{3} \hRightarrow \begin{aligned}[t]
	\dot{a} &\propto a \sqrt{\frac{\Lambda}{3}} \\
	\frac{\rd a}{a} &\propto \sqrt{\frac{\Lambda}{3}} \;\rd t \\
	a &\propto e^{\sqrt{\frac{\Lambda}{3}t}}
\end{aligned}
\hRightarrow 
\begin{aligned}[t]
	&H(t) = \frac{1}{2} \sqrt{\frac{\Lambda}{3 t}} \\
	&t_{0} = \frac{1}{4 H_{0}^{2}} \fpar{\Lambda}{3}
\end{aligned}$$

As the universe evolves, it expands at different rates depending on the regime (radiation/matter/$\Lambda$).

![[scalefactor_time.png|align:center|500]]
