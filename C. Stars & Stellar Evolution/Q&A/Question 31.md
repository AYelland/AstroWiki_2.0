### Question
---
Make a dimensional analysis of the equation of hydrostatic equilibrium using a polytropic equation of state to find a general mass-radius relation for spherically-symmetric, self-gravitating bodies. For which two polytropic indices is the configuration unstable?

### Answer
---
We begin by using [[Stellar Structure#Mass Continuity]], [[Stellar Structure#Hydrostatic Equilibrium]], and the [[Polytropes|Polytrope Equation of State]]... 

$$
\underbrace{\frac{\mathrm{d} M}{\mathrm{d} r} = 4 \pi r^{2} \rho}_{\require{enclose}\enclose{circle}{1}}
\hspace{2cm}
\underbrace{\frac{\mathrm{d} P}{\mathrm{d} r} = - \frac{G M_{r} \rho}{r^{2}}}_{\require{enclose}\enclose{circle}{2}}
\hspace{2cm}
\underbrace{P = K \rho^{\gamma}}_{\require{enclose}\enclose{circle}{3}}
$$

...and doing some loose dimension-matching.

$$\require{enclose}\enclose{circle}{1} \hspace{1cm} \frac{\mathrm{d} M}{\mathrm{d} r} = 4 \pi r^{2} \rho \hspace{1cm} \Rightarrow \hspace{1cm} M_{\rm tot} \; \propto \; R^{3} \, \bar{\rho}$$
$$\require{enclose}\enclose{circle}{2} \hspace{1cm} \frac{\mathrm{d} P}{\mathrm{d} r} = - \frac{G M_{r} \rho}{r^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{P_{\rm c}}{R} \; \propto \; \frac{G M_{\rm tot} \bar{\rho}}{R^{2}}$$
$$\require{enclose}\enclose{circle}{3} \hspace{1cm} P = K \rho^{\gamma} \hspace{1cm} \Rightarrow \hspace{1cm} P_{\rm c} \sim K \bar{\rho}^{\ \gamma} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{P_{\rm c}}{R} \; \propto \; \frac{K \bar{\rho}^{\ \gamma}}{R}$$

Combining $\require{enclose}\enclose{circle}{1}$, $\require{enclose}\enclose{circle}{2}$, and $\require{enclose}\enclose{circle}{3}$...

$$
\frac{P_{\rm c}}{R} \; \propto \; \frac{G M_{\rm tot} \bar{\rho}}{R^{2}} \; \propto \; \frac{K \bar{\rho}^{\ \gamma}}{R} \hspace{1cm} \Rightarrow \hspace{1cm} 
\begin{aligned}[t]
	M_{\rm tot} \; &\propto \; R \, \bar{\rho}^{\ (\gamma-1)} \\
	M_{\rm tot} \; &\propto \; R \, \left(\frac{M_{\rm tot}}{R^{3}}\right)^{\ (\gamma-1)} \\
	M_{\rm tot}^{\ 1 - (\gamma-1)} \; &\propto \; R^{\ -3(\gamma-1)+1} \\
	M_{\rm tot} \; &\propto \; R^{\ (4-3\gamma)/(2-\gamma)}
\end{aligned}
$$
$$\boxed{ \; M_{\rm tot} \; \propto \; R^{\ (4-3\gamma)/(2-\gamma)} \; }$$

The configuration is **unstable** when
- At $\gamma = 2$ the mass scales "infinitely quickly" with $R$
- At $\gamma = \frac{4}{3}$, the mass is independent of $R$
- At $\gamma < \frac{4}{3}$, the mass is directly proportional to radius (should be inversely proportional)

> [!note]- More on stability...
> If we were to "squeeze" the star to perturb the radius ($r' \to r (1 - \varepsilon)$), then the density should be perturbed ($\rho' \to \rho (1-\varepsilon)^{-3} \approx \rho' (1+3\varepsilon)$). The star will remain *stable* in hydrostatic equilibrium if the new outward gas pressure is greater than the new inward gravitational pressure. *(See 8.901 Notes, Lecture 10)*
> $$P'_{\rm gas} \; \propto \; P_{\rm gas} (1 + 3 \varepsilon)^{\gamma}$$
> $$P'_{\rm grav} = \int_{M_{r}}^{M} \frac{\mathrm{d} P}{\mathrm{d} M_{r}} \; \mathrm{d} M_{r} = \int_{M_{r}}^{M} \frac{\mathrm{d} P}{\mathrm{d} r} \frac{\mathrm{d} r}{\mathrm{d} M_{r}} \; \mathrm{d} M_{r} = -\int_{M_{r}}^{M} \frac{G M_{r}}{4 \pi r'^{4}} \; \mathrm{d} M_{r} = P_{\rm grav} (1+4\varepsilon)$$
> $$\Downarrow$$
> $$P'_{\rm grav} = \quad \boxed{P_{\rm grav} (1+4\varepsilon) < P_{\rm gas} (1 + 3 \varepsilon)^{\gamma}} \quad = P'_{\rm gas}$$
> 
> In a similar argument, we can take a more dimensional analysis approach.
> $$P_{\rm gas} \propto \rho^{\gamma} \propto \left(\frac{M}{R^{3}}\right)^{\gamma} \hspace{2cm} P_{\rm HSE} \propto \frac{M \rho}{R} \propto \frac{M^{2}}{R^{4}}$$
> $$\mathrm{d} P_{\rm gas} \propto - R^{(-3\gamma-1)} \; \mathrm{d} R \hspace{2cm} \mathrm{d} P_{\rm HSE} \propto - R^{-5} \; \mathrm{d} R$$
> $$
> \begin{align}
> 	\mathrm{d} P_{\rm gas} &> \mathrm{d} P_{\rm HSE} \\
> 	- R^{(-3\gamma-1)} \; \mathrm{d} R &> - R^{-5} \; \mathrm{d} R \\
> 	R^{-3\gamma} &< R^{-4} \\
> 	R^{\gamma} &> R^{4/3} \\
> 	\gamma \ln R &> \frac{4}{3} \ln R \\
> 	\gamma &> \frac{4}{3}
> \end{align}
> $$
> This is the criteria for the gas pressure to be able to bounce back to equilibrium. Additionally, this is the criteria for the total mass to have a inverse proportionality relationship to radius ($M_{\rm tot} \propto R^{-n}$), which is the desired state. (think of density for justification)

> [!note]
> All of the assumptions made by the question are hidden within the polytropic assumptions or the stellar structure equations.

