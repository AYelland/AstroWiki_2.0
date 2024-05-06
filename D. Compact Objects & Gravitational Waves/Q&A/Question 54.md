### Question
---
Show from a simple dimensional analysis how the effective temperature of an accretion disk depends on accretion rate and distance from the central object.

### Answer
---
To find the effective temperature ($T_{\rm eff}$), we need to relate it to the [[Luminosity|luminosity]] of the accretion disk. We will assume that the accretion disk is a flat disk that emits as a [[Blackbody Radiation|blackbody]] ($F = \sigma T_{\rm eff}^{4}$) from both sides ($A = 2 A_{\rm circle} = 2 \pi R^{2}$).

$$L = F \cdot A = (\sigma T_{\rm eff}^{4}) \cdot (2 \pi R^{2}) \hRightarrow T_{\rm eff} = \fpar{L}{2 \pi \sigma R^{2}}^{1/4}$$

If we assume the gas in the disk is [[Virial Theorem|virialized]] ($2T + U = 0 \implies T = - U/2$), then The power (same units as luminosity) of the accretion disk comes from the releasing the gravitational potential energy of particles/gas migrating inwards from the edge of the disk ($r=R$). 

$$L_{\rm acc} \propto \underbrace{\td{T}{t} = - \frac{1}{2} \td{U}{t}}_{\rm Virial\ Theorem} = - \frac{1}{2} \td{}{t} \left( - \frac{G M \; \rd M}{R} \right) = \frac{G M \dot{M}}{2 R} \hRightarrow L_{\rm acc} = \frac{G M \dot{M}}{2 R}$$

Applying this to the effective temperature equation...

$$T_{\rm eff} = \left( \frac{L_{\rm acc}}{2 \pi \sigma R^{2}} \right)^{1/4} = \left( \frac{1}{2 \pi \sigma R^{2}} \cdot \frac{G M \dot{M}}{2 R} \right)^{1/4} = \left( \frac{G M \dot{M}}{4 \pi \sigma R^{3}} \right)^{1/4} \propto \;  R^{-3/4}$$

This expression has the wrong pre-factor, but the radial dependence is approximately correct, depending on type of disk.