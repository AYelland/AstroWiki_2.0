### Question
---
What is meant by the "gravothermal collapse" of a globular cluster, and what can save the cluster from complete collapse?

### Answer
---
A **gravothermal collapse** occurs in response to an instability from negative heat capacity of self-gravitating systems. 

> [!math] [[Thermodynamics#Negative Heat Capacity]]
> Assuming we are working with a [[Statistical Mechanics#Energy|ideal gas]] and a self-gravitating system ($U \propto r^{-1}$)...
> 
> $$\left\langle K \right\rangle = \frac{1}{2} m \bar{v}^{2} = \frac{d}{2} N k_{\rm B} T \hspace{1cm} \text{where} \hspace{1cm} d \equiv \text{degrees of freedom}$$
> 
> ... the [[Virial Theorem]] allows us to express the average total energy in terms of kinetic energy.
> 
> $$2 \left\langle K \right\rangle + \left\langle U \right\rangle = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \left\langle E \right\rangle = \frac{1}{2} \left\langle U \right\rangle \quad , \quad \left\langle E \right\rangle = - \left\langle K \right\rangle = - \frac{3}{2} N k_{\rm B} T$$
> 
> As we can see, as the temperature ($T$) increases and gets hotter, the system loses energy, and vise versa ($\partial E/\partial T < 0$). This is a consequence of a [[Thermodynamics#Negative Heat Capacity|negative heat capacity]] that appears in inhomogeneous systems not in hydrodynamical equilibrium.

In a [[Stellar Clusters#Globular Cluster|globular cluster]], two-body scattering between stars is responsible for energy transport. Through this mechanism, energy flows from central stars to the halo stars. 

Because a self-gravitating system has a negative heat capacity, when the stars in the cluster core lose energy through this two-body scattering, the core heats up (in the sense that the stellar velocities increase) and contracts on the [[Timescales#Two-Body Relaxation|relaxation timescale]]. This can be seen through the [[Virial Theorem]].

$$\left\langle E \right\rangle = - \left\langle K \right\rangle = -\frac{3}{2} N k_{\rm B} T \hspace{2cm} \left\langle E \right\rangle = \frac{1}{2} \left\langle U \right\rangle = -\frac{3 G M^{2}}{15 R} \hspace{1cm} \Rightarrow \hspace{1cm} - \left\langle E \right\rangle \propto  T \propto  \frac{1}{R}$$

This contraction leads to more heating and higher central densities in the cluster core, causing more energy loss. As it continues, the flow of energy is accelerated into a runaway core collapse.

To prevent or save the cluster from complete collapse, energy has to be re-injected into the cluster core. This is done by the scattering of [[Binary Stars|binary systems]] with a third object within the cluster core. Through the 3-body interactions, energy can be taken out of the binary orbits and can increase the energy of a third object, allowing the cluster to expand.

For clusters having a sufficiently large number of stars, the expansion can be unstable leading to so-called gravothermal oscillations. 

*([More information here...](https://link.springer.com/referenceworkentry/10.1007/978-94-007-5612-0_17))*
