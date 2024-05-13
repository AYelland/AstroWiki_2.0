### Question
---
What is the "ideal Ohm's law" for a plasma? What does "frozen-in" mean?

### Answer
---
##### What is the "ideal Ohm's law" for a plasma?

> [!note]- Ohm's Law
> **Ohm's law** states that the electric current through a conductor between two points is directly proportional to the voltage across the two points, and the constant of proportionality is the resistance to the current. 
> $$V = I R$$
> This has been more generalized in terms of the current density ($\vec{J}$) at a specific point in the material, the conductivity ($\sigma \propto 1/R$), and the electric field ($\vec{E}$)
> $$\vec{J} = \sigma \vec{E}$$

The generalized Ohm's Law for a steady current ($\partial/\partial t \rightarrow 0$) can be expressed as...

$$\vec{J} = \sigma \vec{E}'$$

...where $\sigma$ is electrical conductivity (inverse to the resistivity) and $\vec{E}'$ is the electric field experienced by the plasma (fluid) element in its rest frame. 

In the ideal case, we neglect contributions to the electric field from other terms in the generalized Ohm's law (i.e. the Hall effect, electron inertia and ambipolar diffusion, resistivity, etc) 

When the plasma is moving (with respect to the external magnetic field $\vec{B}$) at velocity $\vec{v}$, we can apply the Lorentz transformation such that...

$$\vec{J} = \sigma (\vec{E} + \vec{v} \times \vec{B})$$

For an ideal plasma, we assume the medium has no resistance, and thus, an infinite conductivity ($\sigma \rightarrow \infty$). Therefore...

$$\boxed{\;\vec{E} + \vec{v} \times \vec{B} = 0 \;}$$

This is the **Idealized Ohm's Law**.

##### What does "frozen-in" mean?

If the Ideal Ohm's Law holds true, then the magnetic flux through any closed contour in the plasma is constant in time. In other words, the magnetic field lines are "frozen in" to the fluid motion such that the bulk fluid of the plasma and embedded magnetic field are constrained to move together (as if magnetic field lines threading through the fluid and "telling it where to flow").

> [!derivation]- Proof of Alfvén's Theorem
> The following proof constitutes "Alfvén's Theorem". Begin by combining the Idealized Ohm's Law with Faraday's Law to obtain:
> 
> $$\frac{\partial \vec{B}}{\partial t} = -\nabla \times \vec{E}  = \nabla \times \left( \vec{v} \times \vec{B} \right) $$
> 
> Then, using the fact that $\nabla \cdot \vec{B} = 0$ along with the properties of a vector triple product $\left[ \; a \times (b \times c) = (a \cdot c) \, b - (b \cdot a) \, c \; \right]$ , we can re-write this expression as:
> 
> $$\frac{\partial \vec{B}}{\partial t} = - (\vec{v} \cdot \nabla) \,\vec{B}$$
> 
> Taking the "advective" or "convective" derivative (goes by many names) $\left[ \; D/Dt = \partial/\partial t + \vec{v} \cdot \nabla \; \right]$ of $\vec{B}$ , one can also obtain this result.
> 
> $$\frac{D \vec{B}}{D t} = \left(\frac{\partial }{\partial t} + \vec{v} \cdot \nabla \right) \vec{B} = \frac{\partial \vec{B}}{\partial t} + (\vec{v} \cdot \nabla) \, \vec{B} = 0$$
> 
> What this means is that the magnetic field is constant along streamlines, or in another sense, the magnetic field lines are streamlines. 
> 
> > [!cian] 
> > I don't trust this above "proof", and I'm not sure if its reliable. I must have done something wrong because it seems that everybody does this with integral calculus. 


