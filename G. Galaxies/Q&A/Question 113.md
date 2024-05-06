### Question
---
What is a violent relaxation? How does the phase space distribution function it produces differ from that of an isothermal gas? How does the timescale for violent relation compare to that for weak 2-body interactions?

### Answer
---
##### What is a violent relaxation?

![[Timescales#Violent Relaxation]]

##### How does the phase space distribution function it produces differ from that of an isothermal gas?

A system is "relaxed" if its coarse-grained phase space distribution is constant. In violent relaxation, the system undergoes fine-grained phase mixing, erasing the memory of its initial conditions.

This results in irreversible end-states with a roughly uniform phase space distribution, subject to the conservation of energy and conservation of fine-grained phase space density.

In comparison to an [[Galaxy Profiles#Isothermal Sphere]], the phase space distribution follows [[Statistical Mechanics#Maxwell-Boltzmann]] statistics versus the uniform distribution produced by phase mixing.

##### How does the timescale for violent relation compare to that for weak 2-body interactions?

The [[Timescales#Weak Interactions|weak two-body interaction timescale]] can be expressed in terms of the [[Timescales#Crossing Timescale|crossing timescale]].

$$t_{\rm weak} \approx \fpar{N}{6 \ln N} \; t_{\rm cross} \approx \fpar{N}{6 \ln N} \fpar{G N m}{v^{3}} \propto \frac{N^{2}}{\ln N}$$

In comparison to the [[Timescales#Violent Relaxation|violent relaxation timescale]] (effectively the [[Timescales#Dynamical Timescale|dynamical/free-fall timescale]])...

$$t_{\rm vr} \sim t_{\rm ff} \sim \frac{1}{\sqrt{G \rho}} \; \propto N\hWhere \rho = m n = \frac{3 N m}{4 \pi R^{3}} = \frac{3 v^{3}}{4 \pi G^{3} N^{2} m^{2}}$$

...we find that the violent relaxation timescale is much shorter.

$$t_{\rm weak} \approx t_{\rm ff} \fpar{N}{\ln N} \hRightarrow t_{\rm vr} \lt t_{\rm weak}$$