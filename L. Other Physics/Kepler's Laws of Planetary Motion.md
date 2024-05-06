---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
  - Kepler's Laws
  - Kepler Problem
---

> [!key-idea]
> Kepler's Law's of Planetary Motion are:
> 1) Bound motion of two body systems move in elliptical orbits. $$r(\phi) = \frac{a \, (1 - \varepsilon^{2})}{1 + \varepsilon \cos \phi} \hspace{1.5cm} a (1 - \varepsilon^{2}) = \frac{L^{2}}{\mu k} \hspace{1.5cm} \varepsilon = \sqrt{1 + \frac{2 E L^{2}}{\mu^{2} k^{2}}}$$
> 2) The radius vector of the orbiting body sweeps out equal areas during equal intervals of time. $$\td{A}{t} = \frac{L}{2 \mu} \hWhere L = \mu r^{2} \dot{\phi}$$
> 3) Period-Radius Relationship: $$P^{2} \propto a^{3}$$

## Parameters for Orbits
*(https://en.wikipedia.org/wiki/Orbital_elements)*

For bodies bound in an orbit, they are constrained to a mutual plane ($xy$-plane) with a shared angular momentum ($z$-direction). We can describe their motion through elliptical orbits and Euler Angles $(\Omega \, , \, i \, , \, \omega) \equiv (\alpha \, , \, \beta \, , \, \gamma)$ from a fixed observational plane ($XY$-plane). The following parameters with simplify these orbital systems such that they solvable.

- Shape of the Orbit
	- $a \equiv$ semi-major axis
	- $\varepsilon \equiv$ eccentricity
	- $b \equiv$ semi-minor axis $=a\sqrt{1 - \varepsilon^{2}}$

- Orientation of the Orbit (Euler Angles)
	- $i \equiv$ inclination angle (see [[Mnemonics#Inclination Angle|mnemonic]])
	- $\Omega \equiv$ longitude of ascending node
	- $\omega \equiv$ argument/longitude of periapse
	
- Time Position
	- $T \equiv$ time of reference, usually periapse
	- $P \equiv$ period of orbit

- $\phi(t) \equiv$ true anomaly - physical angle from periaspe of the object from center of mass
- $\Psi(t) \equiv$ eccentric anomaly - handy variable that lets us get time dependence
- $\omega t \equiv$ mean anomaly - convenient but fictional angle that varies linearly with time


**General Elliptical Orbit**

![[ellipse.png|align:center]]


**Euler Angles**

![[eulerAngles_orbit.png|aling:center|500]]


> [!note] Another definition of Euler Angles...
> ![[eulerAngles.png]]
> 
> - $\alpha$ or $\phi$ (precession) represents a rotation around the _z_ axis,
> - $\beta$ or $\theta$ (nutation) represents a rotation around the _N_ or x′ axis -- inclination
> - $\gamma$ or $\psi$ (intrinsic rotation) represents a rotation around the _Z_ or z″ axis.


## Kepler's 1st Law

Bound motion of two body systems move in elliptical orbits.

$$
r(\phi) = \frac{a \, (1 - \varepsilon^{2})}{1 + \varepsilon \cos \phi}
$$

> [!derivation] Proof of Statement (1)
> 
> Using [[Center of Mass & Relative Coordinates]] with Lagrangian Mechanics...
> $$
\begin{align}
> 	T &= \frac{1}{2} \mu \left( \dot{r}^{2} + r^{2} \dot{\phi}^{2} \right) \\
> 	U &= - \frac{G M \mu}{r} = - \frac{k}{r} \\
> 	\\
> 	\mathcal{L} &= T - U = \frac{1}{2} \mu \left( \dot{r}^{2} + r^{2} \dot{\phi}^{2} \right) + \frac{k}{r}
> \end{align}
> $$
> ...we can find the equations of motion for $r$ and $\phi$ through the Euler-Lagrange equation.
> 
> **Equation of Motion for $\phi(t)$ :** 
> 
> $$
\begin{align}
> 	\td{}{t} \left( \pd{\mathcal{L}}{\dot{\phi}} \right) - \pd{\mathcal{L}}{\phi} &= 0 \\
> 	\td{}{t} \left( \mu r^{2} \dot{\phi} \right) &= 0
> 	\hRightarrow
> 	\td{L}{t} = 0
> 	\hWhere
> 	L \equiv \mu r^{2} \dot{\phi}
> \end{align}
> $$
> This is a statement of the **Conservation of Angular Momentum ($L$)**. Re-writing our Lagrangian in terms of $L$...
> $$
> \mathcal{L} = \frac{1}{2} \mu \dot{r}^{2} + \frac{L^{2}}{2 \mu r^{2}} + \frac{k}{r}
> $$
> 
> **Equation of Motion for $r(t)$ :**
> 
> $$
\begin{align}
> 	\td{}{t} \left( \pd{\mathcal{L}}{\dot{r}} \right) - \pd{\mathcal{L}}{r} &= 0 \\
> 	\td{}{t} \left( \mu \dot{r} \right) - \left( \mu r \dot{\phi}^{2} - \frac{k}{r^{2}} \right) &= 0 \\
> 	\td{}{t} \left( \mu \dot{r} \right) - \mu r \dot{\phi}^{2} + \frac{k}{r^{2}} &= 0 \\
> 	\mu \ddot{r} - \frac{L^{2}}{\mu r^{3}} + \frac{k}{r^{2}} &= 0
> \end{align}
> $$
> $$
> \left[ \hspace{1cm}
\begin{align}
> 	\dot{r} = \td{r}{t} &= \td{\phi}{t} \td{r}{\phi} \hspace{1cm} \textcolor{gray}{\left\{ \dot{\phi} = \td{\phi}{t} = \frac{L}{\mu r^{2}} \right\}} \\
> 	&= \frac{L}{\mu r^{2}} \td{r}{\phi} \\
> 	\\
> 	\ddot{r} = \tdd{r}{t} &= \td{}{t} \left( \td{r}{t} \right) \\
> 	&= \td{\phi}{t} \td{}{\phi} \left( \td{\phi}{t} \td{r}{\phi}  \right) \\
> 	&= \frac{L^{2}}{\mu^{2} r^{2}} \td{}{\phi} \left( \frac{1}{r^{2}} \td{r}{\phi} \right)
> \end{align}
> \hspace{1cm} \right]
> $$
> 
> $$
\begin{align}
> 	\mu \ddot{r} - \frac{L^{2}}{\mu r^{3}} + \frac{k}{r^{2}} &= 0 \\
> 	\mu \left[ \frac{L^{2}}{\mu^{2} r^{2}} \td{}{\phi} \left( \frac{1}{r^{2}} \td{r}{\phi} \right) \right] - \frac{L^{2}}{\mu r^{3}} + \frac{k}{r^{2}} &= 0 \\
> 	\td{}{\phi} \left( \frac{1}{r^{2}} \td{r}{\phi} \right) - \frac{1}{r} + \frac{\mu k}{L^{2}} &= 0 \\
> 	\td{}{\phi} \left( - \td{(\tfrac{1}{r})}{\phi} \right) - \frac{1}{r} + \frac{\mu k}{L^{2}} &= 0 \\
> 	- \tdd{W}{\phi} - W + C &= 0 \hWhere 
> 			W(r) = \frac{1}{r} \hspace{1cm}
> 			C = \frac{\mu k}{L^{2}} \\
> 	\tdd{W}{\phi} + W - C &= 0 \\
> 	\tdd{Y}{\phi} + Y &= 0 \hWhere Y(r) = W(r) - C \\
> \end{align}
> $$
> This  is the differential equation for the simple harmonic oscillator equation. After simplifying the solution form...
> $$
> Y(r) = B \cos (\phi - \phi_{0}) = \frac{1}{r} - \frac{\mu k}{L^{2}}
> \hRightarrow
\begin{aligned}[t]
> 	\frac{1}{r} \fpar{L^{2}}{\mu k} &= 1 + \fpar{L^{2} B}{\mu k} \cos (\phi - \phi_{0})
> \end{aligned}
> $$
> ...we can correlate the equation structure to a conic section with the focus at the origin.
> 
> ![[conicSections.png|align:center]]
> 
> 1) If $\varepsilon = 0$, then we have bounded motion in a *circular orbit*. $\left( \text{radius} = r = a = \frac{L^{2}}{G M \mu^{2}} \right)$
> 2) If $0 < \varepsilon < 1$, then we have bounded elliptical motion.
> 3) If $\varepsilon = 1$, then we have unbounded parabolic motion.
> 4) If $\varepsilon > 1$, then we have unbounded hyperbolic motion.
> 
> $$
> \frac{\alpha}{r} = 1 - \varepsilon \cos (\phi - \phi_{0}) \hTherefore \varepsilon = \frac{L^{2} B}{\mu k} \hspace{0.5cm} , \hspace{0.5cm} \boxed{\alpha = a (1 - \varepsilon^{2}) = \frac{L^{2}}{\mu k} = \frac{L^{2}}{G M \mu^{2}}}
> $$
> $$
> r(\phi) = \frac{L^{2} /\mu k}{1 + \tfpar{L^{2} B}{\mu k} \cos \phi} 
> \hRightarrow
> \boxed{r(\phi) = \frac{a \, (1 - \varepsilon^{2})}{1 + \varepsilon \cos \phi}}
> $$

> [!note] 
> With the [[#Conservation of Energy]], we can express the *eccentricity ($\varepsilon$)* in terms of total energy ($E$).
> $$
> \begin{align}
> 	a (1 - \varepsilon^{2}) = \frac{L^{2}}{\mu k} \hRightarrow E &= - \frac{\mu k}{2 a} = - \frac{\mu^{2} k^{2} (1 - \varepsilon^{2})}{2 L^{2}} \\
> 	& \\
> 	&\boxed{\varepsilon = \sqrt{1 + \frac{2 E L^{2}}{\mu^{2} k^{2}}}}
> \end{align}
> $$

## Kepler's 2nd Law

The radius vector of the orbiting body sweeps out equal areas during equal intervals of time.
$$\td{A}{t} = \frac{L}{2 \mu} \hWhere L = \mu r^{2} \dot{\phi}$$

![[kepler2a.png|300]] ![[kepler2b.png|300]]

> [!derivation] Proof of Statement (2)
> We look at a small period of time ($\rd t$) and take the time derivative of the area of a the created triangle...
> $$
> \begin{align}
> 	\rd A &= \frac{1}{2} r \, (r \, \rd \phi) + \cancelto{\rm \; 0, \; second \ order}{\frac{1}{2} (r \, \rd \phi) \, \rd r} \\
> 	\\
> 	\td{A}{t} &= \td{}{t} \left( \frac{1}{2} r^{2} \, \rd \phi \right) = \frac{1}{2} r^{2} \dot{\phi} = \frac{L}{2 \mu} \; \boxed{= \text{constant}}
> 	\end{align}
> $$

## Kepler's 3rd Law

The square of a planet's orbital period ($P$) is proportional to the cubed-length of the semi-major axis ($a$) of the orbit.

$$
\text{Period-Radius Relationship:} \hspace{1cm} P^{2} = \frac{4 \pi^{2} a^{3}}{G M_{\rm tot}} \hRightarrow P^{2} \propto a^{3}
$$

> [!derivation] Proof of Statement (3)
We compare the area of an ellipse ($A = \pi a b$) to the rate of change in the area ($\td{A}{t}$). 
>
> $$
> \begin{align}
> 	\pi a b &= \int_{0}^{P} \left( \td{A}{t} \right) \; \rd t
	> 	\hspace{1.4cm}
	> 	\textcolor{gray}{\left[ b = a \sqrt{1 - \varepsilon^{2}} \right]} \\
	> \pi a^{2} \sqrt{1 - \varepsilon^{2}} &= \int_{0}^{P} \left( \frac{L}{2 \mu} \right) \; \rd t \\
> 	\pi a^{2}\sqrt{1 - \varepsilon^{2}} &= \fpar{L}{2 \mu} \int_{0}^{P} \rd t 
	> 	\hspace{1.5cm}
	> 	\textcolor{gray}{\left[ a (1 - \varepsilon^{2}) = \frac{L^{2}}{k \mu} = \frac{L^{2}}{G M \mu^{2}} \right]} \\
	> \\
	> \pi a^{2}\sqrt{1 - \varepsilon^{2}} &= \frac{P}{2} \sqrt{G M a (1 - \varepsilon^{2})} \\
> 	\\
> 	P^{2} &= \frac{4 \pi^{2} a^{3}}{G M} \hRightarrow \boxed{ \;P^{2} \propto a^{3} \;}
> \end{align}
> $$


## Conservation of Energy

In a bound Keplerian Orbit, energy is conserved.

> [!derivation] Proof of Statement (E)
> Instead of using Lagrangian Mechanics ($\mathcal{L} = T - U$), we will look at the total energy of the system ($E = T + U$) and its time derivative.
>
> $$
> E = T + U  = \frac{1}{2} \mu \dot{r}^{2} + \frac{L^{2}}{2 \mu r^{2}} - \frac{k}{r} \hWhere k = G M \mu
> $$
> 
> Taking the time-derivative, we can prove that energy is conserved. 
> $$
> \td{E}{t} = \td{}{t} \left( \frac{1}{2} \mu \dot{r}^{2} + \frac{L^{2}}{2 \mu r^{2}} - \frac{k}{r} \right) = \mu \dot{r} \ddot{r} - \frac{L^{2} \dot{r}}{\mu r^{3}} + \frac{k \dot{r}}{r^{2}}
> $$
> $$
> \left[ \hspace{1cm}
> \begin{align}
> 	\text{Equation of Motion for $r(t)$:} \hspace{1cm} \ddot{r} = \frac{L^{2}}{\mu^{2} r^{3}} - \frac{k}{\mu r^{2}}
> \end{align}
> \hspace{1cm} \right]
> $$
> $$
> \td{E}{t} = \left( \frac{L^{2} \dot{r}}{\mu r^{3}} - \frac{k \dot{r}}{r^{2}} \right) - \frac{L^{2} \dot{r}}{\mu r^{3}} + \frac{k \dot{r}}{r^{2}} = 0
> \hRightarrow Conserved.
> $$

**Energy in Terms of the Semi-Major Axis:**

With energy conserved throughout the orbit, we can write the energy in terms of of the semi-major axis ($a$) by choosing to specifically look at one position of the orbit. By convention, we take the initial position of $m_{2}$ to be at the pericenter.
$$
\begin{align}
	\phi_{0} \equiv \phi(t_{0} = 0) = 0 &\hRightarrow r(\phi_{0}) = \frac{a (1 - \varepsilon^{2})}{1 + \varepsilon}  = a (1 - \varepsilon) \\
	\\
	E &= \frac{1}{2} \mu \dot{r}^{2} + \frac{L^{2}}{2 \mu r^{2}} - \frac{k}{r} 
		\hspace{2.5cm} 
		\textcolor{gray}{\left[ \; \dot{r}(\phi_{0}) = 0 \; \right]} \\
	&= \frac{L^{2}}{2 \mu a^{2} (1 - \varepsilon)^{2}} - \frac{k}{a(1 - \varepsilon)} 
		\hspace{1cm} 
		\textcolor{gray}{\left[ \; a (1 - \varepsilon^{2}) = \frac{L^{2}}{\mu k} \; \right]} \\
	&= \frac{k (1 - \varepsilon^{2})}{2 a (1 - \varepsilon)^{2}} - \frac{k}{a(1 - \varepsilon)} \\
	&= \frac{k}{2a} \left( \frac{(1 - \varepsilon^{2})}{(1 - \varepsilon)^{2}} - \frac{2}{(1 - \varepsilon)} \right)\\
	&= - \frac{k}{2a} \\
	&= - \frac{G M \mu}{2a} \\
\end{align}
$$
$$
\boxed{ \; E = - \frac{G M \mu}{2 a} = - \frac{G M_{1} M_{2}}{2 a} \; }
$$
