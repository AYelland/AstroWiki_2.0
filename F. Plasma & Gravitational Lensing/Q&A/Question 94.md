### Question
---
What are the three types of MHD waves in a magnetized plasma? Are magnetic fields important in the propagation of waves in the interstellar medium? In a star?

### Answer
---
##### What are the three types of MHD waves in a magnetized plasma?

> [!atom]- Magnetohydrodynamics (MHD)
> 
> **Magnetohydrodynamics (MHD)** is a model of electrically conducting fluids that treats all particle species together as a single continuous medium.
> 
> The *idealized MHD* model focuses on the low-frequency (long wavelength), large-scale, magnetic behavior in plasmas. 
> 
> It assumes that magnetic energy can convert to kinetic energy with perfect efficiently (no heat loss). Furthermore, it ignores GR, QM, and displacement currents, such that the bulk fluid of the plasma and embedded magnetic field are constrained to move together.
> 
> To derive the model:
> 1. Linearize Ideal MHD Equations
> 2. Define Displacement Vector
> 3. Assume Plane Wave Solution ( $\propto e^{-i (\vec{k} \cdot \vec{r} - \omega t)}$)
> 4. Derive Dispersion Relationship

**Dispersion Relation for MHD Waves:**

For MHD, there is an expanded dispersion relationship...

$$\left( \omega^{2} - k_{\parallel}^{2} \, v_{\rm A}^{2} \right) \left[ \omega^{4} - k^{2} \left( c_{\rm s}^{2} + v_{\rm A}^{2} \right) \, \omega^{2} + k^{2} \, k_{\parallel}^{2} \, c_{\rm s}^{2} \, v_{\rm A}^{2} \right] = 0$$

...where...
$$
\begin{aligned}[t]
	k &\equiv \text{wave vector} \quad(k_{\parallel} \equiv k \cos \theta)\\
	\theta &\equiv \text{angle between }\vec{B}_{0} \; {\rm and} \; \vec{k} \\
	c_{\rm s} &\equiv \text{speed of sound} = \sqrt{\pd{P}{\rho}} \\
	v_{\rm A} &\equiv \text{Alfvén Velocity} = \sqrt{\frac{B_{0}}{\mu_{0} \rho_{0}}}
\end{aligned}
$$

The different solutions to this dispersion relation gives rise to the three types of MHD waves.

![[MHD_waves.png|align:center]]

![[MHD_wavesDiagram.png|align:center|600]]

**1) Alfvén Waves** - Transverse (shear) waves in the magnetic field whose restoring force is magnetic tension. 

This means the wave propagates in the direction of the magnetic field, and oscillate transverse to that direction. Its restoring force serves to straighten out the bent magnetic field lines caused by the oscillations. The ions in the plasma provides the inertia for the wave to continue propagating.

These waves represent one of the normal modes that satisfies the first part of the dispersion relation:

$$\left( \omega^{2} - k_{\parallel}^{2} \, v_{\rm A}^{2} \right) \times \left( \dots \right) = 0 \hRightarrow \underbrace{\vec{v}_{\rm ph} = \fpar{\omega}{k} \; \hat{k} = \left( v_{\rm A} \cos \theta \right)\; \hat{k}}_{\text{phase velocity}} \quad , \quad \underbrace{\vec{v}_{\rm g} = \td{\omega}{k} = \pm \; \vec{v}_{\rm A}}_{\text{group velocity}}$$

**2 & 3) Magnetosonic Waves** - Compression waves in the density of the magnetic field lines *(similar to sounds waves in matter)*. They are driven by the mutual interaction between the electrically conducting fluid and the magnetic field.

There are two versions of magnetosonic waves that represent the other two normal modes that satisfy the second part of the dispersion relation.

$$
\begin{align}
	&\left( \dots \right) \times \left( \omega^{4} - k^{2} \left( c_{\rm s}^{2} + v_{\rm A}^{2} \right) \, \omega^{2} + k^{2} \, k_{\parallel}^{2} \, c_{\rm s}^{2} \, v_{\rm A}^{2} \right) = 0 \\
	\\
	&\hRightarrow\omega^{2} = \frac{1}{2} \left(  k^{2} \left( c_{\rm s}^{2} + v_{\rm A}^{2} \right) \pm \sqrt{k^{4} \left( c_{\rm s}^{2} + v_{\rm A}^{2} \right)^{2} - 4 k^{2} \, k_{\parallel}^{2} \, v_{\rm A}^{2} \, c_{\rm s}^{2}  } \; \right) \\
	\\
	&\hRightarrow \underbrace{\vec{v}_{\rm ph,\ \pm}^{\ 2} = \frac{\omega^{2}}{k^{2}} = \frac{1}{2} \left( \left( c_{\rm s}^{2} + v_{\rm A}^{2} \right) \pm \sqrt{\left( c_{\rm s}^{2} + v_{\rm A}^{2} \right)^{2} - 4 v_{\rm A}^{2} c_{\rm s}^{2} \cos^{2} \theta } \; \right)\; \hat{k}}_{\text{phase velocity}} 
\end{align}
$$

- **Fast Magnetosonic** ($\vec{v}_{\rm ph,\ +}$) - when plasma pressure and magnetic field are in phase
- **Slow Magnetosonic** ($\vec{v}_{\rm ph,\ -}$) - when plasma pressure and magnetic field are out of phase

In general, they are not considered longitude, but in a special case where $\vec{k} \perp \vec{B}$, they are easier to visualize.

> [!note] Sources:
> - https://www.cambridge.org/core/services/aop-cambridge-core/content/view/S0022377816000489
> - https://lweb.cfa.harvard.edu/~namurphy/Lectures/Ay253_2016_07_MHDwaves.pdf
> - http://www.physics.usyd.edu.au/~cairns/teaching/lecture3/node13.html
> - http://sun.stanford.edu/~sasha/PHYS780/SOLAR_PHYSICS/L15/Lecture_15_PHYS780.pdf

##### Are magnetic fields important in the propagation of waves in the interstellar medium? In a star?

- [[Interstellar Medium|ISM]]: Yes $\rightarrow$  mainly due to [[Question 91|Faraday rotation]]
- Stars: Yes $\rightarrow$  Alfvén waves are primary mechanism for heating of stellar corona and accelerating stellar winds. Have also been seen in shockwaves in [[Stellar Explosions#Supernova|SNe]] remnants.
