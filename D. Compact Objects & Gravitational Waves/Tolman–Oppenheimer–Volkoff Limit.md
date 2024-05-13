---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - TOV limit
---
The **Tolman–Oppenheimer–Volkoff (TOV) Equation** is the relativistic hydrostatic equilibrium equation that is used to place an upper mass limit on a [[Neutron Star|neutron star]]. 

$$\frac{\mathrm{d} P}{\mathrm{d} r} = - \frac{G \left[ M(r) + 4 \pi r^{3} P(r) / c^{2} \right] \left[ \rho(r) + P(r) / c^{2} \right]}{r^{2} \left[ 1 - 2 G M(r) / r c^{2} \right]}$$

*(Analogous to the [[Chandrasekhar Limit]] for the maximum mass of a stable [[Stellar Classes#White Dwarf|white dwarf star]].)*

> [!math]- Using the Chandrasekhar Limit...
> 
> If we use the [[Chandrasekhar Limit]], the limit is constructed through balancing gravitational pressure with [[Degeneracy Pressure|degeneracy pressure]] to avoid [[Core-Collapse|core-collapse]]. But, instead of being supported with *electron* degeneracy pressure, it is supported by *neutron* degeneracy pressure.
> 
> If we use the same argument we derived in [[Question 52]], then we find...
> 
> $$
> E_{\rm grav} + E_{\rm deg} = 0
> \hspace{1cm} \Rightarrow \hspace{1cm}
> M_{\rm crit} \simeq \left(\frac{1}{\mu_{\rm n} m_{\rm p}}\right)^{2} \left(\frac{\hbar c}{G}\right)^{3/2} \approx 5.8 \; {\rm M_{\odot}}
> $$
> 
> ...but this neglects general relativity instabilities that dominate at lower masses.

**Currently, there is not an *accurate* constraint on this limit.** This is because...
- The equations of state for extremely dense matter are not well known.
	- For electron degeneracy, we use the Fermi-Dirac statistics, which tacitly assumes that the particles are non-interacting. This is not bad an assumption for the electron gas inside a white dwarf, but in a neutron star, the density is similar to the density inside an atomic nucleus. (Meaning, the neighboring neutrons interact with each other through nuclear forces and it is no longer justified to treat them as non-interacting particles). 
- Higher rotation rates allow for larger masses.
- The strong repulsive nuclear force plays a bigger role than for white dwarfs
- [Causality](https://arxiv.org/pdf/gr-qc/0703121.pdf) must be satisfied
	- The speed of sound (how the NS responds to perturbations) cannot exceed the speed of light

|  Year  | Mass Limit Approx. Ranges                         | Notes                                        |
| :----: | :------------------------------------------------ | -------------------------------------------- |
| $1939$ | $M_{\rm TOV} \sim 0.7 \; {\rm M_{\odot}}$         | Original calculation.                        |
| $1974$ | $M_{\rm TOV} \sim 3.2 \; {\rm M_{\odot}}$         | "Maximally Stiff" EoS (incompressible fluid) |
| $1996$ | $M_{\rm TOV} \sim 1.5 - 3.0 \; {\rm M_{\odot}}$   |                                              |
| $1996$ | $M_{\rm TOV} \sim 2.2 - 2.9 \; {\rm M_{\odot}}$   |                                              |
| $2017$ | $M_{\rm TOV} \sim 2.01 - 2.17 \; {\rm M_{\odot}}$ | From the GW170817 observation.               |

Today, the limit is generally held to be around $2.1\,M_\odot$, but a recent estimate puts the upper limit at $2.16\,M_\odot$. The maximum observed mass of neutron stars is about $2.14\,M_\odot$ for PSR J0740+6620 discovered in September, 2019.

$$M \lesssim M_{\rm TOV} \simeq 2.16 \; {\rm M_{\odot}}$$

In the case of a rigidly spinning neutron star, the mass limit is thought to increase by up to $18 - 20 \%$.

> [!extra]- From 8.901, Problem Set 10
> 
> If we model a neutron star as a nearly incompressible fluid with constant density ($\rho_{0}$), the relativistic version of the equation of hydrostatic equilibrium is...
> 
> $$\frac{\mathrm{d} P}{\mathrm{d} r} = - \frac{G \left[ M(r) + 4 \pi r^{3} P(r) / c^{2} \right] \left[ \rho(r) + P(r) / c^{2} \right]}{r^{2} \left[ 1 - 2 G M(r) / r c^{2} \right]}$$
> 
> If we solve this equation for neutron star with constant mass ($M$) and radius ($R$), and [[Black Hole#Event Horizon|Schwarzschild radius]] ($R_{\rm S} \equiv 2 G M / c^{2}$), we can integrate the TOV to express the pressure as...
> 
> $$P(r) = \rho_{0} c^{2} \left(\frac{\sqrt{1 - (R_{\rm S} / R)} - \sqrt{1 - (R_{\rm S} \,r^{2} / R^{3})}}{3 \sqrt{1 - (R_{\rm S} / R)} - \sqrt{1 - (R_{\rm S} \,r^{2} / R^{3})}}\right)$$
> 
> > [!derivation]-
> > 
> > With the constant density, our mass can be expressed as...
> > $$M(r) = \int_{0}^{r} \rho_{0} (4 \pi r'^{\ 2}) \; \mathrm{d} r' = \left(\frac{4 \pi r^{3}}{3}\right) \rho_{0}$$
> > $$\Downarrow$$
> > $$\frac{\mathrm{d} P}{\mathrm{d} r} = - G \left(\frac{ 4 \pi r^{3} \left[ \rho_{0}/3 + P / c^{2} \right] \left[ \rho_{0} + P / c^{2} \right]}{r^{2} \left[ 1 - 8 \pi G \rho_{0} r^{2} / 3 c^{2} \right]}\right)$$
> > 
> > Non-dimensionalizing with the variables...
> > 
> > $$u \equiv \frac{P}{\rho_{0} c^{2}} \hspace{3cm} \xi \equiv r \sqrt{\frac{4 \pi G \rho_{0}}{3 c^{2}}} = r \sqrt{\frac{G M}{R^{3} c^{2}}}$$
> > 
> > ...our differential equation becomes...
> > 
> > $$
> > \frac{\mathrm{d} u}{\mathrm{d} \xi} = - \frac{ \xi (1 + 3 u) (1+u)}{(1 - 2\xi^{2})}
> > \hspace{1cm} \Rightarrow \hspace{1cm}
> > \begin{aligned}[t]
> > 	\int_{u(\xi)}^{0} \frac{\mathrm{d} u}{(1+3u)(1+u)} &= - \int_{\xi}^{\xi_{\rm m}} \frac{\xi \; \mathrm{d} \xi}{(1 - 2 \xi^{2})} \\
> > 	\\
> > 	\frac{1}{2} \ln \left(\frac{1 + u(\xi)}{1+3u(\xi)}\right) &= - \frac{1}{4} \ln  \left(\frac{1 - 2 \xi_{\rm m}^{2}}{1 - 2 \xi^{2}}\right) \\
> > 	\\
> > 	&\hspace{-3cm} u(\xi) = \frac{\sqrt{1 - 2 \xi^{2}} - \sqrt{1 - 2 \xi_{\rm m}^{2}}}{3\sqrt{1 - 2 \xi_{\rm m}^{2}} - \sqrt{1 - 2 \xi^{2}}} \\
> > \end{aligned}
> > $$
> > 
> > ...where we integrate from some point ($r$) to the surface ($r = R$). In the dimensionless units, the surface is at $\xi = \xi_{\rm m}$ where $\xi_{\rm m}^{2} = G M / R c^{2} = R_{\rm S} / 2 R$.  Re-dimensionalizing the expression, we can express the 
> > 
> > $$P(r) = \rho_{0} c^{2} \left(\frac{\sqrt{1 - (R_{\rm S} / R)} - \sqrt{1 - (R_{\rm S} \,r^{2} / R^{3})}}{3 \sqrt{1 - (R_{\rm S} / R)} - \sqrt{1 - (R_{\rm S} \,r^{2} / R^{3})}}\right)$$
> 
> In order for the pressure in the center of the neutron star ($r=0)$ to remain finite and not collapse into a singularity, the denominator must be non-zero. Furthermore, to connect this relativistic relationship to the non-relativistic counterpart, the denominator must be positive. Therefore, evaluating at $r=0$ where the pressure is the highest...
> 
> $$3 \sqrt{1 - (R_{\rm S} / R)} - \sqrt{1 - (R_{\rm S} \,r^{2} / R^{3})} > 0 \hspace{1cm} \Rightarrow \hspace{1cm} R > \frac{9}{8} R_{\rm S} = \frac{9 G M}{4 c^{2}}$$
> 
> ...we can construct a lower limit on the radius of the neutron star. This, with the constant density, can give us a constraint on the mass as well.
> 
> $$
> R = \left(\frac{M}{\frac{4}{3} \pi \rho_{0}}\right)^{1/3} > \left(\frac{9 G M}{4 c^{2}}\right)
> \hspace{1cm} \Rightarrow \hspace{1cm}
> \boxed{\; M \lesssim M_{\rm TOV} = \left(\frac{4 c^{2}}{9 \sqrt{3 \pi G^{3} \rho_{0}}}\right) \;}
> $$
