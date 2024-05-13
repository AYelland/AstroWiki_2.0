---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
*(For more details, see [online source](https://www.mit.edu/~iancross/8901_2019A/lec011.pdf) or [[timescales.pdf|offline source]].)*

> [!sun] Hierarchy of Stellar Timescales
> 
> $$
> \begin{alignat}{6}
>     t_{\gamma} \quad &\ll \quad &t_{\rm dyn} \quad &\ll \quad &t_{\rm rad} \quad &\ll \quad &t_{\rm KH} \quad &\ll \quad &t_{\rm nuc} \\
>     10^{-10} \; {\rm s} \quad &\ll \quad &30 \; {\rm min} \quad &\ll \quad &10^{4} \; {\rm yr} \quad &\ll \quad &10^{7} \; {\rm yr} \quad &\ll \quad &10^{10} \; {\rm yr}
> \end{alignat}
> $$
> 
> Given that the timescales are strongly separated, when we look at processes occurring on one timescale, we can assume that slower processes are static and faster processes are at equilibrium.

## Photon Collision with Matter

The timescale needed for radiation and matter to reach a thermal equilibrium.

$$t_{\gamma} \sim \frac{\ell}{c} \hspace{1cm} \text{where} \hspace{1cm} \ell = \frac{1}{\alpha} = \frac{1}{n \sigma} \hspace{2cm}
\begin{align}
	\ell &= \text{mean free path} \\
	n &= \text{\# density of absorptions/scattering} \\
	\sigma &= \text{cross-section}
\end{align}$$
For the full ionization inside the [[Sun|sun]], the density of protons is $\rho \sim 1 \; {\rm g/cm^{3}}$, such that the mean-free-path (MFP) is $\ell \sim 1 \; {\rm cm}$.

$$\textbf{For the Sun:} \quad \ell \approx \frac{m_{\rm p}}{\rho \, \sigma_{\rm T}} \sim 1 \; {\rm cm} \hspace{1cm} \Rightarrow \hspace{1cm} t_{\gamma} \approx 10^{-10} \; {\rm s}$$

## Dynamical Timescale
*(Also known as the **free-fall timescale**)*

The timescale necessary for a pressureless fluid in a homogeneous sphere to gravitationally collapse and reach a mechanical, pressure equilibrium (initially released from rest).
$$t_{\rm dyn} \equiv  t_{\rm ff} = \sqrt{\frac{3 \pi}{32 G \rho}} \sim \frac{1}{\sqrt{G \rho}} \hspace{1cm} \Rightarrow \hspace{1cm} \textbf{For the Sun:} \quad t_{\rm dyn} \sim 30 \; {\rm min}$$

> [!derivation]-
> In the initial state of the system, the fluid is at rest and under the influence of a central gravitational force. After the fluid it released, the fluid will all start moving towards the center of the sphere until it cannot be compressed any further. *(In this problem, we will ignore any Fermi and Boltzmann statistics and assume all of the gas can be compressed into a central point at $r=0$.)*
>
> The rate at which the fluid collapses can be described by analyzing the acceleration of a test mass at the edge of the sphere, $r = R$.
> 
> Using Newton's Gravity relationship...
> $$F_{\rm G} = m \vec{a} = - \frac{G M m}{r^{2}} \hat{r} \hspace{1cm} \Rightarrow \hspace{1cm} a = - \frac{G M}{r^{2}}$$
> ...and the chain-rule with respect to the acceleration, ...
> $$a = \frac{\mathrm{d}^{2} r}{\mathrm{d} t^{2}} = \frac{\mathrm{d} }{\mathrm{d} t} \left( \frac{\mathrm{d} r}{\mathrm{d} t} \right) = \frac{\mathrm{d} r}{\mathrm{d} t} \frac{\mathrm{d} }{\mathrm{d} r} \left( \frac{\mathrm{d} r}{\mathrm{d} t} \right) = v \, \frac{\mathrm{d} v}{\mathrm{d} r}$$
> ...we can perform the separation of variables to find $t_{\rm ff}$.
> $$
> \begin{align}
> 	v \, \frac{\mathrm{d} v}{\mathrm{d} r} = - \frac{G M}{r^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} \int_{0}^{v} v' \, \mathrm{d} v' &= - \int_{R}^{r} \frac{G M}{r'^{2}}  \, \mathrm{d} r' \\
> 	\frac{1}{2} \left( v^{2} - 0 \right) &= - G M \left( - \frac{1}{r} + \frac{1}{R} \right) \\
> 	\frac{\mathrm{d} r}{\mathrm{d} t} = |v| &= \sqrt{\frac{2 G M}{R} \left( \frac{R}{r} - 1\right)}
> \end{align}
> $$
> $$
> \begin{align}
> 	\int_{0}^{t_{\rm ff}} \; \mathrm{d} t &= \int_{R}^{0} \frac{\mathrm{d} r}{\sqrt{\frac{2 G M}{R} \left( \frac{R}{r} - 1\right)}} \\
> 	\int_{0}^{t_{\rm ff}} \; \mathrm{d} t &= \int_{0}^{R} \frac{\mathrm{d} r}{\sqrt{\frac{2 G M}{R} \left( \frac{R}{r} - 1\right)}} \\
> 	t_{\rm ff} &= \sqrt{\frac{R}{2 G M}} \; \int_{0}^{R} \left(\frac{R}{r} - 1\right)^{-1/2} \; \mathrm{d} r \\
> 	t_{\rm ff} &= \sqrt{\frac{R^{3}}{2 G M}} \; \int_{0}^{1} \left(\frac{1}{u} - 1\right)^{-1/2} \; \mathrm{d} u \\
> 	t_{\rm ff} &= \sqrt{\frac{R^{3}}{2 G M}} \; \int_{0}^{\pi/2} \left( \frac{\sin^{2} \theta}{1 - \sin^{2} \theta} \right)^{1/2} \; \left(2 \sin \theta \cos \theta \right) \; \mathrm{d} \theta \\
> 	t_{\rm ff} &= \sqrt{\frac{R^{3}}{2 G M}} \; \int_{0}^{\pi/2} 2 \sin^{2} \theta \; \mathrm{d} \theta \\
> 	t_{\rm ff} &= \sqrt{\frac{R^{3}}{2 G M}} \left(\frac{\pi}{2}\right) \\
> 	t_{\rm ff} &= \sqrt{\frac{\pi ^{2} R^{3}}{8 G M}}
> \end{align}
> $$
> *Note: We can flip the radial integration bounds from $[R_{0}, 0] \to [0, R_{0}]$ without worrying about flipping the sign. This is because the last separation of variables originates from the absolute value of the velocity, $|v|$, where the sign is yet undetermined.*
> 
> If we now take $M = \rho V = \rho \left( \frac{4}{3} \pi R^{3}\right)$ where $\rho$ is the initial density of the spherical body of gas, then the free-fall time is...
> $$t_{\rm ff} = \sqrt{\frac{\pi ^{2} R^{3}}{8 G M}} = \sqrt{\frac{3 \pi}{32 G \rho}} \sim \frac{1}{\sqrt{G \rho}}$$

## Radiation Transport
*(Also known as the **photon diffusion timescale**)*

The timescale for radiation energy transportation for a single proton (repeatedly absorbed and emitted by other particles in a random walk) to travel from the center of a star to the surface.

$$t_{\rm rad} \approx \frac{N \ell}{c} \sim \frac{R^{2}}{\ell c} \hspace{1cm} \Rightarrow \hspace{1cm} \textbf{For the Sun:} \quad t_{\rm rad} \sim 10^{4} \; {\rm year\ for\ Sun}$$

> [!derivation]-
> If the photons were free-streamed in an unimpeded path, then they could travel from the center of the sun to the surface in $\sim 2 \; {\rm s}$.
> 
> $$c \, t_{\rm rad} = R_{\odot} \hspace{1cm} \Rightarrow \hspace{1cm} t_{\rm rad} = \frac{R_{\odot}}{c} \approx 2.32 \; {\rm s}$$
> 
> However, the mean-free-path (MFP) of the photon in the sun is $\ell \sim 1 \; {\rm cm}$, such that under a random walk, the photon will take $N$ steps (of absorption and emittion) before it can reach the surface.
> 
> $$\ell \sqrt{N} \sim R_{\odot} \hspace{1cm} \Rightarrow \hspace{1cm} N \sim \left(\frac{R}{\ell}\right)^{2}$$
> $$c \, t_{\rm rad}  = N \ell = \frac{R^{2}}{\ell} \hspace{1cm} \Rightarrow \hspace{1cm} t_{\rm rad} = \frac{R^{2}}{\ell c}$$

## Thermal Timescale
*(Also known as **Kelvin-Helmholtz Timescale**)*

The timescale it would take for a star to radiate away its gravitational binding energy, given the current luminosity of the star.
$$t_{\rm KH} \sim \frac{G M^{2}}{R L} \hspace{1cm} \Rightarrow \hspace{1cm} \textbf{For the Sun:} \quad t_{\rm KH} \sim \frac{G M_{\odot}^{2}}{R_{\odot}L_{\odot}} \sim 10^{7} \; {\rm yr}$$

> [!derivation]-
> Beginning with the average gravitational binding energy...
> ![[Binding Energy#Gravitational Binding Energy]]
>
> We can apply the [[Virial Theorem]] such that at thermal equilibrium, the total energy of the star is:
> $$\left< E \right> = \frac{1}{2} \left< U_{\rm G} \right> = - \frac{3 G M^{2}}{10 R}$$
> 
> In the 19th century when nuclear fusion was still unknown, Helmholtz and Kelvin proposed that the energy produced from stars was solely from gravitational contraction. If this were true, then we could calculate how much energy would be radiated during the contraction by assuming that the Sun was much larger than today ($R_{i} \gg R_{\odot}$).
> $$\Delta E_{\rm G} = - \left( E_{f} - E_{i} \right) = \frac{3 G M^{2}}{10} \left( \frac{1}{R_{f}} - \cancelto{0}{\frac{1}{R_{i}}} \right) = \frac{3 G M_{\odot}^{2}}{10 R_{\odot}} \approx 10^{48} \; {\rm erg}$$
> The gravitational contraction would then power the sun for...
> $$t_{\rm KH} \approx \frac{\Delta E_{\rm G}}{L_{\odot}} = \frac{3 G M_{\odot}^{2}}{10 R_{\odot} L_{\odot}} \sim 10^{7} \; {\rm yr}$$
> ...but this is much younger than the age of the Sun ($\sim 10^{9} \; {\rm yr}$) from geological evidence. 
> 
> This is still a useful timescale for gravitational collapse if the internal power source turns off in a star (i.e. if the core nuclear burning is extinguished due to fuel depletion). In star formation, this timescale is characteristic for protostar contraction into a star, before nuclear burning.

## Nuclear Timescale

The timescale that an average star spends on the main sequence, which is directly correlated to how long a star’s nuclear fuel will last under a constant burn rate.

$$t_{\rm nuc} \approx \frac{\eta \, (f X_{*} M_{*}) \, c^{2}}{L_{*}} \hspace{1cm} \Rightarrow \hspace{1cm} \textbf{For the Sun:} \quad t_{\rm nuc} \sim \frac{0.007 \, (0.1 \times 0.7 \times M_{\odot}) \,  c^{2}}{L_{\odot}} \sim 10^{10} \; {\rm year}$$

> [!derivation]-
> Using the helium production processes ([[Alpha Process|alpha process]], [[Triple-Alpha Process|triple-alpha process]]), we can use the  mass difference between the reactants and product of the nuclear reaction to determine the energy produced, according to $E = m c^{2}$. 
> 
> Fusing 4 protons into a $\ce{^{4}He}$ nucleus (*alpha particle*) creates the fractional energy change ($\eta \equiv$ fusion efficiency) of
> $$\eta = \frac{\Delta E}{E} = \frac{4 m_{\rm p} c^{2} - m_{\rm He} c^{2}}{4 m_{\rm p} c^{2}} \approx 0.007$$
> > [!tip] 
> > We can use this number as a general rule for Helium fusion: it always produces $\sim 0.7\%$ energy from the original mass. For heavier element fusion in larger stars, ($\ce{He} \to \ce{C}$ and $\ce{C} \to \ce{Fe}$) each produces another $\sim 0.1 \%$ of energy.
> 
> The nuclear timescale relationship is dependent on the stellar mass fraction of hydrogen ($M_{\rm H} \equiv X M_{*}$ where $X =$ mass fraction of $H$ in the star), the stellar luminosity ($L$), and a factor ($f \sim 10 \%$) to account for the amount of hydrogen burned before the star undergoes significant evolutionary changes that alter its energy production processes. Therefore, expressing it all together...
> $$t_{\rm nuc} \approx \frac{\eta \, M_{\rm H, burning} \, c^{2}}{L_{*}} \approx \frac{\eta \, (f X M_{*}) \, c^{2}}{L_{*}}$$
> 
> For a [[Units & Conversions#Solar Mass (${ rm M_{ odot}}$)|solar-mass]] star with [[Units & Conversions#Solar Luminosity ($L_{ odot}$)|solar-luminosity]], we find the timescale to be:
> $$t_{\rm nuc} \approx \frac{(0.007) \, (0.1 \times 0.7 \times M_{\odot}) \, c^{2}}{L_{\odot}} \sim 10^{10} \; {\rm year}$$
> 

## Crossing Timescale

$$t_{\rm cross} = \frac{R}{\sigma_{v}} \sim \frac{G N m}{\sigma_{v}^{3}} \hspace{1cm} \text{where} \hspace{1cm} \sigma_{v} \equiv \text{velocity dispersion}$$

The crossing-timescale is defined as the time it roughly takes a star to travel across the scale radius/size of a galaxy.

## Violent Relaxation

Violent relaxation is a process by which a collection of bodies relax/virialize through the collisionless exchange of the gravitational potential, where the total energy of the system remains constant. 

This is the most efficient way for a self-gravitating system, as it is comparable to the [[Timescales#Dynamical Timescale]].

**The General Picture:**
If the potential is time-varying ($\phi(t)$), then "particles" (i.e. stars) can gain or lose energy. Consider the change in specific energy of an individual star.

$$\mathcal{E} = \frac{1}{2} v^{2} + \phi(t) \hspace{1cm} \Rightarrow \hspace{1cm} 
\begin{aligned}[t]
	\frac{\mathrm{d} \mathcal{E}}{\mathrm{d} t} &= \frac{\partial \mathcal{E}}{\partial \vec{v}} \frac{\mathrm{d} \vec{v}}{\mathrm{d} t} + \frac{\partial \mathcal{E}}{\partial \phi} \frac{\mathrm{d} \phi}{\mathrm{d} t} \\
	&= - \vec{v} \, \vec{\nabla} \phi + \frac{\mathrm{d} \phi}{\mathrm{d} t} \\
	&= - \vec{v} \, \vec{\nabla} \phi + \left( \frac{\partial \phi}{\partial t} + \frac{\partial \phi}{\partial \vec{x}} \frac{\mathrm{d} \vec{x}}{\mathrm{d} t} \right) \\
	&= - \vec{v} \, \vec{\nabla} \phi + \frac{\partial \phi}{\partial t} + \vec{v} \, \vec{\nabla} \phi \\
	&= \frac{\partial \phi}{\partial t}
\end{aligned}$$

More intuitively...
- If the potential is constant with time, the particle will recover the same energy as it comes out the other side and there is no relaxation.
- If the potential grows with time, the particle will need to expend more energy to cross the wells, and thus will lose energy. 
- If the potential shrinks with time, the particle will gain energy as it crosses the well.

![[violent-relaxation.png|align:center|500]]

This leads to the spreading out of particle energy distributions. By taking the average across all particles and using the time-dependent virial theorem ([Lynden-Bell 1967](https://articles.adsabs.harvard.edu/pdf/1967MNRAS.136..101L)), we can express the violent relaxation time as the same timescale as the [[Timescales#Dynamical Timescale|dynamical/free-fall timescale]].

$$t_{\rm vr} = \left\langle \frac{\mathcal{E}^{2}}{\left( \frac{\mathrm{d} \mathcal{E}}{\mathrm{d} t} \right)^{2}} \right\rangle^{1/2} \sim \left\langle \frac{\phi^{2}}{\dot{\phi}^{2}} \right\rangle^{1/2} \sim t_{\rm ff}$$

## Two-Body Relaxation
*(Also known as the **Collision Timescale**)*

The **two-body relaxation** is mediated by encounters ("collisions") between two bodies -- typically stars -- that drives the overall system into an equilibrium state by affecting the bodies velocities.

To calculated the frequency of two-body interactions and the associated relaxation timescale, we consider a smooth density field (system of stars) and an incident "subject" star moving into the field from infinity. We now consider a single gravitational scatter.

![[two-body-relaxation.png|align:center|350]]

$$\vec{F} = \frac{G m^{2}}{b^{2} + (v t)^{2}} \; \hat{r} \hspace{1cm} \Rightarrow \hspace{1cm} F_{\perp} = \frac{G m^{2} \cos \theta}{b^{2} + (v t)^{2}} = \frac{G m^{2} b}{\left( b^{2} + (v t)^{2} \right)^{3/2}}$$

By the definition of our relaxation, we are concerned with the change in velocity of the subject star due to the field star. From [[Newton's Laws of Motion#Newton's 2nd Law]]...

$$\vec{F} = m \vec{a} = m \frac{\mathrm{d} v}{\mathrm{d} t} \hspace{1cm} \Rightarrow \hspace{1cm}
\begin{aligned}[t]
	\delta v &= \frac{1}{m} \int_{-\infty}^{+\infty} F_{\perp} \; \mathrm{d} t \\
	\delta v &= \frac{G m}{b^{2}} \int_{-\infty}^{+\infty} \frac{\mathrm{d} t}{\left[ 1 + \left(\frac{v t}{b}\right)^{2} \right]^{3/2}} \\
	\delta v &= \frac{G m}{b v} \int_{-\infty}^{+\infty} \frac{\mathrm{d} s}{\left[ 1 + s^{2} \right]^{3/2}} \\
	\delta v &= \frac{2G m}{b v}
\end{aligned}$$

From this, we can see the change in velocity is roughly equal to the acceleration at the closest approach $(\tfrac{G m}{b^{2}})$ times the duration of the acceleration $(\tau' \sim \frac{2 b}{v})$

> [!note] 
> This calculation is conceptually very similar to [[Question 86]], but instead of using the Coulomb force, we are using the gravitational force.

### Strong Interactions

If the star's change in trajectory involves a change in momentum roughly equal to the original momentum of the star ($v\sim \delta v$), then we regard it as a collision or a "**strong interaction**" and the deflection of the star is $\sim 90 \degree$. The associated impact parameter and cross-section for a strong interaction is then...

$$v \sim \delta v \hspace{1cm} \Rightarrow \hspace{1cm} v \sim \frac{2 G m}{v \, b_{\rm strong}} \hspace{1cm} \Rightarrow \hspace{1cm} b_{\rm strong} \sim \frac{2G m}{v^{2}} \hspace{0.5cm} , \hspace{0.5cm} \sigma_{\rm strong} = \pi b_{\rm strong}^{2}$$

From the [[Virial Theorem]] of the spherical body of field stars...

$$ 2 \left\langle T \right\rangle + \left\langle U \right\rangle =2 \left(\frac{m v^{2}}{2}\right) + \left(\frac{G M m}{R}\right) = 0 \hspace{1cm} \Rightarrow \hspace{1cm} R = \frac{G M}{v^{2}} = \frac{G N m}{v^{2}}\sim \frac{N b_{\rm strong}}{2}$$

...we find that the interaction cross-section (for strong interactions) is very small for large $N$ values. 
$$\sigma_{\rm strong} = \pi b_{\rm strong}^{2} \sim \frac{4 \pi R^{2}}{N^{2}}$$

> [!note]
> With a small interaction cross-section, there is a low probability of these strong interactions occurring in galaxies, whom have $N\sim 10^{11}$. For clusters, these interactions are more often give they have $N \sim 10^{4}$.

The expected number of expected collisions is...

![[strong-interactions.png|align:center|350]]

$$\begin{align}
	\text{\# of collisions} = n \cdot (v t) \cdot \sigma_{\rm strong} &= \left(\frac{3 N}{4 \pi R^{3}}\right) \cdot (v t) \cdot \left( \pi b_{\rm strong}^{2} \right) \\
	\\
	&= \frac{3 N}{4 \pi} \left(\frac{v^{2}}{G N m}\right)^{3} \cdot (v t) \cdot \pi \left(\frac{2 G m}{v^{2}}\right)^{2} \\
	\\
	&=\frac{3 v^{3} t}{G N^{2} m}
\end{align}$$

...such that the relaxation time for strong interactions is then defined as:

$$\boxed{\;t_{\rm strong} = \frac{\rm \#\ of\ collisions}{\rm time} = \frac{G m N^{2}}{3 v^{3}}\;}$$

> [!note]- Similar Approach - Mean Free Path
> 
> If we think about the [[Optical Depth#Mean Free Path]] ($l$) of the system, then can define the relaxation time in a very similar way.
> $$l \equiv \frac{1}{n \left( \pi b_{\rm strong}^{2} \right)} \hspace{1cm} \Rightarrow \hspace{1cm} 
> \begin{aligned}[t]
> 	t_{\rm strong} = \frac{l}{v} &= \frac{1}{n \left( \pi b_{\rm strong}^{2} \right) v} \\
> 	&= \frac{4 \pi R^{3}}{3 N} \cdot \frac{N^{2}}{4 \pi R^{2}} \cdot \frac{1}{v} \\
> 	&= \frac{N R}{3 v} \\
> 	&= \frac{G m N^{2}}{3 v^{3}} \\
> \end{aligned}$$
> $$t_{\rm strong} = \frac{G m N^{2}}{3 v^{3}}$$

> [!math] Comparison to [[#Crossing Timescale]]
> 
> $$t_{\rm strong} \approx \frac{G m N^{2}}{3 v^{3}} \hspace{1.5cm} t_{\rm cross} \approx \frac{G N m}{v^{3}} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{t_{\rm strong} \sim N t_{\rm cross}}$$

> [!space]- For Different Astronomical Objects
> 
> - Stellar Cluster: $t_{\rm strong} \sim 14 \; {\rm Gyr}$ (similar age to the universe)
> 	- $m \sim M_{\odot}$
> 	- $N \sim 10^{5}$
> 	- $\sigma_{v} = v = 10 \; {\rm km/s}$
>
> - Elliptical Galaxy: $t_{\rm strong} \sim 10^{10} \; {\rm Gyr}$ (way too long $\implies$ [[#Violent Relaxation]]).
> 	- $m \sim M_{\odot}$ 
> 	- $N \sim 10^{11}$
> 	- $\sigma_{v} = v = 100 \; {\rm km/s}$
> 

### Weak Interactions

Instead of the star's trajectory changing dramatically due to a single interaction, we can also consider the summation of "**weak interactions**" as it progresses through the field ($\sum \delta v$). 

![[weak-interactions.png|align:center|350]]

![[weak-interactions_propagation.png|align:center|400]]

We assume the star will undergo small velocities kicks in a random walk, such that cumulative $\delta v$ is zero, but the square of the velocity changes is nonzero.

$$\begin{align}
	(\delta v )^{2} = \sum_{i}^{N} \left( \delta v_{i} \right)^{2} &= \int_{b_{\rm min}}^{b_{\rm max}} \underbrace{\left[ \, (2 \pi b \; \mathrm{d} b) \times (v t) \times n \, \right]}_{\text{\# of encounters within $\mathrm{d} b$}} \times \underbrace{\left[ \left(\frac{2 G m}{bv}\right)^{2} \right]}_{\delta v \text{ for each encounter}} \\
	&= \left(\frac{8 \pi G^{2} m^{2} n \,t}{v}\right) \int_{b_{\rm min}}^{b_{\rm max}} \frac{\mathrm{d} b}{b} \\
	&= \left(\frac{8 \pi G^{2} m^{2} n \,t}{v}\right) \ln \left(\frac{b_{\rm max}}{b_{\rm min}}\right)
\end{align}$$

The bounds for this integration come from the size of the field ($b_{\rm max} \approx R$) and the impact parameter for a strong interaction ($b_{\rm min} \approx b_{\rm strong} = 2R/N$). 

The relaxation time for weak interactions is then:

$$(\delta v )^{2} \approx \left(\frac{8 \pi G^{2} m^{2} n \,t}{v}\right) \ln \left(\frac{N}{2}\right) \sim \left(\frac{8 \pi G^{2} m^{2} n \,t}{v}\right) \ln N \hspace{1cm} \text{where} \hspace{1cm} N \gg 2$$
$$v^{2} \sim (\delta v)^{2} \hspace{1cm} \Rightarrow \hspace{1cm} t_{\rm weak} \approx \left(\frac{v^{3}}{8 \pi G^{2} m^{2} n}\right) \frac{1}{\ln N}$$

> [!math] Comparison to [[#Crossing Timescale]]
> 
> If we take the velocity of the subject star to be comparable to the velocity dispersion of the field, then we can apply the [[Virial Theorem]] to the velocity.
> 
> $$\begin{align}
> 	\frac{t_{\rm weak}}{t_{\rm cross}} &\approx \left[ \left(\frac{v^{3}}{8 \pi G^{2} m^{2} n}\right) \frac{1}{\ln N} \right] \cdot \left[ \frac{v}{R} \right] \\
> 	t_{\rm weak} &\approx \left[ \left(\frac{1}{8 \pi G^{2} m^{2}}\right) \left(\frac{v^{4}}{n R}\right) \frac{1}{\ln N} \right] \cdot t_{\rm cross} \\
> 	t_{\rm weak} &\approx \left[ \left(\frac{1}{8 \pi G^{2} m^{2}}\right) \left(\frac{G N m}{R}\right)^{2} \left(\frac{4 \pi R^{3}}{3 N}\right) \left(\frac{1}{R}\right) \frac{1}{\ln N} \right] \cdot t_{\rm cross} \\
> 	t_{\rm weak} &\approx \left[ \frac{N}{6 \ln N} \right] \cdot t_{\rm cross} \\
> \end{align}$$
> $$\boxed{\; t_{\rm weak} \approx \left(\frac{N}{6 \ln N}\right) \left(\frac{G N m}{v^{3}}\right) \approx \left(\frac{N}{6 \ln N}\right) \; t_{\rm cross} \;}$$

> [!space]- For Different Astronomical Objects
> 
> - Stellar Cluster: $t_{\rm weak} \sim 0.6 \; {\rm Gyr}$
> 	- $m \sim M_{\odot}$
> 	- $N \sim 10^{5}$
> 	- $\sigma_{v} = v = 10 \; {\rm km/s}$
>
> - Elliptical Galaxy: $t_{\rm weak} \sim 10^{8} \; {\rm Gyr}$ (way too long $\implies$ [[#Violent Relaxation]])
> 	- $m \sim M_{\odot}$ 
> 	- $N \sim 10^{11}$
> 	- $\sigma_{v} = v = 100 \; {\rm km/s}$

## Hubble Time

The Hubble time is the age of the universe assuming that it has expanded at a constant rate since the beginning of time. This rate of expansion is the [[#Hubble Law|Hubble flow]] we measure today with $H_{0}$.

$$d = v \, t_{\rm H} = (H_{0} \, d) \,t_{H} \hspace{1cm} \Rightarrow \hspace{1cm} t_{H} = \frac{1}{H_{0}} \sim 14 \; {\rm Gyr} \quad \text{for} \quad H_{0} = 70 \; \pu{km s^{-1} Mpc^{-1}}$$

## Cooling Time
*(See [[Question 84]] for cooling function. Also a good source [here](http://www.astro.yale.edu/vdbosch/astro610_lecture15.pdf))*

The **cooling timescale** is the time it takes the gas to radiate away its internal energy.

$$t_{\rm cool} \equiv \frac{\varepsilon}{\mathcal{C}} = \frac{\varepsilon}{n^{2} \, \Lambda(T)} \propto \frac{k_{\rm B} T}{n \Lambda (T)} \hspace{1cm} \text{where} \hspace{1cm} \varepsilon = \left(\frac{d}{2}\right) nk_{\rm B} T =\text{energy of ideal gas}$$

Based on how the cooling time scales with density ($t_{\rm cool} \propto n^{-1} \propto \rho^{-1}$), denser mediums cool faster.

> [!math] Comparison to the [[#Hubble Time]] and [[#Dynamical Timescale]]
> 
> When considering a gas cloud collapsing, we can compare the Hubble time at $z$ (in a  matter-dominated universe, $\Omega_{M}=1$) and the free-fall timescale for a halo with 200 times the [[Friedmann Equation#Critical Density|critical density]] (in association with [[Dark Matter#CDM]]).
> 
> $$\begin{alignat}{3}
> 	t_{H} &= \frac{1}{H(z)} \propto \frac{1}{\sqrt{G \bar{\rho}}} &&\hspace{1cm} \text{where} \hspace{1cm} \bar{\rho} &&= \Omega_{M} \, \rho_{\rm crit} =  \rho_{\rm crit} \\
> 	t_{\rm ff} &\propto \frac{1}{\sqrt{G \bar{\rho}_{\rm vir}}} &&\hspace{1cm} \text{where} \hspace{1cm} \bar{\rho}_{\rm vir} &&= \rho_{200} = 200 \rho_{\rm crit}
> \end{alignat}$$
> $$t_{\rm ff} \sim \frac{t_{H}}{10}$$
> 
> This yields three regimes, depending on how long the cooling timescale is.
> 
> - $t_{\rm cool} > t_{H} \implies$ Cooling is not important. 
> 	- Gas is in hydrostatic equilibrium, unless it was recently disturbed.
> -  $t_{\rm ff} < t_{\rm cool} < t_{H} \implies$ System evolves on the cooling timescale. 
> 	- Gas contracts slowly as it cools in a quasi-hydrostatic equilibrium, but the system has sufficient time to continue to re-establish hydrostatic equilibrium.
> -  $t_{\rm cool} < t_{\rm ff} \implies$ Cooling is catastrophic. 
> 	- Gas cannot respond fast enough to loss of pressure. Since cooling time decreases with increasing density, cooling proceeds faster and faster (i.e. catastrophic). Gas falls to center of dynamic system on free-fall time.
> 
> We can go a step further and see that cooling is general more efficent at higher redshifts.
> $$\begin{alignat}{2}
> 	t_{\rm cool} &\propto \rho &&\propto (1+z)^{-3} \\
> 	t_{\rm ff} &\propto \rho &&\propto (1+z)^{-3/2}
> \end{alignat}$$
