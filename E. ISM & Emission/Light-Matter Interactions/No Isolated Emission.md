---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
An isolated particle with no internal structure cannot spontaneously emit or absorb a photon, as one cannot do so while conserving both energy and momentum.

**Explanation:**

A photon has (1D) momentum and energy:

$$p = \hbar k = h/\lambda \hspace{2cm} E = h\nu = hc/\lambda = pc$$

Let consider an electron with energy ($E_{e} = m_{e} c^{2}$) and momentum ($p_{e}$) in its rest frame. If a photon spontaneously emits from the electron, then the total system must conserve energy and momentum. 

Using "primes" to post-emission variables...

$$
\begin{aligned}
	E_{e} &= E'_{e} + |\vec{p}| c \\
	\vec{p}_{e} &= \vec{p}_{e}^{\,\prime} + \vec{p}
\end{aligned}
\hWhere
\begin{aligned}
	E_{e} &= m_{e} c^{2} \\
	\vec{p}_{e} &= 0
\end{aligned}
$$

...we see that the electron and photon must have equal and opposite momenta after the emission: $\vec{p}_{e}^{\,\prime} = - \vec{p}$ and $|p_{e}^{\,\prime}| = |p|$. 

This implies that the resulting electron energy is: 

$$E'_{e} = m_{e} c^{2} - |\vec{p}_{e}^{\,\prime}| c$$

Filling in the relativistic kinetic energy, we find...

$$E'_{e} = c \sqrt{|\vec{p}_{e}^{\,\prime}|^{2} + m_{e}^{2} c^{2}} \hRightarrow 
\begin{aligned}[t]
	\sqrt{|\vec{p}_{e}^{\,\prime}|^{2} + m_{e}^{2} c^{2}} &= m_{e} c - |\vec{p}_{e}^{\,\prime}| \\
	\sqrt{x^{2} + y^{2}} &= y - x
\end{aligned}$$

This equation cannot be true for any positive $x$ and $y$ by the triangle inequality, unless $|\vec{p}_e{}'| = 0$ in which case the photon momentum is also zero and nothing happens. That is, **this process cannot occur if both energy and angular momentum are conserved.**