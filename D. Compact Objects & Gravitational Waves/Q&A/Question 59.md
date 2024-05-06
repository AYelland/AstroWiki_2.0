### Question
---
Describe a scenario whereby a neutron star can be formed in a binary system and have the system remain bound.

### Answer
---
For a [[Neutron Star|neutron star]] to be formed in a [[Binary Stars|binary]], then its predecessor must have been a high mass star ($M \gtrsim 8 \; {\rm M_{\odot}}$) that underwent a [[Core-Collapse|core-collapse]] [[Stellar Explosions#Supernova|supernova]].

In this situation, we can calculated the limit for which the companion star can remain bound in the binary system. 

> [!note] Notation
> The subscript of 0 implies the state of the system prior to the SNe. Varibales without the subscript imply after the SNe.

**Before the Supernovae:**

We will assume that the two stars had masses ($M_{1}$ and $M_{2}$) before the [[Stellar Explosions#Supernova|SNe]], and that they were bound in a circular orbit, separated by the distance $a$. The total initial energy of the binary system is then: *(see [[Kepler's Laws of Planetary Motion#Conservation of Energy|Keplerian Orbit Energy]])*

$$E_{0} = - \frac{G M_{1} M_{2}}{2 a} = - \frac{G M_{\rm 0} \mu_{0}}{2 a} \hWhere M_{0} \equiv M_{1} + M_{2} \quad , \quad \mu_{0} \equiv \frac{M_{1} M_{2}}{M_{0}}$$

Using [[Center of Mass & Relative Coordinates|center of mass]] coordinates, we can also consider the effective one-body problem of reduced mass ($\mu_{0}$) and relative velocity ($v_{0}$). With the [[Virial Theorem]], we can express the initial orbital energy as...

$$2 T + U = 0 \hRightarrow E_{0} = -T = - \left( \frac{1}{2} \mu_{0} v_{0}^{2} \right)$$

...such that we can express the relative velocity in terms of the total mass ($M_{0}$).
$$v_{0}^{2} = \frac{G M_{0}}{a}$$

**After the Supernovae:**

We now consider Star 1 undergoing a spherically-symmetric [[Stellar Explosions#Supernova|supernova]], reducing its mass from $M_{1}$ to the remnant mass $M_{\rm R} = q M_{1}$ where $q \in [0,1]$. Due to spherical symmetry no additional momentum gained by Star 1 (such that $|\vec{v}_1|$ remains constant).

This assumption does not impart significant momentum onto the other star (most of the energy is release through in neutrinos anyway, see [[Question 58|58]]). As such, the relative speed of the stars will not change ($v = v_0, a = a_0$). Only the mass of Star 1, and thus, the reduced mass is changed ($\mu_{0} \rightarrow \mu$). 

With this, the total energy after explosion is composed of the kinetic energy of the relative coordinates and the gravitational potential.

$$E = \frac{1}{2} \mu v_{0}^{2} - \frac{G M_{\rm R} M_{2}}{a} = \frac{1}{2} \mu v_{0}^{2} - \frac{G (q M_{1}) M_{2}}{a}$$

**Condition to Remain Bound:**

The binary masses in the system will remain gravitationally bound if $E < 0$. Otherwise, the SN removed too much of the mass (and gravitational energy) such that the masses will drift apart.

Plugging in the expression for $v_{0}^{2}$ into our limit such that...

 $$
\begin{align}
	E < 0 \hRightarrow \hspace{3cm} \frac{1}{2} \mu v_{0}^{2} &- \frac{G (q M_{1}) M_{2}}{a} < 0 \\
	\\\
	\frac{1}{2} \mu v_{0}^{2} &< \frac{G q M_{1} M_{2}}{a} \\
	\frac{1}{2} \fpar{(q M_{1}) M_{2}}{M} \fpar{G M_{0}}{a} &< \frac{G q M_{1} M_{2}}{a} \\
	\frac{1}{2} &< \fpar{M}{M_{0}}
\end{align}
$$

...the masses will remain in a bound orbit after the SN if....

$$\boxed{\; \frac{M_{\rm final}}{M_{\rm initial}} > \frac{1}{2} \; } \hWhere M_{i} \equiv \text{total mass}$$
 
Meaning, if we don't lose more than half of the total mass of the system, the binary system will persist and the masses will remain bound.

> [!note]
> This limit is assuming that there is no momentum transfer to the secondary mass through the SN ejecta. This can be turned into a condition to improve the constraints, but the above limit is sufficient. 
