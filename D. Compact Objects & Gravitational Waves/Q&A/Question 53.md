### Question
---
What is a "millisecond pulsar"? What is the shortest spin period known for such an object? Estimate a lower bound to its mean density.

### Answer
---
##### What is a "millisecond pulsar"?

![[Neutron Star#Millisecond Pulsar (MSP)]]

##### What is the shortest spin period known for such an object?

[[Catalogs#PSR]] J1748-2446ad 
- Location: [[Stellar Clusters#Globular Cluster|GC]] Terzan 5
- Discovery Date: 2006
- Period: $P = 1.4\,\pu{ms}$
- Frequency: $\nu = 716 \; {\rm Hz}$

##### Estimate a lower bound to its mean density.

The [[Neutron Star#Pulsar|pulsar]] must be at least dense enough to not be disrupted by centrifugal forces. If we consider some test mass ($m$) at the edge of the body, then  the *gravitational* and *centrifugal* forces experienced by the body are: 

$$F_{\rm g} = \frac{G M m}{R^{2}} \hspace{2.5cm} F_{\rm c} = m \Omega^{2} R$$

The minimum mean density is then achieved when these forces are balanced at the radius of the pulsar ($R$).

$$
\frac{G M m}{R^{2}} = m \Omega^{2} R
\hspace{1cm} \Rightarrow \hspace{1cm}
\Omega^{2} = G \left(\frac{M}{R^{3}}\right) = \frac{4 \pi G}{3} \underbrace{\left(\frac{M}{\frac{4}{3} \pi R^{3}}\right)}_{\rho} = \frac{4 \pi G \rho}{3}
$$
which implies 


$$\rho \ge\rho_{\rm crit} = \frac{3 \Omega^{2}}{4 \pi G}$$
