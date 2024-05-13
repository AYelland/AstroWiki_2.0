---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
  - polytrope
  - polytropes
  - Polytrope
  - polytropic
---

> [!info] Background Motivation
> 
> The [[Stellar Structure]] equations are complicated, but much of the difficulty comes from the third and fourth ($L$ and $T$).
> 
> If we separate and distinguish the [[Stellar Structure]] equations by **physical structure** ([[Stellar Structure#Mass Continuity]] and [[Stellar Structure#Hydrostatic Equilibrium]]) and **thermal structure** ([[Stellar Structure#Conservation of Energy]] and [[Stellar Structure#Energy Transport]]), then we define a system that may or may not describe a physically realistic thing. In this system, we find that the **physical structure** relationships lack explicit dependence on temperature. 
> 
> We can then introduce temperature dependence through some theoretical equation of state (i.e. $P = P(\rho, T)$); however, if we instead ignored the** thermal structure** relationships by assuming the equation of state is independent of temperature (i.e. $P = P(\rho)$), then we can create a useful approximation that can accurately describe some stellar bodies. This is the model of a polytrope.

**Polytropes** are pseudo-stellar model for an equation of state that assume a power-law relationship between pressure and density.
$$
P = \kappa \rho^{\gamma} = \kappa \rho^{1 + \frac{1}{n}}
\hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}
	\kappa &\equiv \text{constant} \\
	\gamma &\equiv \text{polytropic exponent} = \left( 1 + \tfrac{1}{n} \right) \\
	n &\equiv \text{polytropic index}
\end{aligned}
$$
This model is fully correct for:
- Fully convective stars that move heat via adiabatic transport ($\gamma = \gamma_{\rm ad} = \frac{5}{3}$, $n=\frac{3}{2}$)
- White dwarves (low mass) with a non-relativistic degenerate core ($\gamma = \frac{5}{3}$, $n=\frac{3}{2}$)
- Isothermal ideal gases ($\gamma = 1$, $n=\infty$)

We have the following cases for $n$: 
$$
n = \cases{
	0 &\text{rocky planets} \\
	0-1 &\text{neutron star} \\
	1.5 &\text{non-relativistic degenerate (low mass WD, convective core)} \\
	3 &\text{relativistic degenerate (high mass WD, radiative zone) $\rightarrow$ Sun} \\
	\infty &\text{isothermal sphere}
}
$$

![[eos.png|align:center|400]]

## Lane-Emden Equation

If we define a dimensionless density ($\theta^{\ n}(r)$) with respect to the central density ($\rho_{c} = \rho(r=0)$)...
$$\theta^{\ n} = \frac{\rho}{\rho_{c}} \hspace{1cm} \text{where} \hspace{1cm}\theta^{\ n}(r=0) = 1 \quad , \quad \theta^{\ n}(r=R) = 0$$

...then we can express our polytropic equation of state as:
$$
P = \kappa \rho^{1 + \frac{1}{n}} = \kappa \, \left( \rho_{c} \, \theta^{\ n} \right)^{1 + \frac{1}{n}} = \left( \kappa \, \rho_{c}^{1 + \frac{1}{n}} \right) \, \theta^{\ n + 1} = P_{c} \, \theta^{\ n + 1}
\hspace{1cm} \text{where} \hspace{1cm}
P_{c} = \kappa \, \rho_{c}^{1 + \frac{1}{n}}
$$

By then combining the [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]] and [[Stellar Structure#Mass Continuity|mass continuity]] stellar structure equations through a radius ($r$) derivative, we find that $\theta$ represents a dimensionless temperature and $\theta^{\ n}$ a dimensionless density. The resulting expression is the **Lane-Emden Equation**.

$$
a^{2} \equiv \frac{ (n + 1) P_{c}}{4 \pi G \rho_{c}^{2}} 
\quad , \quad 
\xi \equiv \frac{r}{a}
\hspace{1cm} \Rightarrow \hspace{1cm} 
\frac{1}{\xi^{2}} \frac{\mathrm{d} }{\mathrm{d} \xi} \left( \xi^{2} \frac{\mathrm{d} \theta}{\mathrm{d} \xi} \right) = - \theta^{\ n}
$$

> [!derivation]-
> Beginning this the hydrostatic equilibrium equation, we take the derivative with respect to $r$ to introduce the mass continuity relationship. This will create a relationship representative of a Poisson Equation ($\nabla^{2} \Phi = 4 \pi G \rho$). After introducing our dimensionless variables and central density and pressure expressions, we can perform a few more algebraic steps to find the **Lane-Emden Equation.**
> $$
> \begin{align}
> 	\frac{\mathrm{d} P}{\mathrm{d} r} = - \frac{G M_{r} \rho}{r^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} \hspace{1.4cm} \frac{r^{2}}{\rho} \frac{\mathrm{d} P}{\mathrm{d} r} &= - G M_{r} \\
> 	\frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\rho} \frac{\mathrm{d} P}{\mathrm{d} r} \right) &= - G \frac{\mathrm{d} M_{r}}{\mathrm{d} r} \\
> 	\frac{\mathrm{d} M_{r}}{\mathrm{d} r} = 4 \pi r^{2} \rho \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\rho} \frac{\mathrm{d} P}{\mathrm{d} r} \right) &= - 4 \pi r^{2} \rho G \\
> 	\text{(Poisson Equation with $\Phi = \tfrac{-G M_{r}}{r}$)} \hspace{1cm} \frac{1}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\rho} \frac{\mathrm{d} P}{\mathrm{d} r} \right) &= - 4 \pi \rho G \\
> 	\frac{1}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\rho_{c} \theta^{\ n}} \frac{\mathrm{d} (P_{c} \theta^{\ n+1})}{\mathrm{d} r} \right) &= - 4 \pi G \rho_{c} \theta^{\ n} \\
> 	\left[ \frac{P_{c}}{4 \pi G \rho_{c}^{2}} \right] \;  \frac{1}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\theta^{\ n}} \frac{\mathrm{d} (\theta^{\ n+1})}{\mathrm{d} r} \right) &= -\theta^{\ n} \\
> 	\left[ \frac{P_{c}}{4 \pi G \rho_{c}^{2}} \right] \;  \frac{1}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{r^{2}}{\theta^{\ n}} \left( (n+1) \;  \theta^{n} \frac{\mathrm{d} \theta}{\mathrm{d} r} \right) \right) &= -\theta^{\ n} \\
> 	\underbrace{\left[ \frac{(n+1)P_{c}}{4 \pi G \rho_{c}^{2}} \right]}_{= a^{2}} \;  \frac{1}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( r^{2} \frac{\mathrm{d} \theta}{\mathrm{d} r} \right) &= -\theta^{\ n} \\
> 	\frac{a^{2}}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( r^{2} \frac{\mathrm{d} \theta}{\mathrm{d} r} \right) &= -\theta^{\ n} \\
> 	\xi = \frac{r}{a} \hspace{1cm} \Rightarrow \hspace{1cm} \hspace{1cm} \frac{a^{2}}{r^{2}} \frac{\mathrm{d} }{\mathrm{d} (r/a)} \left( \left(\frac{r}{a}\right)^{2} \frac{\mathrm{d} \theta}{\mathrm{d} (r/a)} \right) &= -\theta^{\ n} \\
> 	\frac{1}{\xi^{2}} \frac{\mathrm{d} }{\mathrm{d} r} \left( \xi^{2} \frac{\mathrm{d} \theta}{\mathrm{d} \xi} \right) &= -\theta^{\ n}
> \end{align}
> $$

The solutions to this equation ($\theta$) define the complete mass, radius, density and pressure profiles of a polytropic star. Analytical solutions exist for $(n = 0, 1, 5)$, and solutions have finite mass for $(n \le 5)$.

**Boundary Conditions:**
Assuming we determine $\xi_{\rm surf}$ from the solution of the Lane-Emden Equation.
$$
\theta(\xi=0) = 1
\hspace{2cm}
\theta(\xi_{\rm surf}) = 0
\hspace{2cm}
\left. \frac{\mathrm{d} \theta}{\mathrm{d} \xi} \right|_{\xi=0} = 0
$$
 