### Question
---
What is the Shakura-Sunyaev (alpha-disk) model for accretion disks? What are the assumptions that go into its derivation?

### Answer
---
##### What is the Shakura-Sunyaev (alpha-disk) model for accretion disks? 

In accreting sources, the conservation of angular momentum causes the accreting matter to form a disk-like structure. In order accrete onto the central object, the matter in the disk must lose angular momentum. This loss in energy causes the mass to be transferred inwards and a commensurate increase in angular momentum to be transferred outwards. 

*That is, for accretion to occur, angular momentum must be transferred from inner parts of the disk to the outer parts of the disk.*

$$\ell  = v r = r^{2} \Omega = \sqrt{G M r} \hspace{1cm} \Rightarrow \hspace{1cm} \substack{\text{leads to spreading} \\ \text{the accretion material into a ring}}$$

The mechanism for this transport is the viscosity, but phenomenologically, we need turbulence-enhanced viscosity to explain what we see. However, the microphysics is not understood and is an active area of research.

The **$\mathbf{\alpha}$-disk model** is a steady-state model for a geometrically thin accretion disk with constant mass transfer ($\dot{M}$) that is parameterized by a single parameter ($\alpha$) that encodes our ignorance of the viscosity microphysics.

$$
\nu = \alpha c_{\rm s} H 
\hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}
	\nu &\equiv \text{disk visocity} \\
	\alpha &\equiv \text{parameter} \in \left[ 0, \, 1 \right]\\
	c_{\rm s} &\equiv \text{speed of sound} \\
	H &\equiv \text{scale height}
\end{aligned}
$$

> [!note]- Viscosity is Scaled with Pressure
> 
> The viscous shear stress (force in $\varphi$ direction, per unit area in $r$ direction) is directly proportional to pressure.
> $$
> \begin{align}
> 	\left| T_{r\varphi} \right| &= \rho \nu r \left| \frac{\mathrm{d} \Omega}{\mathrm{d} r} \right| \\
> 	&= \rho \nu r \left| \frac{\mathrm{d} }{\mathrm{d} r} \left( \sqrt{ \frac{G M}{r^{3/2}}} \right) \right| \\
> 	&= \frac{3 \rho \nu r \sqrt{G M}}{2 r^{5/2}} \\
> 	&= \frac{3}{2} \rho \nu \Omega
> \end{align}
> $$
> Combining with the vertical pressure balance...
> $$\frac{\mathrm{d} P}{\mathrm{d} z} = - \Omega^{2} z \rho$$
> $$\int_{P}^{0} \mathrm{d} P = \int_{0}^{H} - \Omega^{2} z \rho \; \mathrm{d} z \hspace{1cm} \Rightarrow \hspace{1cm} H = \sqrt{\frac{2 P}{\rho \Omega^{2}}} \sim \frac{c_{\rm s}}{\Omega}$$
> ...and the pressure of an ideal gas...
> $$P = c_{\rm s}^{2} \rho$$
> ...we can express the shear stress in terms of pressure.
> $$\left| T_{r\varphi} \right| \sim \frac{3}{2} \left(\frac{P}{c_{\rm s}^{2}}\right) \left( \alpha c_{\rm s} H \right) \left(\frac{c_{\rm s}}{H}\right) \sim \frac{3}{2} \alpha P \sim \alpha' P$$

For this model, there are 6 governing equations:
1) *Conservation of Mass* $$\dot{M} = - 2 \pi r \Sigma v_{\rm r} \hspace{1cm} \text{where} \hspace{1cm} \Sigma = \int_{-\infty}^{+\infty} \rho \; \mathrm{d} z = 2 H \bar{\rho} \equiv \text{surface density}$$
2) *Conservation of Angular Momentum* ($\times 3$) $$\widetilde{\tau}_{\rm net} = \underbrace{\left(\frac{1}{(2 \pi r) (2 H)}\right)}_{\text{surface area of disk}} \frac{\mathrm{d} }{\mathrm{d} r} \Big[ 2 \pi r (\Sigma \Omega r^{2}) v_{\rm r} \Big] \hspace{1cm} \text{where} \hspace{1cm} \begin{aligned} \widetilde{\tau}_{\rm net} &\equiv \text{net torque} \\ \Sigma \Omega r^{2} &\equiv \text{ang. mom. density} \end{aligned}$$
3) *Conservation of Energy* $$\underbrace{\dot{Q} = \sigma \, T_{\rm eff}^{4}}_{\rm blackbody\ radiation} \hspace{1cm} \text{where} \hspace{1cm} \dot{Q} \equiv \text{power per unit surface area}$$
4) *Radiation Transport* $$\frac{\mathrm{d} T}{\mathrm{d} r} = -\frac{3 \kappa_{\rm R} \rho L}{16 \pi a c T^{3} r^{2}}$$

Solving these allow us to model the accretion disk's **temperature, pressure and density profiles.** To do this, we use the zero torque boundary conditions.
- [[Black Hole#Innermost Stable Circular Orbit (ISCO)|ISCO]] for [[Black Hole|BH]]
- [[Question 64|Magnetospheric Radius]] for [[Neutron Star|NS]]
- Surface of star

To go further and infer more about the disk, we need to consider the...
5. *Equation of State* (pressure or radiation dominated)
6. *[[Optical Depth#Kramer's Opacity Law]]*


> [!space] Accretion Luminosity
> Accretion assumes in-falling objects start from rest and convert gravitational potential energy into luminosity. 
> 
> $$L_{\rm acc} \propto \underbrace{\frac{\mathrm{d} T}{\mathrm{d} t} = - \frac{1}{2} \frac{\mathrm{d} U}{\mathrm{d} t}}_{\rm Virial\ Theorem} = - \frac{1}{2} \frac{\mathrm{d} }{\mathrm{d} t} \left( - \frac{G M \; \mathrm{d} M}{R} \right) = \frac{G M \dot{M}}{2 R}$$
> 
> *(See [[Question 54]])*

##### What are the assumptions that go into its derivation?

1. Subsonic turbulence
2. Geometrically thin
3. Optically thick
4. Disk acts as a [[Blackbody Radiation|blackbody]]
	- Local Thermodynamic Equilibrium (LTE)
	- Efficiently radiates heat
5. Steady state (constant $\dot{M}$)
6. Self-gravity of disk neglected