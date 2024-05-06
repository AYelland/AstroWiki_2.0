### Question
---
Derive a plausible relation between the luminosity of an X-ray pulsar and its spin-up rate. How would you calculate the magnetospheric radius of an accreting neutron star?

### Answer
---
*(It seems to make more sense to do this problem in the reverse order...)*


![[NS_pulsar_accretion_lightCylinder.png|align:center|500]]

> [!note] Recall that...
> - Isolated [[Neutron Star#Pulsar|pulsars]] are powered by magnetic dipole radiation, such that they lose rotational energy over time and spin down (without an accreting companion).
> - Accreting [[Neutron Star#Pulsar|pulsars]] gather matter and angular momentum from the donor, companion star, spinning up and releasing gravitational potential energy through x-ray emission.

##### How would you calculate the magnetospheric radius of an accreting neutron star?
*(See Bradley-Ostlie, 2nd Edition, Chp. 18.6, pg 692)*

The **magnetospheric radius** ($R_{\rm M}$) for a [[Neutron Star#Pulsar|pulsar]] is where the magnetic pressure (i.e. magnetic energy density) from the [[Neutron Star|NS]] magnetic field is balanced with the external [[Fluid Mechanics#Ram Pressure|ram pressure]] of the surrounding gas in the accretion disk. 

To find an expression for this value at the boundary ($r = R_{\rm M}$), we can assume the surrounding gas is falling in on the [[Timescales#Dynamical Timescale|dynamical timescale (freefall)]]...

$$P_{\rm ram} = \rho \,v_{\rm dyn}^{2} = \frac{\dot{M}\sqrt{2 G M}}{4 \pi R_{\rm M}^{5/2}}$$
$$\textcolor{gray}{\left[ \hspace{0.5cm}
\rho = \underbrace{\fpar{\dot{M}}{4 \pi R_{\rm M}^{2}\; v_{\rm dyn}}}_{\rm mass\ continuity}
\hspace{2cm}
v_{\rm dyn} = \sqrt{\frac{2 G M}{R_{\rm M}}}
\hspace{0.5cm} \right]}$$

...and the magnetic field acts as a dipole with a constant dipole moment $|m|$. 

$$P_{\rm mag} = \frac{B_{\rm M}^{2}}{2 \mu_{0}} = \frac{1}{2 \mu_{0}} \fpar{\mu_{0} m}{2 \pi R_{\rm M}^{3}}^{2} = \frac{\mu_{0} m^{2}}{8 \pi^{2} R_{\rm M}^{6}}$$
$$
\textcolor{gray}{\left[ \;
B_{*} = \pm \frac{\mu_{0} m}{2 \pi R_{*}^{3}}
\hspace{0.5cm} , \hspace{0.5cm}
B_{*} R_{*}^{3} = B_{\rm M} R_{\rm M}^{3}
\hRightarrow
B_{\rm M} = B_{*} \fpar{R_{*}}{R_{\rm M}}^{3} = \pm \frac{\mu_{0} m}{2 \pi R_{\rm M}^{3}} 
\; \right]}
$$

Balancing the pressures...

$$
P_{\rm ram} = P_{\rm mag}
\hRightarrow
\frac{\dot{M}\sqrt{2 G M}}{4 \pi R_{\rm M}^{5/2}} = \frac{\mu_{0} m^{2}}{8 \pi^{2} R_{\rm M}^{6}}
\hRightarrow
\begin{aligned}[t]
	R_{\rm M}^{7/2} &\propto \fpar{4 \pi}{\dot{M} \sqrt{2 G M}} \fpar{\mu_{0} m^{2}}{8 \pi^{2}} \\
	R_{\rm M} &\propto \fpar{\mu_{0} m^{2}}{2 \pi \dot{M} \sqrt{2 G M}}^{2/7} \\
	R_{\rm M} &\propto \fpar{\mu_{0}^{2} m^{4}}{8 \pi^{2} G M \dot{M}^{2}}^{1/7}
\end{aligned}

$$

...we can then show how the magnetospheric radius is dependent on the accretion power ([[Luminosity|luminosity]]) derived in [[Question 54]].

$$
\textcolor{gray}{\left[ L_{\rm acc} = \frac{G M \dot{M}}{2 R} \quad \implies \quad \dot{M} = \fpar{2 R}{G M} L_{\rm acc} \right]}
\hspace{2cm}
\begin{aligned}[t]
	R_{\rm M} &\propto \left( \frac{\mu_{0}^{2} m^{4}}{8 \pi^{2} G M} \fpar{G M}{2 R L_{\rm acc}}^{2} \right)^{1/7} \\
	R_{\rm M} &\propto \left( \frac{\mu_{0}^{2} m^{4}}{32 \pi^{2}} \fpar{G M}{R^{2}} \right)^{1/7} L_{\rm acc}^{-2/7}
\end{aligned}
$$
$$\boxed{R_{\rm M} \propto L_{\rm acc}^{-2/7}}$$

From this, we can see that if $r < R_{\rm M}$, then the motion of the surrounding gas will dominate. And if $r > R_{\rm M}$, then the magnetic field will dominate the motion.

##### Derive a plausible relation between the luminosity of an X-ray pulsar and its spin-up rate. 

To calculate the relationship between [[Luminosity|luminosity]] or [[Question 54|accretion power]] ($L \equiv L_{\rm acc}$) and the spin-up rate ($\dot{P}$), we use the *Conservation of Angular Momentum* between accretion disk and the pulsar.

For the accretion disk, we assume that within the magnetosphere ($r < R_{\rm M}$), it is truncated and negligible. Beyond the edge of the magnetospheric radius ($r \ge R_{\rm M}$), the accretion disk has a circular orbit with constant angular velocity, equal to the spin of the pulsar ($\Omega \equiv \Omega_{\rm disk} \equiv \Omega_{\rm pulsar}$) .

The angular momentum ($\ell$) and the torque ($\tau$) of the disk and pulsar can then be written as...

$$
\begin{alignat}{2}
	&\text{For the Pulsar:} &\hspace{2cm} &\ell_{\rm pulsar} &&= I \Omega &\hRightarrow &\tau_{\rm pulsar} &&= \dot{\ell}_{\rm pulsar} &&= I \dot{\Omega} \\
	&\text{For the Disk:} &\hspace{2cm} &\ell_{\rm disk} &&= m \Omega r^{2} &\hRightarrow &\tau_{\rm disk} &&= \dot{\ell}_{\rm disk} &&= \dot{m} \Omega r^{2}
\end{alignat}
$$

...where $I \equiv$ moment of inertia $\propto M R^{2}$.

Using the circular orbit approximation and mass conservation laws, we can evaluate the angular momentum conservation at the boundary ($r = R_{\rm M}$)...

$$
\begin{align}
	\tau_{\rm pulsar} + \tau_{\rm disk} &= 0 \\
	I \dot{\Omega} + \dot{m} \Omega r^{2} &= 0
		\hspace{1cm} \textcolor{gray}{\left[ \; \dot{m} = - \dot{M} \; \right]} \\
	M R^{2} \dot{\Omega} - \dot{M} r (\Omega r) &\propto 0 
		\hspace{1cm} \textcolor{gray}{\left[ \; v_{\rm r} \equiv \Omega r = \sqrt{\tfrac{G M}{r}} \; \right]} \\
	M R^{2} \dot{\Omega} - \dot{M} \sqrt{G M r} &\propto 0
		\hspace{1cm} \textcolor{gray}{\left[ \; r = R_{\rm M} \; \right]} \\
	M R^{2} \dot{\Omega} - \dot{M} \sqrt{G M R_{\rm M}} &\propto 0 \\
	\\
	\dot{\Omega} &\propto \frac{\dot{M}}{R^{2}} \sqrt{\frac{G R_{\rm M}}{M}} \textcolor{gray}{\quad \propto - \frac{\dot{P}}{P^{2}}} \\
	\\
	\dot{P} &\propto \left( - \frac{P^{2}}{R^{2}} \sqrt{\frac{G}{M}} \right) \; \dot{M} R_{\rm M}^{1/2}
\end{align}
$$

Comparing to the the [[Question 54|accretion power]] we can identify the relationship between the spin-up rate and the luminosity.

 $$
\begin{aligned}[t]
	\textcolor{gray}{\left[ L_{\rm acc} = \frac{G M \dot{M}}{2 R} \quad \implies \quad \dot{M} = \fpar{2 R}{G M} L_{\rm acc} \right]} \hspace{2cm}
		&\dot{P} \propto \dot{M} R_{\rm M}^{1/2} \\
	\textcolor{gray}{\left[ R_{\rm M} \propto \left( \frac{G M \mu_{0}^{2} m^{4}}{32 \pi^{2}R^{2}} \right)^{1/7} L_{\rm acc}^{-2/7} \quad \implies \quad R_{\rm M} \propto L_{\rm acc}^{-2/7} \right]} \hspace{2cm}
		&\dot{P} \propto \Big( L_{\rm acc} \Big) \; \Big( L_{\rm acc}^{-2/7} \Big)^{1/2}
\end{aligned}
$$
$$\boxed{ \; \dot{P} \; \propto \; L_{\rm acc}^{6/7} \; }$$

