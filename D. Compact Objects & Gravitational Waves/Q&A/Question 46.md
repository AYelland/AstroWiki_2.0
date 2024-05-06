### Question
---
How does the orbital frequency of the innermost stable circular orbit around a black hole scale with its (i) mass? (ii) spin?

### Answer
---
For a [[Black Hole|black hole]] of mass $M_{\rm BH}$, we can use [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] to calculate the orbital frequency through balancing the gravitational force and the centripetal force at the radius of the [[Black Hole#Innermost Stable Circular Orbit (ISCO)]], using some test mass ($m$).

$$
m (\Omega^{2} R) = \frac{G M m}{R^{2}} \hRightarrow \Omega_{\rm ISCO} = \sqrt{\frac{G M}{R_{\rm ISCO}^{3}}}
$$

The [[Black Hole#Innermost Stable Circular Orbit (ISCO)|ISCO]] radius can be expressed with the $\alpha$ [[Black Hole#Spin|spin-parameter]] such that...

$$R_{\rm{ISCO}} = \alpha \frac{GM}{c^{2}} \hWhere \alpha \equiv \text{spin-parameter}$$

> [!note] About the $\alpha$ Spin-Parameter
> 
> It might seem as though we could rearrange the orbital frequency ($\Omega_{\rm ISCO}$) expression to define the [[Black Hole#Spin|spin-parameter]] $\alpha$; however, the above expression for $R_{\rm ISCO}$ does not come from the force balancing equations. 
> 
> Instead, it originates from solving the Einstein equations with the [[General Relativity#Kerr Metric]] in general relativity. Thus, it has significantly more complex (non-trivial) derivation.
> 
> The resulting limits on $\alpha$ can be related to the primary spin parameter ($a$) such that...
> $$
> a = \cases{
> 	-1 &\text{(retrograde, maximal spin)} \\ 
> 	~~~0 &\text{(Schwarzschild, zero spin)} \\ 
> 	+1 &\text{(prograde, maximal spin)}
> }
> \hRightarrow
> \alpha = \begin{cases}
> 	9 &\text{when } a=-1 \\
> 	6 &\text{when } a=~~~0 \\
> 	1 &\text{when } a=+1
> \end{cases}
> $$
> ...higher $\alpha$ values correlate to lower relative spin values.

Combining the two, we find...

$$\Omega_{\rm ISCO} = \sqrt{\frac{G M (c^{2})^{3}}{(\alpha G M)^{3}}} = \frac{c^{3}}{G M \alpha^{3/2}} \hRightarrow \Omega_{\rm ISCO} \sim \frac{1}{M \alpha^{3/2}}$$

By this relationships, we know:
- As $\alpha$ (and $R_{\rm ISCO}$) increases, the relative spin decreases and $\Omega_{\rm ISCO}$ decreases
	- (*retrograde* is considered "less spin" & *prograde* is considered "more spin")
- As $M$ increases, $\Omega_{\rm ISCO}$ decreases

$$
\boxed{ \; \alpha \uparrow \implies R_{\rm ISCO} \uparrow \implies \text{Relative Spin } \downarrow \implies \Omega_{\rm ISCO} \downarrow \; }
\hspace{2cm}
\boxed{ \; \text{Mass } \uparrow \implies \Omega_{\rm ISCO} \downarrow \; }
$$

