---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - spherical top-hat
  - spherical top-hat filter
---
The **spherical top hat model** assumes density perturbations (i.e. overdensity) can be treated as a step function in radius, such that it is a sphere of constant density. 

![[tophat.png|align:center|600]]

We can use the [[Friedmann Equation]] to define the Hubble parameter in the background by assuming a flat universe when dark-energy contributions aren't dominate (early times)....

$$H^{2} = \frac{8 \pi G \bar{\rho}}{3} - \cancelto{\ flat}{\frac{k c^{2}}{a^{2}}} + \cancelto{\ \Lambda = 0}{\frac{\Lambda c^{2}}{3}} \hRightarrow \bar{\rho} = \frac{3 H^{2}}{8 \pi G}$$

...and within overdensity by assuming it acts as spherically symmetric perturbation is its own mini, closed ($k=+1$) universe ([[#^birkhoffs-theorem|Birkhoff's Theorem]]).

$$H^{2} = \frac{8 \pi G \rho}{3} - \frac{c^{2}}{a^{2}} + \cancelto{\ \Lambda = 0}{\frac{\Lambda c^{2}}{3}} \hRightarrow \rho = \frac{3}{8\pi G} \left(H^{2} + \frac{c^{2}}{a^{2}}\right)$$

The overdensity ($\delta$) is then defined as...
$$\delta(\vec{x}) = \frac{\rho(\vec{x}) - \bar{\rho}}{\bar{\rho}} = \xi - 1 = \left( \frac{3 c^{2}}{8 \pi G} \right) \frac{1}{ \bar{\rho} a^{2}}$$

> [!space] Birkhoff's Theorem
> The dynamics of a uniform expanding self-gravitating sphere is equivalent to a section of the Universe as a whole.
^birkhoffs-theorem

## Expansion

> [!note] Using the results of [[Question 137]]
> 
> - For a radiation-dominated universe: $\bar{\rho} \propto a^{-4} \implies \delta \propto a^{2} \propto t \implies \bar{\rho} \propto t^{-2}$
> - For a matter-dominated universe: $\bar{\rho} \propto a^{-3} \implies \delta \propto a \propto t^{2/3} \implies \bar{\rho} \propto t^{-2}$

Assuming that the background universe is flat and matter-dominated at early times, we can simplify the Hubble parameter expression using the Einstein-de Sitter Universe model ($\Omega_{m} = 1 \; , \; \Omega_{\Lambda} = \Omega_{r} = \Omega_{k} = 0$).

$$\begin{alignat}{3}
    H(z) &= H_{0} \sqrt{\Omega_{r} (1+z)^{4} + \Omega_{m} (1+z)^{3} + \Omega_{k} (1+z)^{2} + \Omega_{\Lambda}} 
    &\hRightarrow 
    &H(z) = H_{0} (1+z)^{3/2} \\
    H(a) &= H_{0} \sqrt{\Omega_{r} a^{-4} + \Omega_{m} a^{-3} + \Omega_{k} a^{-2} + \Omega_{\Lambda}} 
    &\hRightarrow 
    &H(a) = H_{0} a^{-3/2}
\end{alignat}$$

We also define three new quantities...

$$\begin{alignat}{3}
    \alpha &= \frac{a}{a_{\rm ta}} &\quad&= \text{scale factor (units of scale factor at maximum expansion)} \\
    \mathcal{R} &= \frac{R}{R_{\rm ta}} &\quad&= \text{radius (units of maximum radius)}\\
    \tau &= H_{\rm ta} t &\quad&= \text{time (normalized by expansion rate at maximum expansion)}
\end{alignat}$$

...where the "${\rm ta}$" subscript represents the "turn around point" (turning point) when the halo reaches maximum expansion and the collapse begins.

If we take the derivative of $\alpha$ with respect to $\tau$, we can evaluate how the scale factor changes over the collapse. Going a step further with the separation of variables, we can find an expression for $\tau(\alpha)$.

$$\begin{align}
    \td{\alpha}{\tau} = \td{}{\tau} \fpar{a}{a_{\rm ta}} &= \frac{1}{H_{\rm ta}} \td{}{t} \fpar{a}{a_{\rm ta}} \\
        &= \frac{1}{H_{\rm ta}} \fpar{\dot{a}}{a_{\rm ta}} 
            \hspace{1.2cm} {\color{gray} \left[ H(z) = H(a) = \frac{\dot{a}}{a} \right]} \\
        &= \frac{1}{H_{\rm ta}} \fpar{\dot{a}}{a} \fpar{a}{a_{\rm ta}} \\
        &= \frac{H(a)}{H_{\rm ta}} \; \alpha 
            \hspace{2cm} {\color{gray} \left[ H_{\rm ta} = H(a_{\rm ta}) = H_{0} a_{\rm ta}^{-3/2} \right]} \\
        &= \fpar{H_{0} a^{-3/2}}{H_{0} a_{\rm ta}^{-3/2}} \alpha \\
        &= \left( \alpha^{-3/2} \right) \alpha \\
        &= \alpha^{-1/2}
\end{align}$$
$$\begin{align}
    \td{\alpha}{\tau} = \alpha^{-1/2} 
    \hRightarrow
    \int_{0}^{\alpha} (\alpha')^{1/2} \rd \alpha' &= \int_{0}^{\tau} \rd \tau' 
    \hRightarrow
    \boxed{\tau = \frac{2}{3} \alpha^{3/2}}
\end{align}$$

From [[Newton's Laws of Motion|Newtonian mechanics]], we can derive the following acceleration of the collapse, and re-express it in terms of $\mathcal{R}$ with an overdensity parameter ($\xi$).
$$\begin{align}
    \ddot{R} = \tdd{R}{t} &= - \frac{G M}{R^{2}} \\
    \tdd{R}{t} &= - \frac{G \left[ \rho_{\rm ta} \left( \frac{4}{3} \pi R_{\rm ta}^{3} \right) \right]}{R^{2}} \\
    \frac{1}{H_{\rm ta}^{2}} \left( \tdd{R}{t} \right) &= \frac{1}{H_{\rm ta}^{2}} \left( - \frac{4 \pi R_{\rm ta}^{3} \rho_{\rm ta} G}{3 R^{2}} \right) \\
    \tdd{R}{\tau} &= - \frac{4 \pi \rho_{\rm ta} G}{3 H_{\rm ta}^{2}} \fpar{R_{\rm ta}^{3}}{R^{2}} \\
    \frac{1}{R_{\rm ta}} \tdd{R}{\tau} &= - \frac{4 \pi \rho_{\rm ta} G}{3 H_{\rm ta}^{2}} \fpar{R_{\rm ta}^{2}}{R^{2}} \\
    \tdd{\mathcal{R}}{\tau} &= - \frac{4 \pi \rho_{\rm ta} G}{3 H_{\rm ta}^{2}} \fpar{1}{\mathcal{R}^{2}} 
        \hspace{1cm} {\color{gray} \left[ \rho_{\rm ta} = \rho_{\rm crit}(z_{\rm ta}) \; \xi = \fpar{3 H_{\rm ta}^{2}}{8 \pi G} \xi \right]} \\
    \tdd{\mathcal{R}}{\tau} &= - \frac{\xi}{2} \fpar{1}{\mathcal{R}^{2}} 
\end{align}$$
$$\tdd{\mathcal{R}}{\tau} = - \frac{\xi}{2 \mathcal{R}^{2}} \hWhere (\xi > 1 \text{ is an overdensity})$$

With the boundary conditions at maximum radius $(a = a_{\rm ta})$ and the beginning of time $(a = \infty)$...

$$\begin{align}
	\left\{ \;
    \begin{alignedat}{3}
        \alpha &= 1 &\quad &\implies \td{\mathcal{R}(\tau=\tfrac{2}{3})}{\tau} = 0 \\
        \\
        \alpha &= 0 &\quad &\implies \mathcal{R}(\tau=0) = 0
    \end{alignedat}
    \; \right\}
    \hRightarrow
    \boxed{\tau = \frac{1}{\sqrt{\xi}} \left( \frac{1}{2} \arcsin \left( 2 \mathcal{R} - 1 \right) - \sqrt{\mathcal{R} - \mathcal{R}^{2}} + \frac{\pi}{4} \right)}
\end{align}$$

> [!math]- Linear Extrapolation for Density Contrast
> 
> We perform a linear extrapolation of the timescale $\tau$ for early times, such that $\mathcal{R} \ll 1$ ...
> $$\begin{aligned}
> 	\tau &= \frac{1}{\xi} \left( \frac{1}{2} \arcsin \left( 2 \mathcal{R} - 1 \right) - \sqrt{\mathcal{R} - \mathcal{R}^{2}} + \frac{\pi}{4} \right) \\
> 	&\approx \frac{1}{\xi} \left( \frac{1}{2} \left( 2 \mathcal{R} - 1 \right)- \mathcal{R}^{1/2} \left(1 - \frac{\mathcal{R}}{2} \right) + \frac{\pi}{4} \right) \\
> 	&\approx \frac{1}{\xi} \left( \mathcal{R} - \frac{1}{2} - \mathcal{R}^{1/2} + \frac{\mathcal{R}^{3/2}}{2} + \frac{\pi}{4} \right) \\
> 	&\approx \frac{1}{2 \xi} \mathcal{R}^{3/2} \left( \frac{2}{\mathcal{R}^{1/2}} - \frac{1}{R^{3/2}} - \frac{2}{\mathcal{R}} + 1 + \frac{\pi}{2 R^{3/2}} \right) \\
> 	\\
> 	\\
> 	\tau &= \frac{1}{\xi} \left( \frac{1}{2} \underbrace{\arcsin \left( 2 \mathcal{R} - 1 \right)}_{-\pi/2} - \sqrt{\mathcal{R} - \mathcal{R}^{2}} + \frac{\pi}{4} \right) \\
> 	&\approx \frac{1}{\xi} \left(- \sqrt{\mathcal{R} - \mathcal{R}^{2}} \right) \\
> 	&\approx \frac{1}{\xi} \left( - \mathcal{R}^{1/2} \left(1 - \mathcal{R} \right)^{1/2} \right) \\
> 	&\approx \frac{1}{\xi} \left( - \mathcal{R}^{1/2} \left(1 - \frac{\mathcal{R}}{2} \right)\right) \\
> 	&\approx \frac{1}{\xi} \left( - \mathcal{R}^{1/2} + \frac{\mathcal{R}^{3/2}}{2} \right) \\
> 	&\approx \frac{1}{2 \xi} \mathcal{R}^{3/2} \left( 1 - \frac{2}{\mathcal{R}} \right) \\
> \end{aligned}$$

## At turnaround...

The growth of this overdensity continues until it decouples from the Hubble flow, after which it collapses. 

![[turnaround_overdensity.png|align:center|400]]

At these maximum/turnaround values, our defined dimensionless parameters become...

$$\alpha_{\rm ta} = \frac{a_{\rm ta}}{a_{\rm ta}} = 1 \hspace{1.5cm} \mathcal{R}_{\rm ta} = \frac{R_{\rm ta}}{R_{\rm ta}} = 1 \hspace{1.5cm} \tau_{\rm ta} = \frac{2}{3} \alpha_{\rm ta}^{3/2} = \frac{2}{3}$$

Applying these parameters to our $\tau$ expression above, we find the value of our overdensity parameter $(\xi)$ at turnaround ($R = R_{\rm ta}$) to be:

$$\begin{align}
    \tau_{\rm ta} &= \frac{1}{\sqrt{\xi}} \left( \frac{1}{2} \arcsin \left( 2 \mathcal{R}_{\rm ta} - 1 \right) - \sqrt{\mathcal{R}_{\rm ta} - \mathcal{R}_{\rm ta}^{2}} + \frac{\pi}{4} \right) \\
    \frac{2}{3} &= \frac{1}{\sqrt{\xi}} \left( \frac{1}{2} \arcsin \left( 1 \right) + \frac{\pi}{4} \right) \\
    \frac{2}{3} &= \frac{1}{\sqrt{\xi}} \fpar{\pi}{2} \\
    \xi &= \fpar{3 \pi}{4}^{2}
\end{align}$$
$$\boxed{\xi_{\rm ta} \equiv \frac{\rho_{\rm halo}}{\rho_{\rm universe}} = \frac{\rho_{\rm ta}}{\rho_{\rm crit}(z)} = \fpar{3 \pi}{4}^{2}}$$

$$\rho_{\rm ta} = \xi_{\rm ta} \; \rho_{\rm crit}(z_{\rm ta})  = \fpar{3 \pi}{4}^{2} \fpar{3 H_{0}^{2} (1+z_{\rm ta})^{3}}{8 \pi G} \hWhere H_{\rm ta} \equiv H_{0} (1+z_{\rm ta})$$

This $(3 \pi / 4)^{2}$ defines the minimum overdensity a spherical halo can have, such that it will "turnaround" and initiate its collapse. 

> [!note]- Duration of the Collapse
> 
> With the cosmological critical density, the turnaround density can be expressed in terms of redshift, and then applied to the [[Timescales#Dynamical Timescale|dynamical timescale]] to determine the duration of the collapse.
> 
> $$t_{\rm ff} = \left[ \frac{3 \pi}{32 G \rho_{\rm ta}} \right]^{1/2} = \frac{2}{3} \fpar{1}{H_{0} (1+z)^{3/2}}$$

## At collapse (virialization)...

$$\alpha_{\rm vir} = \left( \frac{3}{2} \tau_{\rm vir} \right)^{2/3} = 4^{1/3} \hspace{1.5cm} \underbrace{\mathcal{R}_{\rm vir} = \frac{R_{\rm vir}}{R_{\rm ta}} = \frac{1}{2}}_{\rm Virial\ Theorem} \hspace{1.5cm} \underbrace{\tau_{\rm vir} = 2 \tau_{\rm ta} = \frac{4}{3}}_{\rm collapse\ symmetry}$$

We assume that the time of the collapse is comparable to the time of expansion ($\Delta t_{\rm vir} = \Delta t_{\rm ta}$), such that $\tau_{\rm vir} = 2 \tau_{\rm ta}$ (i.e. collapse symmetry). 

We will consider the "end of the collapse" to be the point of [[Virial Theorem|virialization]] of the halo. By this, we can we use the [[Virial Theorem]] to compare the turnaround density to the collapsed, end-state density through the conservation of energy.

$$\left. \begin{alignedat}{2}
	&\text{At turnaround:} &\hspace{1cm} E &= U_{\rm ta} \\
	&\text{At collapse/virialization:} &\hspace{1cm} E &= T_{\rm vir} + U_{\rm vir} = \frac{1}{2} U_{\rm vir}
\end{alignedat} \; \right\}
\hRightarrow U_{\rm ta} = \frac{1}{2} U_{\rm vir}$$
$$
U_{\rm ta} = \frac{1}{2} U_{\rm vir} \hRightarrow \frac{1}{R_{\rm ta}} = \frac{1}{2 R_{\rm vir}} \hRightarrow \rho_{\rm ta} = \frac{1}{8} \rho_{\rm vir}$$

Additionally, using $\rho_{\rm crit} \propto H^{2} \propto t^{-2}$, we can compare the turnaround critical density to the collapsed critical density.

$$\frac{\rho_{\rm crit}(z_{\rm ta})}{\rho_{\rm crit}(z_{\rm vir})} = \fpar{t_{\rm ta}}{t_{\rm vir}}^{-2} = \fpar{1}{2}^{-2} = 4 \hRightarrow \rho_{\rm crit}(z_{\rm vir}) = \frac{1}{4} \rho_{\rm crit}(z_{\rm ta})$$

Bringing these together, we can express the overdensity parameter as:

$$\boxed{ \;\xi_{\rm vir} \equiv \frac{\rho_{\rm halo}}{\rho_{\rm universe}} = \frac{\rho_{\rm vir}}{\rho_{\rm crit}(z_{\rm vir})} = \frac{\left( 8 \rho_{\rm ta} \right)}{\left( \frac{1}{4} \rho_{\rm crit}(z_{\rm ta}) \right)} = 32 \fpar{\rho_{\rm ta}}{\rho_{\rm crit}(z_{\rm ta})} = 32 \fpar{3 \pi}{4}^{2} = \left( 18 \pi^{2} \right) \; }$$

$$\rho_{\rm vir} = \xi_{\rm vir} \rho_{\rm crit} = \left( 18 \pi^{2} \right) \fpar{3 H_{0}^{2} (1+z_{\rm vir})^{3}}{8 \pi G} \hWhere H_{\rm vir} \equiv H_{0} (1+z_{\rm vir})$$

This $18 \pi^{2} \simeq 178$ is the defining overdensity of a "collapsed" object. Meaning, if any spherical halo has an overdensity $\xi = \rho/\rho_{\rm crit} \ge 18\pi^{2}$, it is a collapsed and virialized object.

> [!note] Determining the Temperature at Collapse/Virialization
> 
> Using the Virial Theorem, we can find the temperature of the system after collapse. Since there is no cooling mechanism in this system, we only need to focus on the interactions between the baryons of the gas and the driving gravitational force.
> 
> Furthermore, if we assume the universe is completely ionized, we can treat the baryons as a spatially uniform density of $N$ monoatomic ideal gas particles. *(This is a redshift-dependent assumption, and most of the time, there is a non-negligible percentage of diatomic and polyatomic nuclei in the universe. For simplicity though, we will assume an entirely monatomic population.)*
> 
> The kinetic energy is then determined by Boltzmann Statistics...
> 
> $$\expval{K} = \frac{d}{2} N k_{B} T \hWhere d \equiv \text{d.o.f.} = 
> \begin{cases}
 >     3 &\text{for monatomic gas} \\
 >     5 &\text{for diatomic gas} \\
 >     6 &\text{for polyatomic gas} \\
> \end{cases}$$
> ...and the potential energy is determined by a [[Binding Energy#Gravitational Binding Energy|sphere of self-gravitating material]].
> 
> $$\expval{U} = - \frac{3 G M^{2}}{5 R_{\rm vir}}$$
> 
> Applying these energy values to the Virial Theorem:
> 
> $$\begin{align}
>     2 \expval{K} + \expval{U} = 0
>     \hRightarrow 
>     2 \left( \frac{3}{2} N k_{B} T \right) &+ \left( - \frac{3 G M^{2}}{5 R_{\rm vir}} \right) = 0 \\
>     3 N k_{B} T &= \frac{3 G M^{2}}{5 R_{\rm vir}} \\
>         {\color{gray} \left[ N = \frac{M}{m_{p}} \right]} \hspace{2cm} 
>     T &= \frac{G M^{2}}{5 N k_{B} R_{\rm vir}} \\
>     T &= \frac{G M m_{p}}{5 k_{B} R_{\rm vir}}
> \end{align}$$
> 
> To write temperature ($T$) solely in terms of mass ($M$), we can re-express the virial radius ($R_{\rm vir}$) in terms of thermal equilibrium (virial) density.
> 
> $$\left[ \hspace{0.2cm}
>     \begin{aligned}
>         R_{\rm vir} = \fpar{3 M}{4 \pi \rho_{\rm vir}}^{1/3} &= \left[ \frac{3 M}{4 \pi} \fpar{1}{18 \pi^{2}} \fpar{8 \pi G}{3 H_{0}^{2} (1+z)^{3}} \right]^{1/3} \\
>         &= \left[ \frac{3 M}{4 \pi} \fpar{1}{18 \pi^{2}} \fpar{8 \pi G}{3 H_{0}^{2} (1+z)^{3}} \right]^{1/3} \\
>         &= \fpar{2 G M}{18 \pi^{2} H_{0}^{2}}^{1/3} (1+z)^{-1} 
>     \end{aligned}
>     \hspace{0.2cm} \right]$$
>
> 
> $$\begin{align}
>     T &= \frac{G M m_{p}}{5 k_{B} R_{\rm vir}} \\
>     T &= \frac{G M m_{p}}{5 k_{B}} \fpar{18 \pi^{2} H_{0}^{2}}{2 G M}^{1/3} (1+z) \\
>     T &= \left[ \frac{G m_{p} (1+z)}{5 k_{B}} \fpar{18 \pi^{2} H_{0}^{2}}{2 G}^{1/3} \right] M^{2/3}
> \end{align}$$
^1d19c7


