### Question
---
Give a qualitative description of the frequency and amplitude evolution of the gravitational wave signal from a binary compact star system. Compute actual numbers for a $30 \; {\rm M_{\odot}} - 30 \; {\rm M_{\odot}}$ binary black hole system.

### Answer
---
##### Give a qualitative description of the frequency and amplitude evolution of the gravitational wave signal from a binary compact star system.

> [!note]- Conceptual Background: Flat Spacetime with a Perturbation
> *(Sources: [[GW_wheeler.pdf]], [[GW-Theory.pdf]])*
> 
> Conceptually, gravitational fields ($g_{\mu nu}$) can be represented by Minkowski/flat spacetime ($\eta_{\mu \nu}$) with some metric perturbation ($h_{\mu \nu}$) that satisfies the wave equation.
> 
> $$g_{\mu \nu} = \eta_{\mu \nu} + h_{\mu \mu} \hWhere \left| h_{\mu \nu} \right| \ll 1 \hspace{0.5cm} , \hspace{0.5cm} \square^{2} h_{\mu \nu} \equiv \underbrace{\left( \nabla^{2} + \pdd{}{t} \right) h_{\mu \nu} = 0}_{\rm wave\ equation}$$
> 
> The perturbation can be represented by a traceless transform (TT) gauge composed of different contributions in polarization orientations.
> 
> $$
> h_{\mu \nu} \equiv A_{\mu \nu} \exp \left( i k_{\rho} k^{\rho} \right) \hWhere A_{\mu \nu} \equiv 
> \begin{bmatrix}
> 0 &0 &0 &0 \\
> 0 & a_{+} & a_{\times} & 0 \\
> 0 & a_{+} & a_{\times} & 0 \\
> 0 &0 &0 &0
> \end{bmatrix}
> \hspace{1cm}
> \begin{aligned}
> 	a_{+} &\equiv \text{plus polarization} \\
> 	a_{\times} &\equiv \text{cross polarization}
> \end{aligned}
> $$
>
> After some GR derivation, we can express the radiation from gravitational waves as:
> $$L_{\rm GW} \equiv \td{{E}_{\rm GW}}{t} = \frac{G}{5 c^{5}} \expval{\dddot{Q} \; \dddot{Q}} \hWhere Q \equiv I_{ij} = \text{moment of inertia tensor}$$
> 
> The scaling amplitude ($h_{0}$) of the gravitational waves can then be defined as...
> 
> $$h_{0}^{2} \equiv \left| h_{\mu \nu} \right|^{2} = h^{\mu \nu} h_{\mu \nu} = \expval{a_{+}^{2}} + \expval{a_{\times}^{2}}$$
> 
> ...where $h(t) = h_{0} \cos \phi(t) = h_{0} \cos \left( 2 \omega t + \dot{\omega} t^{2} + \phi_{0} \right)$
> 
> *(Note: $\omega = \pi f \equiv$ orbital frequency and $f \equiv$ gravitational wave frequency.)*
> 
^conceptual-bkgd

Since energy and angular momentum are continuously carried away by [[Gravitational Waves#Gravitational Radiation|gravitational radiation]] *(See the [[Gravitational Waves#Sticky Bead Argument]])*, as the two orbiting masses spiral towards each other over time, their orbital frequency $\omega$ increases. Furthermore, the [[Gravitational Waves|GW]] frequency $(f = \omega / \pi)$ and the [[Gravitational Waves|GW]] scaling amplitude ($h_{0}$) are also increasing functions of time. 


**GW Frequency:**
The orbital frequency (and thus the GW frequency) of a binary system can be calculated from Newtonian mechanics.

At coalescence, we can simply use [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] and define the orbital separation as the sum of the radii of the two binary objects. Since Newtonian mechanics breaks down near the compact objects, we use their ISCO radius for coalescence (Maggorie, pg 174).

$$a_{\rm c} = R_{1}^{\rm ISCO} + R_{2}^{\rm ISCO} = \frac{6 \, G M}{c^{2}} \hRightarrow \omega_{\rm c} = \sqrt{\frac{G M}{a_{c}^{3}}} = \frac{c^{3}}{(6)^{3/2} \, G M}$$

For a time-dependent frequency expression (prior to coalescence), we compare the gravitational radiation ($L_{\rm GW}$) to the change in orbital energy of a binary ($\dot{E}_{\rm orb}$). This yields...
$$\dot{\omega} = \td{\omega}{t} \simeq \frac{96}{5 c^{5}} \left( G M_{\rm c} \right)^{5/3} \; \omega^{11/3} \hRightarrow \omega(t) = \fpar{256 (G M_{\rm c})^{5/3}}{5 c^{5}}^{-3/8} \left( t_{\rm c} - t \right)^{-3/8}$$
$$\boxed{ \; f \; \propto \; \omega \; \propto \; \left( t_{\rm c} - t \right)^{-3/8} \; }$$

where $M_{\rm c} = \mu^{3/5} M^{2/5} \equiv$ [[Gravitational Waves#Chirp Mass|chirp mass]] and $t_{\rm c} \equiv$ the coalescence time. We can see that after the coalescence time, the expression diverges.

> [!derivation]- Frequency Time-Dependence - Newtonian Derivation
> 
> The frequency of the gravitational waves can be found by comparing the gravitational wave radiation and to the change to gravitational potential energy.
> 
> Beginning with the moment of inertia tensor ($I_{ij}$), we can take the third time derivative and apply it to the GW radiation equation ($L_{\rm GW}$), where we apply [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] to the orbital separation ($a$):
> 
> $$\textcolor{gray}{\left[ \; \text{Kepler's 3rd Law: } \quad \frac{a^{3}}{P^{2}} = \frac{G M}{4 \pi^{2}} \hRightarrow a = \fpar{G M}{\omega^{2}}^{1/3} \hspace{1cm} \dot{a} = - \frac{2 (G M)^{1/3} \dot{\omega}}{3 \,\omega^{5/3}} \; \right]}$$
>
> $$
> I_{ij} = \frac{1}{2} \mu a^{2} \begin{bmatrix} 1 + \cos 2 \omega t & \sin 2 \omega t & 0 \\ \sin 2 \omega t & 1 - \cos 2 \omega t & 0  \\ 0 & 0 & 0 \end{bmatrix} 
> \hTherefore 
> \dddot{I}_{ij} = 4 \mu a^{2} \omega^{3} \begin{bmatrix} \sin 2 \omega t & -\cos 2 \omega t & 0 \\ -\cos 2 \omega t & -\sin 2 \omega t & 0  \\ 0 & 0 & 0 \end{bmatrix}$$
> $$\Downarrow$$
> $$L_{\rm GW} = \frac{G}{5 c^{5}} \; \expval{\dddot{I}^{\ ij} \; \dddot{I}_{ij}}  = \frac{G}{5 c^{5}} \; \expval{ 32 \mu^{2} a^{4} \omega^{6} }
> \begin{aligned}[t]
> 	&= \frac{32 G \mu^{2} \omega^{6} a^{4}}{5 c^{5}} \\
> 	&= \frac{32 G \mu^{2} \omega^{6}}{5 c^{5}} \fpar{G M}{\omega^{2}}^{4/3} \\
> 	&= \frac{32 G^{7/3}}{5 c^{5}} (M_{\rm c} \, \omega)^{10/3}
> \end{aligned}$$
> 
> For the change in gravitational potential energy, we take the time derivative of the [[Kepler's Laws of Planetary Motion#Conservation of Energy|Keplerian Energy of a binary]] (and apply [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] again).
> 
> $$
> E_{\rm orb} = \frac{G M \mu}{2 a} \hRightarrow 
> \begin{aligned}[t]
> 	L_{\rm orb} \equiv \td{E_{\rm orb}}{t} &= \frac{G M \mu \dot{a}}{2 a^{2}} \\
> 	&= - \frac{G M \mu \dot{a}}{2 a^{2}} \\
> 	&= - \frac{G M \mu}{2} \left( - \frac{2 (G M)^{1/3} \dot{\omega}}{3 \,\omega^{5/3}} \right) \fpar{\omega^{2}}{G M}^{2/3} \\
> 	&= \frac{(G M)^{2/3} \mu}{3} \fpar{ \dot{\omega}}{\omega^{1/3}} \\
> \end{aligned}
> $$
> 
> Setting them equal to each other...
> 
> $$L_{\rm GW} = L_{\rm orb} \hRightarrow \frac{32 G \mu^{2} \omega^{6}}{5 c^{5}} \fpar{G M}{\omega^{2}}^{4/3} = \frac{(G M)^{2/3} \mu}{3} \fpar{\dot{\omega}}{\omega^{1/3}}$$
> $$\dot{\omega} = \frac{96 G^{5/3}}{5 c^{5}} \left( \mu M^{2/3} \right) \; \omega^{11/3}$$
> 
> ...we can define the [[Gravitational Waves#Chirp Mass]] ($M_{\rm c} \equiv \mu^{3/5} M^{2/5}$) and the "chirp" ($\dot{\omega}$).
> 
> $$\dot{\omega} = \frac{96}{5 c^{5}} \left( G M_{\rm c} \right)^{5/3} \; \omega^{11/3}$$
> 
> Integrating via the separation of variables, the time-dependence of the orbital frequency can be expressed up to the time of coalescence ($t_{\rm c}$).
> 
> $$\int_{\omega}^{\infty} \frac{\rd \omega}{\omega^{11/3}} \; \propto \; \int_{t}^{t_{\rm c}} \rd t \hRightarrow \omega(t) = \fpar{256 (G M_{\rm c})^{5/3}}{5 c^{5}}^{-3/8} {\underbrace{\left( t_{\rm c} - t \right)}_{\equiv \; \delta t_{\rm c}}}^{-3/8}$$
> $$\boxed{ \; \omega \; \propto \; \left( t_{\rm c} - t \right)^{-3/8} \; }$$
> 
> We can see from this that when the binary object coalesce, the frequency ($\omega$) formally goes to infinity, such that after the coalescence, the frequency is non-physical because the two objects have become one.
^freq-dependence

**Scaling Amplitude:**
The scaling amplitude ($h_{0}$) of a GW at a distance ($R$) from the source is composed of two polarization states ($a_{+}$ and $a_{\times}$). *(see [[#^conceptual-bkgd|Conceptual Background]])*

$$h_{0}^{2} \equiv \left| h_{\mu \nu} \right|^{2} = h_{\mu \nu} \, h^{\mu \nu} = \expval{a_{+}^{2}} + \expval{a_{\times}^{2}}$$
$$\textcolor{gray}{\text{where} \hspace{1cm} h(t) = h_{0} \cos \phi(t) = h_{0} \cos \left( 2 \omega t + \dot{\omega} t^{2} + \phi_{0} \right)}$$

This scalar quantity represents the overall growth in amplitude, and it can be found through dimensional analysis of the GW flux. *(The $(1/2\pi)$ comes from GR)*

$$F_{\rm GW} \simeq \frac{1}{2 \pi} \fpar{h_{0}^{2} \omega^{2} c^{3}}{G} \hRightarrow \frac{L_{\rm GW}}{4 \pi R^{2}} \simeq \frac{1}{2 \pi} \fpar{h_{0}^{2} \omega^{2} c^{3}}{G}$$
$$h_{0} \simeq \sqrt{\frac{G L_{\rm GW}}{2 R^{2} \omega^{2} c^{3}}} \quad \simeq \fpar{4}{\sqrt{5} c^{4}} \frac{(G M_{\rm c})^{5/3}\omega^{2/3}}{R}$$
$$\boxed{\;h_{0} \; \propto \; R^{-1} \;} \hspace{2cm} \boxed{\; h_{0} \; \propto \; \omega^{2/3} \; \propto \; \left( t_{\rm c} - t \right)^{-1/4} \;}$$

Similar to the frequency, the expression diverges after the coalescence. Furthermore, we can also identify that the amplitude scales inversely with the distance to the source.

> [!derivation]- Scaling Amplitude Time-Dependence - Dimensional Analysis Derivation
> 
> For the amplitude of the gravitational waves, we can use dimensional analysis to define the GW flux ($F_{\rm GW}$) for a binary system at distance ($R$) away form the observer, with frequency ($\omega$) and strain ($h$). From GR, we can take the coefficient to be $1/2\pi$.
> 
> $$F_{\rm GW} \simeq \frac{1}{2 \pi} \fpar{h_{0}^{2} \omega^{2} c^{3}}{G}$$
> 
> Then, we can relate the GW flux ($F_{\rm GW}$) to the GW radiation ($L_{\rm GW}$) to find the time-dependence, assuming an isotropic emission.
> 
> $$
> F_{\rm GW} \simeq \frac{L_{\rm GW}}{4 \pi R^{2}}
> \hRightarrow
> \begin{aligned}[t]
> 	\frac{1}{2 \pi} \fpar{h_{0}^{2} \omega^{2} c^{3}}{G} &\simeq \frac{1}{4 \pi R^{2}} \left( \frac{32 G \mu^{2} \omega^{6}}{5 c^{5}} \fpar{G M}{\omega^{2}}^{4/3} \right) \\
> 	h_{0}^{2} &\simeq \frac{1}{2 R^{2}} \fpar{G}{\omega^{2} c^{3}} \left( \frac{32 G \mu^{2} \omega^{6}}{5 c^{5}} \fpar{G M}{\omega^{2}}^{4/3} \right) \\
> 	h_{0}^{2} &\simeq \fpar{16}{5 c^{8}} \frac{(G M_{\rm c})^{10/3} {\omega}^{4/3}}{R^{2}} \\
> 	h_{0} \;&\simeq \fpar{4}{\sqrt{5} c^{4}} \frac{(G M_{\rm c})^{5/3}\omega^{2/3}}{R}
> \end{aligned}
> $$
> $$\boxed{\;h_{0} \; \propto \; \frac{\omega^{2/3}}{R} \;} \hRightarrow \boxed{\; h_{0} \; \propto \; \left( t_{\rm c} - t \right)^{-1/4} \;}$$
> 
> Similar to the frequency ($\omega$), we see that as the binary object coalesce, the amplitude of the GW ($h_{0}$) also formally goes to infinity, such that after the coalescence, the frequency is non-physical because the two objects have become one.
^amp-dependence

**Overall Evolution:**
Bringing these together, we can see this behavior reflected in the observed waveforms. As the binary "inspirals", the amplitude of the wave peaks increases while their wavelength decreases (frequency increases). This climaxes at the coalescence time ($t_{\rm c}$), after which there is a period of "ring down" as the two bodies reach an equilibrium state. Though they have merged, there are enough asymmetries that gravitational radiation can still be emitted. That said, this ring down is very hard to observe.
![[GW_timedependence.png|align:center|550]]![[GW_strain.png|align:center|400]]

##### Compute actual numbers for a $30 \; {\rm M_{\odot}} - 30 \; {\rm M_{\odot}}$ binary black hole system.

We will assume that the [[Black Hole|black holes]] coalesce at the [[Black Hole#Innermost Stable Circular Orbit (ISCO)]]. Using the coalescence orbital frequency ($\omega_{\rm c}$) expression we derived above from [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]], with $M \equiv$ total mass...

$$\omega_{\rm c} = \sqrt{\frac{G M}{a_{c}^{3}}} = \frac{c^{3}}{(6)^{3/2} \, G M} \simeq 230 \; {\rm rad \, s^{-1}} \hRightarrow \boxed{ \; f_{\rm c} = \frac{\omega_{\rm c}}{\pi} \simeq 70 \; {\rm Hz} \; }$$

For the scaling amplitude of the strain ($h_{0}$), we need to know the distance to the merger.

$$h_{0} \simeq \fpar{4}{\sqrt{5} c^{4}} \frac{(G M_{\rm c})^{5/3}\omega^{2/3}}{R} \hRightarrow h_{0} \propto \frac{1}{R}$$

Without this knowledge, we cannot get an explicit value. That said, if we calculate the luminosity of the coalescence, then we can compare to similar previously-observed events and get an approximation for the [[Distances#Luminosity Distance|luminosity distance]], and thus, the scaling amplitude.

$$M_{\rm c} \simeq 26.12 \; {\rm M_{\odot}} \hRightarrow L_{\rm GW} = \left[ \frac{32 G^{7/3}}{5 c^{5}} (M_{\rm c} \, \omega)^{10/3} \right] \sim 10^{48} \; {\rm W} \sim 10^{21} \; {\rm L_{\odot}}$$

Based on the scaling of the above expressions, we can see...
- $\omega_{\rm c} \propto M^{-1}$ : more massive objects have lower coalescence frequencies
- $h_{0} \propto R^{-1}$ : closer objects are easier to observe
