### Question
---
Explain the steps that you would take to show that both the orbital period and the total energy of a Keplerian orbit depend only on the semi-major axis, and not on the orbital eccentricity.

### Answer
---
*For more detailed derivations, see [[Kepler's Laws of Planetary Motion]]*.

**For the Total Energy ($E$):**

- Total energy of the Keplerian Orbit: $$E = T + U = \left( \frac{1}{2} \mu \dot{r}^{2} + \frac{L^{2}}{2 \mu r^{2}} \right) + \left(- \frac{G M \mu}{r} \right)$$
- Since the energy is conserved, we evaluate the energy at a specific point on the orbit. by convention, we use the pericenter *(position of minimum distance between the two bodies)*. $$r(\phi=0) = a (1-\varepsilon) \hspace{1cm} \Rightarrow \hspace{1cm} \dot{r} = 0$$ $$E = \frac{L^{2}}{2 \mu r^{2}} - \frac{G M \mu}{r} = \frac{L^{2}}{2 \mu a^{2} (1 - \varepsilon^{2})^{2}} - \frac{G M \mu}{a (1 - \varepsilon^{2})}$$
- We then apply one of the results from [[Kepler's Laws of Planetary Motion#Kepler's 1st Law]]. $$a (1 - \varepsilon^{2}) = \frac{L^{2}}{\mu k} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{E = - \frac{k}{2 a} = - \frac{G M \mu}{2a}}$$

**For the Orbital Period ($P$):**

We compare the general area of ellipse ($A = \pi a b$) and the constant rate of change of the area ($\frac{\mathrm{d} A}{\mathrm{d} t}$). Similar to before, we have to apply the same result from [[Kepler's Laws of Planetary Motion#Kepler's 1st Law]] 
$$
\begin{align}
	\pi a b &= \int_{0}^{P} \left( \frac{\mathrm{d} A}{\mathrm{d} t} \right) \; \mathrm{d} t
		\hspace{1.4cm}
		\textcolor{gray}{\left[ b = a \sqrt{1 - \varepsilon^{2}} \right]} \\
	\pi a^{2} \sqrt{1 - \varepsilon^{2}} &= \int_{0}^{P} \left( \frac{L}{2 \mu} \right) \; \mathrm{d} t \\
	\pi a^{2}\sqrt{1 - \varepsilon^{2}} &= \left(\frac{L}{2 \mu}\right) \int_{0}^{P} \mathrm{d} t 
		\hspace{1.5cm}
		\textcolor{gray}{\left[ a (1 - \varepsilon^{2}) = \frac{L^{2}}{k \mu} = \frac{L^{2}}{G M \mu^{2}} \right]} \\
	\\
	\pi a^{2}\sqrt{1 - \varepsilon^{2}} &= \frac{P}{2} \sqrt{G M a (1 - \varepsilon^{2})} \\
	\\
	P^{2} &= \frac{4 \pi^{2} a^{3}}{G M} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{ \;P^{2} \propto a^{3} \;}
\end{align}
$$
*(This is just the proof of [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]].)*

