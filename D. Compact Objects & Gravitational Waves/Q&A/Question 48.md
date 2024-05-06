---
aliases:
  - Roche Potential
  - Roche Limit
---
### Question
---
What is the Roche potential in a binary system? Describe carefully the assumptions that go into deriving it. Define the Roche limit.

### Answer
---
##### What is the Roche potential in a binary system?

![[Binary Stars#Roche Lobe]]
##### Describe carefully the assumptions that go into deriving it.

1. The binary objects are treated as point sources.
2. The objects have synchronous orbits (i.e same rotation period, $\Omega_{1} \equiv \Omega_{2}$)
3. The orbits move non-relativistically (Newtonian Gravity, circular orbits in [[Center of Mass & Relative Coordinates|CoM frame]])
4. There is no Coriolis force acting on the binary objects (and test masses) if they move relative to the co-rotating frame

##### Define the Roche limit.

![[binary_rochelobe_derivation.png|align:center|600]]

The Roche Limit can be derived by evaluating the point at which the differential tidal forces exceed the self-gravity of the satellite. Using a test mass ($m$) on the satellite's surface, the two competing forces can be expressed as...

*Self-Gravitational Force of the Satellite:*

$$F_{\rm g} = \underbrace{\left( \frac{G M_{2} m}{R_{2}^{2}} \right)}_{\rm gravity\ to\ M_{2}}$$

*Differential Tidal Force to Primary Mass:*

$$
\begin{aligned}[t]
	F_{\rm t} &= - \Bigg| \underbrace{\left( \frac{G M_{1} m}{\left( a - R_{2} \right)^{2}} \right)}_{\substack{{\rm gravity\ to} \\ {\rm M_{1}\ from\ M_{2}\ surface}}} - \underbrace{\left( \frac{G M_{1} m}{a^{2}} \right)}_{\substack{{\rm gravity\ to} \\ {\rm M_{1}\ from\ M_{2}\ core}}} \Bigg| \\
	\\
	&= - G M_{1} m \left| \frac{\left( a - R_{2} \right)^{2} - a^{2}}{a^{2} \left( a - R_{2} \right)^{2}} \right| \\
	&= - G M_{1} m \left| \frac{-2 a R_{2} + R_{2}^{2}}{a^{4} - 2 a^{3} R_{2} + a^{2} R_{2}^{2}} \right| \hspace{1cm} \textcolor{gray}{\left[ a \gg R_{2} \right]} \\
	&\approx - G M_{1} m \left| -\frac{2 a R_{2}}{a^{4}} \right|
\end{aligned}
$$
$$F_{\rm t} \approx - \frac{2 G M_{1} m R_{2}}{a^{3}}$$

...where $M_{1} , R_{1} \equiv$ primary mass and radius, $M_{2} , R_{2} \equiv$ secondary/satellite mass and radius, $a \equiv$ semi-major axis.

Setting the tidal forces equal to the self-gravitational forces...

$$\left| F_{\rm g} \right| = \left| F_{\rm t} \right| \hRightarrow \frac{G M_{2} m}{R_{2}^{2}} = \frac{2 G M_{1} m R_{2}}{a^{3}}$$
$$a^{3} = \fpar{2 M_{1}}{M_{2}} R_{2}^{3}$$
$$a_{\rm roche} = \fpar{2 M_{1}}{M_{2}}^{1/3} R_{2} \hspace{1cm} \Longleftrightarrow \hspace{1cm} a_{\rm roche} = \fpar{2 \rho_{1}}{\rho_{2}}^{1/3} R_{1}$$

This calculation assumes that the orbiting bodies are rigid and represent by point masses. In reality, these bodies are fluid and they are disrupted "easier" than rigid bodies. Accounting for the fluid mechanics, the leading coefficient $\alpha \equiv 2^{1/3} \simeq 1.3$ changes to $\alpha \simeq 2.4$.

$$\boxed{\; a_{\rm roche} = \alpha \, \fpar{M_{1}}{M_{2}}^{1/3} R_{2} \hspace{1cm} \Longleftrightarrow \hspace{1cm} a_{\rm roche} = \alpha \, \fpar{\rho_{1}}{\rho_{2}}^{1/3} R_{1} \;} \hWhere \alpha \simeq 2.4$$

Physically, this means if the satellite mass is at $a = a_{\rm roche}$, then it will begin to disrupt. The material closer to the primary body will orbit faster than the material further away, causing the material to spread out and create a ring-like structure. (planetary ring formation?)

![[binary_rochelobe_disruption.png|align:center|300]]