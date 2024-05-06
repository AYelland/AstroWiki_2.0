---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
  - general relativity
  - GR
---
> [!note]
> Here, there is some basic info; however, we are not currently required to know general relativity for the ASTRO Oral Qual beyond basic knowledge of Schwarzschild and some things about [[Gravitational Waves]].

## Schwarzschild Metric

The Schwarzchild metric is an exact (and vacuum-region) solution to the Einstein field equations that describes the geometry of spacetime around an uncharged, spherically symmetric, and non-rotating body where the universal cosmological constant is zero.

Omitting tensor notation entirely, the line element for proper time takes the form

$$
- c^{2} \rd \tau^{2} = - \left( 1 - \frac{R_{\rm s}}{r} \right) c^{2} \rd t^{2} + \left( 1 - \frac{R_{\rm s}}{r} \right)^{-1} \rd r^{2} + r^{2} ( \rd \theta^{2} + \sin^{2}\theta \, \rd \varphi^{2} )
$$

...where $R_S = \frac{2GM}{c^2}$ is the **Schwarzschild radius** and we use the so-called "Schwarzschild coordinates"  
$$\begin{align}
t &\in (-\infty,\infty) \\
r &\in (0,\infty) \\
\theta &\in (0,\pi) \\
\varphi &\in (0,2\pi) \\
\end{align}$$

## Kerr Metric

The Kerr metric is a generalization of the [[#Schwarzschild Metric]] for a rotating body. In other words, the Kerr metric is an exact solution to the Einstein field equations that describes the geometry of spacetime around an uncharged, spherically symmetric, and rotating body where the universal cosmological constant is zero.

$$
\begin{aligned}
	\rd s^{2} &= - c^{2} \rd \tau^{2} \\
	&= - \left( 1 - \frac{R_{\rm s} r}{\Sigma} \right) c^{2} \rd t^{2} + \frac {\Sigma}{\Delta} \rd r^{2} + \Sigma \rd \theta^{2} + \left( r^{2} + a^{2} + \frac{R_{\rm s} r a^{2}}{\Sigma} \sin^{2} \theta \right) \sin^{2} \theta \, \rd \varphi^{2} - \frac{2 R_{\rm s} r a \sin^{2} \theta}{\Sigma} c \, \rd t \, \rd \varphi 
\end{aligned}
$$

where the coordinates $(r, \theta, \varphi)$ are standard oblate spheroidal coordinates (which are equivalent to the cartesian coordinates),  $R_{\rm s}$ is the Schwarzschild radius, and $(a, \Sigma, \Delta)$ are length scales.

$$
R_{\rm s} = \frac{2 G M}{c^{2}}
\hspace{2.5cm}
\begin{aligned}
	x &= \sqrt{r^{2} + a^{2}} \, \sin \theta \cos \varphi \\
	y &= \sqrt{r^{2} + a^{2}} \, \sin \theta \sin \varphi \\
	z &= r \cos \theta
\end{aligned}
\hspace{2.5cm}
\begin{aligned}
	a &= \frac{J}{Mc} \\
	\Sigma &= r^{2} + a^{2} \cos^{2} \theta \\
	\Delta &= r^{2} - R_{\rm s} r + a^{2}
\end{aligned}
$$

A key feature is the $\rd t \, \rd \varphi$ term that couples time and the motion in the plane of rotation. When the black hole's angular momentum goes to zero, this term disappears such that we are left with the [[#Schwarzschild Metric]].

## Friedmann–Lemaître–Robertson–Walker Metric
*(Abbrev. as **FLRW metric**)*

The **Friedmann–Lemaître–Robertson–Walker Metric** is a solution to the Einstein field equations that describes the geometry of spacetime following the isotropic expansion and contraction of a homogenous universe. 

These assumptions lead to a form of the metric...

$$- c^{2} \rd \tau^{2} = - c^{2} \rd t^{2} + a(t)^{2} \, \rd \mathbf{\Sigma}^{2}$$
...where $\rd \mathbf{\Sigma}$ is the line element on a 3D space of uniform curvature...

$$\rd \mathbf{\Sigma}^{2} \equiv \frac{\rd r^{2}}{1 - k r^{2}} + r^{2} \rd \mathbf{\Omega}^{2} \hWhere \rd \mathbf{\Omega}^{2} = \rd \theta^{2} + \sin^{2}{\theta} \, \rd \varphi^{2}$$

...and $k$ represents the curvature of the spacetime.

|  $k$   | Curvature | Topology | Example          |
| :----: | :-------: | :------: | :--------------: |
|  $+1$  | positive  |  closed  | 3-sphere         |
| $~~~0$ | zero      |   flat   | Euclidean space  |
|  $-1$  | negative  |   open   | Hyperbolic space |

In this parameterization, $a$ has dimensions of length (and represents the radius of curvature) and $r$ is dimensionless. Additionally, we are using the [[Distances#Comoving Distance|comoving coordinate system]] ($r,\theta,\varphi$), which is invariant under the expansion of the universe described by $a(t)$. 

In such a universe, the relation between scale factors at a certain [[Redshift|redshift]] ($z$) and today's scale factor ($a_{0}$) is given by 

$$a(z) = \frac{a_{0}}{1+z}$$

We usually define $a$ such that $a_0=1$.

By applying this metric in the Einstein field equations, we find two differential equations, one of which represents the energy conservation while the other represents the Hubble parameter, $H(a)$.

$$
H^{2}(a) \equiv \underbrace{\fpar{\dot{a}}{a}^{2} = \frac{8 \pi G \rho}{3} - \frac{k c^{2}}{a^{2}} +\frac{\Lambda c^{2}}{3}}_{\text{Hubble Parameter}}
\hspace{2cm}
\underbrace{\frac{\ddot{a}}{a} = - \frac{4 \pi G}{3} \left( \rho + \frac{3 p}{c^{2}} \right) + \frac{\Lambda c^{2}}{3}}_{\text{Conservation of Energy}}
$$

These equations are known as the **Friedmann Equations.** For relativistic bosons and fermions $p = \rho c^{2/3}$, and for non-relativistic particles $p = 0$.

## Classical Tests of General Relativity

1. Precession of Perihelion of Mercury
2. [[Question 97|Shapiro Time Delay]]
3. [[Redshift#Gravitational Redshift]]
4. [[Gravitational Lensing]] - angle between real source and apparent source double what was predicted without GR

Other Tests of GR
- [[Gravitational Waves]]
- [[Question 56|Hulse-Taylor Pulsar]]


