### Question
---
What is the Robertson-Walker metric? What are the Friedmann equations? How does the universe expand if it is (i) radiation dominated? (ii) matter dominated with $\Omega \ll 1$, $\Omega = 1$, $\Omega \gg 1$ (iii) dominated by a cosmological constant?

### Answer
---
##### What is the Robertson-Walker metric? What are the Friedmann equations? 

The **Friedmann–Lemaître–Robertson–Walker Metric** is a solution to the Einstein field equations that describes the geometry of spacetime following the isotropic expansion and contraction of a homogenous universe. *(See [[General Relativity#Friedmann–Lemaître–Robertson–Walker Metric|FLRW Metric]])*

$$- c^{2} \mathrm{d} \tau^{2} = - c^{2} \mathrm{d} t^{2} + a(t)^{2} \left( \frac{\mathrm{d} r^{2}}{1 - k r^{2}} + r^{2} \mathrm{d} \mathbf{\Omega}^{2} \right) \hspace{1cm} \text{where} \hspace{1cm} \mathrm{d} \mathbf{\Omega}^{2} = \mathrm{d} \theta^{2} + \sin^{2}{\theta} \, \mathrm{d} \varphi^{2}$$

The **Friedmann Equations** are the two differential equations that come out of the Einstein field equations when you apply the FLRW metric. One represents the conservation of energy and the other represents the expanding and contracting of space through the Hubble parameter. *(See [[Friedmann Equation]].)*

$$H^{2}(a) \equiv \underbrace{\left(\frac{\dot{a}}{a}\right)^{2} = \frac{8 \pi G \rho}{3} - \frac{k c^{2}}{a^{2}} +\frac{\Lambda c^{2}}{3}}_{\text{Hubble Parameter}}
\hspace{2cm}
\underbrace{\frac{\ddot{a}}{a} = - \frac{4 \pi G}{3} \left( \rho + \frac{3 p}{c^{2}} \right) + \frac{\Lambda c^{2}}{3}}_{\text{Conservation of Energy}}$$
$${\rm or}$$
$$H^{2}(a) = H_{0}^{2} E^{2}(a) = H_{0}^{2} \Big( \Omega_{M,0} \, a^{-3} + \Omega_{r,0} \, a^{-4} + \Omega_{k,0} \, a^{-2} + \Omega_{\Lambda,0} \Big)$$

##### How does the universe expand if it is (i) radiation dominated?

> [!space] Radiation-Dominated: $\quad \Omega_{r} = 1 \quad , \quad \Omega_{M} = \Omega_{k} = \Omega_{\Lambda} = 0$

In a radiation-dominated (flat) universe, the [[Friedmann Equation]] reduces to...

$$E^{2}(a) = \frac{H^{2}(a)}{H_{0}^{2}} = a^{-4}$$

...such that when we use the separation of variables to find the time dependence, we find...

$$H(a) = \frac{\dot{a}}{a} = \sqrt{H_{0}^{2} a^{-4}} = \frac{H_{0}}{a^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{a(t)} a \; \mathrm{d} a = \int_{0}^{t} H_{0} \; \mathrm{d} t$$

$$\boxed{ \; a(t) = \sqrt{2 H_{0} t} \quad \propto t^{1/2} \;}$$

##### How does the universe expand if it is (ii) matter dominated with $\Omega \ll 1$, $\Omega = 1$, $\Omega \gg 1$?

> [!space] Flat, Matter-Dominated: $\quad \Omega_{M} =1 \quad , \quad \Omega_{r} = \Omega_{k} = \Omega_{\Lambda} = 0$

In a matter-dominated (flat) universe, the [[Friedmann Equation]] reduces to...

$$E^{2}(a) = \frac{H^{2}(a)}{H_{0}^{2}} = a^{-3}$$

...such that when we use the separation of variables to find the time dependence, we find...

$$H(a) = \frac{\dot{a}}{a} = \sqrt{H_{0}^{2} a^{-3}} = \frac{H_{0}}{a^{3/2}} \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{a(t)} a^{1/2} \; \mathrm{d} a = \int_{0}^{t} H_{0} \; \mathrm{d} t$$

$$\boxed{ \; a(t) = \left( \frac{3}{2} H_{0} t \right)^{2/3} \quad \propto t^{2/3} \;}$$

> [!space] Non-Flat, Matter-Dominated: $\quad \Omega_{M} \ne 1 \quad \implies \quad \Omega_{M} + \Omega_{k} = 1 \quad , \quad \Omega_{r} = \Omega_{\Lambda} = 0$

In a matter-dominated (non-flat, $k \ne 0$) universe, the [[Friedmann Equation]] reduces to...

$$E^{2}(a) = \frac{H^{2}(a)}{H_{0}^{2}} = \Omega_{M} \, a^{-3} + \Omega_{k} \, a^{-2}$$

...such that when we use the separation of variables to find the time dependence, we find...

$$\begin{align}
	H(a) = \frac{\dot{a}}{a}&= H_{0} \sqrt{\Omega_{M} \, a^{-3} + (1-\Omega_{M}) \, a^{-2}} \\
	\frac{\dot{a}}{a} &= \frac{H_{0} \,\Omega_{M}^{1/2}}{a} \sqrt{a^{-1} + \left(\frac{1-\Omega_{M}}{\Omega_{M}}\right)}
\end{align}$$
$$\Downarrow$$
$$\int_{0}^{a(t)} \left( a^{-1} + \left(\tfrac{1-\Omega_{M}}{\Omega_{M}}\right) \right)^{-1/2} \; \mathrm{d} a = \int_{0}^{t} H_{0} \, \Omega_{M}^{1/2} \; \mathrm{d} t$$

To find $a(t)$, we look at the limiting cases of extremely high and low matter contributions. 

$$
\begin{alignat}{3}
	\Omega_{M} \ll 1 : \quad \Omega_{k} &= 1 - \Omega_{M} > 0 &\hspace{1cm} \Rightarrow \hspace{1cm} &\text{negative curvature} \rightarrow \textbf{open universe} \\
	\Omega_{M} \gg 1 : \quad \Omega_{k} &= 1 - \Omega_{M} < 0 &\hspace{1cm} \Rightarrow \hspace{1cm} &\text{positive curvature} \rightarrow \textbf{closed universe}
\end{alignat}
$$

In the **open universe**, space will continuing expanding forever. In the **closed universe**, space will expand up to a some threshold and then collapse in on itself.

> [!note] Recall the curvature ($k$) has the opposite sign of the cosmological density parameter ($\Omega_{k} \propto - k /a^{2}$).

> [!space] Open, Matter-Dominated Universe: $\quad \Omega_{M} \ll 1 \quad \implies \quad \Omega_{k} = 1 - \Omega_{M} \simeq 1$

 At later times (high $z$ and low $a$), the curvature term ($\propto a^{-2}$) will dominate over the matter term ($\propto a^{-3}$) $\implies$ **curvature dominated** ($\Omega_{k} = 1$).

$$E^{2}(a) = \frac{H^{2}(a)}{H_{0}^{2}} = a^{-2} \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{a(t)} \mathrm{d} a = \int_{0}^{t} H_{0} \; \mathrm{d} t$$

$$\boxed{ \; a(t) = H_{0} \, t \quad \propto t \;}$$

> [!space] Closed, Matter-Dominated Universe: $\quad \Omega_{M} \gg 1 \quad \implies \quad \Omega_{k} = 1 - \Omega_{M} \simeq - \Omega_{M}$

At earlier times (low $z$ and high $a$), the curvature and matter terms are about the same order of magnitude.

$$H^{2}(a) = H_{0}^{2} \Big( \Omega_{M} a^{-3} + \Omega_{k} a^{-2} \Big) \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{a(t)} \left( a^{-1} -1 \right)^{-1/2} \; \mathrm{d} a = \int_{0}^{t} H_{0} \, \Omega_{M}^{1/2} \; \mathrm{d} t$$

$$- \sqrt{a-a^{2}} - \arctan \left(\frac{\sqrt{1-a}}{\sqrt{a}}\right) + \frac{\pi}{2} = H_{0} \, \Omega_{M}^{1/2} \, t \hspace{1cm} \Rightarrow \hspace{1cm} \text{Solve for }a(t).$$

##### How does the universe expand if it is (iii) dominated by a cosmological constant?

> [!space] Dark Energy-Dominated: $\quad \Omega_{\Lambda} = 1 \quad , \quad \Omega_{M} = \Omega_{r} = \Omega_{k} = 0$

In a Dark Energy-dominated universe where $\Omega_{\Lambda}=1$, the [[Friedmann Equation]] reduces to...

$$E^{2}(a) = \frac{H^{2}(a)}{H_{0}^{2}} = 1$$

...such that when we use the separation of variables to find the time dependence, we find...

$$H(a) = \frac{\dot{a}}{a} = H_{0} \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{a(t)} \frac{\mathrm{d} a}{a} = \int_{0}^{t} H_{0} \; \mathrm{d} t$$

$$\boxed{ \; a(t) = e^{H_{0} t} \;}$$