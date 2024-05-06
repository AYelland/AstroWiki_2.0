### Question
---
What is a white dwarf star? Why is the radius of a white dwarf a decreasing function of its mass? What is the basic physics that leads to the upper limit on the mass of a white dwarf (i.e. the Chandrasekhar limit)?

### Answer
---
##### What is a white dwarf star?

![[Stellar Classes#White Dwarf]]

##### Why is the radius of a white dwarf a decreasing function of its mass?

In a [[Stellar Classes#White Dwarf|WD]], there is no mechanism (like nuclear fusion) to support the core from gravitational collapse, outside of the electron [[Degeneracy Pressure|degeneracy pressure]]. The stellar remnant must maintain a balance between the gravitational pressure pushing inward and the [[Degeneracy Pressure#Non-Relativistic|non-relativistic degeneracy pressure]] pushing outward. 

Instead of working with pressure relationships directly, we can make an energy minimization argument, relating the gravitational potential energy (per unit mass)...
$$E_{\rm grav} = - \frac{G M}{R}$$
...to the non-relativistic, degenerate kinetic energy (per unit mass) generated through the motion the electrons.

$$E_{\rm deg} = N_{\rm e} \,\frac{p^{2}}{2 m_{\rm e}} \hWhere [N_{\rm e}] \equiv \frac{\text{\# of electrons}}{\rm mass}$$

Since the matter is degenerate, we can take the momentum ($p$) to be the [[Degeneracy Pressure|Fermi momentum]] ($p_{\rm F}$), defined by the saturated Heisenberg Uncertainty Principle ($\Delta x \; \Delta p \simeq \hbar$).

$$p \equiv p_{\rm F} \sim \left( 3 \pi^{2} \hbar^{3} \bar{n}_{\rm e} \right)^{1/3} \sim \hbar \,\left( \bar{n}_{\rm e} \right)^{1/3} \hWhere \bar{n}_{\rm e} \equiv \text{electron number density}$$

The total number of electrons in the white dwarf can be expressed as $(N_{\rm e} M)$, where the $N_{\rm e}$ quantity is related to the [[Mean Molecular Weight|mean molecular weight]] per electron, $N_{\rm e} \simeq 1 / (\mu_{\rm e} m_{\rm p})$. With the volume of the white dwarf scaling as $V\propto R^{3}$,  the electron number density can be expressed as...

$$\bar{n}_{\rm e} = \frac{N_{\rm e} M}{V} \sim \frac{N_{\rm e} M}{R^{3}}$$

Combining these, this allows us to express the electron [[Degeneracy Pressure|degenerate energy]] as:

$$E_{\rm deg} \simeq N_{\rm e} \,\frac{p_{\rm F}^{2}}{2 m_{\rm e}} \simeq \frac{\hbar^{2} N_{\rm e}}{2 m_{\rm e}} (\bar{n}_{\rm e})^{2/3} \simeq \frac{\hbar^{2}}{2 m_{\rm e}} \fpar{N_{\rm e}^{5/3} \, M^{2/3}}{R^{2}}$$

The limit at which the gravitational energy is balanced with the electron degeneracy energy is then...

$$
E_{\rm grav} + E_{\rm deg} = 0
\hRightarrow 
\frac{G M}{R} \simeq \frac{\hbar^{2}}{2 m_{\rm e}} \fpar{N_{\rm e}^{5/3} \, M^{2/3}}{R^{2}} \hRightarrow \boxed{R \propto M^{-1/3}}
$$

**Therefore as mass is added to the white dwarf, the radius decreases.** Larger masses simply "push more" against the electron degeneracy pressure, which is eventually overcome at the [[Chandrasekhar Limit|Chandrasekhar Mass]] ($\sim 1.4\,M_\odot$). *(see below)*

##### What is the basic physics that leads to the upper limit on the mass of a white dwarf (i.e. the Chandrasekhar limit)?

As the mass of a white dwarf increases, the degeneracy pressure on the electrons (pushing them together and increasing the Fermi level) becomes more and more relativistic. When the velocities of the electrons approach the speed of light, we must then consider the [[Degeneracy Pressure#Ultra-Relativistic|relativistic degeneracy pressure]] instead of the [[Degeneracy Pressure#Non-Relativistic|non-relativistic degeneracy pressure]].

Following the same process as [[Question 52#Why is the radius of a white dwarf a decreasing function of its mass?|before]], we can calculate the *relativistic* limit of the kinetic energy (per unit mass) as...

$$
E_{\rm deg} \simeq N_{\rm e} \, p \, c \hRightarrow E_{\rm deg} \simeq N_{\rm e} \, p_{\rm F} \, c \simeq N_{\rm e} \; \hbar c \; (\bar{n}_{\rm e})^{1/3} \simeq \hbar c \fpar{M^{1/3} N_{\rm e}^{4/3}}{R}
$$

Equating with the gravitational energy, we find $R$ drops out completely. That means that the relativistic limit occurs when the white dwarf reaches the critical mass ($M$) of...

$$
E_{\rm grav} + E_{\rm deg} = 0
\hRightarrow
\begin{aligned}[t]
	\frac{G M_{\rm crit}}{R} &\simeq \hbar c \fpar{M_{\rm crit}^{1/3} N_{\rm e}^{4/3}}{R} \\
	M_{\rm crit} &\simeq N_{\rm e}^{2} \fpar{\hbar c}{G}^{3/2} \\
	M_{\rm crit} &\simeq \fpar{1}{\mu_{\rm e} m_{\rm p}}^{2} \fpar{\hbar c}{G}^{3/2} \approx 1.8 \; {\rm M_{\odot}}
\end{aligned}
$$

To interpret this result, we observe that as we add mass to a white dwarf, its radius will still decrease, and by the Heisenberg Uncertainty Principle, the momentum/velocity of its electrons will increase. As the electron velocity approaches the relativistic limit ($v \to c$), the ultra-relativistic analysis becomes more exact, meaning that the mass of the white dwarf ($M$) must approach this limiting mass ($M_{\rm crit}$) above. As such, no white dwarf can be heavier than this limiting mass.

If we evaluate this limiting/critical mass more rigorous, we find it is closer to  $M_{\rm crit} \sim 1.4 \; {\rm M_{\odot}}$. This is known as the [[Chandrasekhar Limit]].

> [!note] 
> Exact final critical mass depends on initial mass of the white dwarf and its composition.
