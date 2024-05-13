---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - Jeans stability criteria
---
## Jeans Equation

> [!key-idea] The Jeans Equation
> 
> The Jeans equation describes the collisionless motion of a collection of stars in a gravitational potential field.

Beginning with the **Collisionless Boltzmann Equation (CBE)**...

$$\frac{\partial f}{\partial t} + \vec{v} \, \frac{\partial f}{\partial \vec{x}} - \frac{\partial \Phi}{\partial \vec{x}} \, \frac{\partial f}{\partial \vec{v}} \, = \, 0 \hspace{1cm} \text{where} \hspace{1cm} \left\{ \; \begin{aligned}
	\frac{\partial f}{\partial t} &\equiv \text{rate of change in \# of stars} \\
	\vec{v} \, \frac{\partial f}{\partial \vec{x}} &\equiv \text{in/out flow of spatical volume} \\
	\frac{\partial \Phi}{\partial \vec{x}} \, \frac{\partial f}{\partial \vec{v}} &\equiv \text{in/out flow of momentum volume}
\end{aligned} \right.$$

...we can derive the **Jeans Equation** through analyzing the "moments" of the CBE in the phase-space distribution. The  moment of a function can be defined as:

$$\mu_{n} = \int_{-\infty}^{+\infty} x^{n} f(x) \; \mathrm{d} x$$

Usually, these moments represent total probability ($n=0$), the mean ($n=1$), the variance ($n=2$), the skewness ($n=3$), etc. For the phase-space density function ($f$) of the CBE, these moments represent the **density** ($n=0$), **mean velocity** ($n=1$), and the **velocity dispersion** ($n=2$). (see [[Fluid Mechanics#Conservation Laws]]) 

$$n = \int_{-\infty}^{+\infty} \mathrm{d}^{3} \vec{v} \; f \hspace{1.3cm} \overline{v}_{i} = \frac{1}{n} \; \int_{-\infty}^{+\infty} \mathrm{d}^{3} \vec{v} \; v_{i} f \hspace{1.3cm} \sigma_{ij} \equiv \overline{v_{i} v_{j}} = \frac{1}{n} \; \int_{-\infty}^{+\infty} \mathrm{d}^{3} \vec{v} \; v_{i} v_{j} f$$

By explicitly calculating zeroth moment ($n=0$) of the CBE, we can find the **[[Fluid Mechanics#Conservation of Mass|3D continuity equation]]**.

$$\frac{\partial n}{\partial t} + \frac{\partial }{\partial \vec{x}} \left( n \vec{v} \right) = 0$$

> [!derivation]-
> 
> We now look at the first moment of the collisionless Boltzmann equation.  We break each integral into three terms to simplify each individually.
> 
> $$\begin{aligned}
> 	& \int d^{3} \vec{v} \left( \frac{\partial f}{\partial t} + \vec{v} \frac{\partial f}{\partial \vec{x}} - \vec{\nabla} \Phi \frac{\partial f}{\partial \vec{v}} \right) = 0 \\
> 	& \underbrace{\int d^{3} \vec{v} \; \frac{\partial f}{\partial t}}_{\require{enclose}\enclose{circle}{1}} + \underbrace{\int d^{3} \vec{v} \; \vec{v} \frac{\partial f}{\partial \vec{x}}}_{\require{enclose}\enclose{circle}{2}} - \underbrace{\int d^{3} \vec{v} \; \vec{\nabla} \Phi \frac{\partial f}{\partial \vec{v}}}_{\require{enclose}\enclose{circle}{3}} = 0
> \end{aligned}$$
> 
> $$\begin{alignat}{3}
> 	\require{enclose}\enclose{circle}{1}:& \quad \int \mathrm{d}^{3} \vec{v} \; \frac{\partial f}{\partial t} &&= \frac{\partial }{\partial t} \int d^{3} \vec{v} \; f &&= \frac{\partial n}{\partial t} \\
> 	\require{enclose}\enclose{circle}{2}:& \quad \int d^{3} \vec{v} \; \vec{v} \frac{\partial f}{\partial \vec{x}} &&= \frac{\partial }{\partial \vec{x}} \left(\int \mathrm{d}^{3} \vec{v} \; \vec{v} f \right) &&= \vec{\nabla}_{x} \left( n \vec{v} \right) \\
> 	\require{enclose}\enclose{circle}{3}: & \quad \int d^{3} \vec{v} \; \frac{\partial \Phi}{\partial \vec{x}} \frac{\partial f}{\partial \vec{v}} > &&= \frac{\partial \Phi}{\partial \vec{x}} \int d^{3} \vec{v} \; \frac{\partial f}{\partial \vec{v}} &&= \frac{\partial \Phi}{\partial \vec{x}} \Big[ \; f \; \Big]_{\vec{v}=-\infty}^{\vec{v}=+\infty} = 0
> \end{alignat}$$
> 
> For the third term, we used the fact that phase-space distribution goes to 0 at $\pm\infty$ for physical systems.
>   
> This gives us the **3D Continuity Equation**:
> 
> $$\boxed{\frac{\partial n}{\partial t} + \vec{\nabla}_{x} \left( n \vec{v} \right) = 0}$$

By explicitly calculating first moment ($n=1$) of the CBE, we can find the **Jeans Equation**. 

$$\boxed{\frac{\partial \overline{v}_{j}}{\partial t} + \sum_{i} \overline{v}_{i} \frac{\partial \overline{v}_{j}}{\partial x_{i}} =  - \frac{\partial \Phi}{\partial x_{j}} - \frac{1}{n} \sum_{i} \frac{\partial (n \sigma_{ij}^{2})}{\partial x_{i}}}$$

$$\begin{alignat}{2}
    \frac{\partial \overline{v}_{j}}{\partial t} &\equiv \text{acceleration of fluid} &\hspace{1.5cm} - \frac{1}{n} \sum_{i} \frac{\partial (n \sigma_{ij}^{2})}{\partial x_{i}} &\equiv \text{pressure} \\
    \sum_{i} \overline{v}_{i} \frac{\partial \overline{v}_{j}}{\partial x_{i}} &\equiv \text{kinematic viscosity} &\hspace{1.5cm} - \frac{\partial \Phi}{\partial x_{j}} &\equiv \text{gravity}
\end{alignat}$$

We can rewrite the Jeans Equation if we express the number density $n$ using $\rho=mn$ and assume that $\sigma_{ij}$ is isotropic, such that the pressure is $P = \rho \sigma_{ij}^{2} = \rho \sigma_{ij} = m n \sigma_{ij}^{2}$.  

$$\boxed{\; \frac{\partial \vec{v}}{\partial t} + \left(\vec{v}\cdot\vec{\nabla}\right)\vec{v} = -\vec{\nabla}\Phi - \frac{1}{\rho}\vec{\nabla} P \;} \hspace{1cm} \text{or} \hspace{1cm} \frac{D \vec{v}}{Dt} = -\nabla \Phi - \frac{1}{\rho}\nabla P$$

...where $D/Dt = \partial/\partial t + (\mathbf{v}\cdot\nabla)$ is the convective derivative. Here $\Phi$ is the gravitational potential and $P$ is the pressure. *(This is the same as the [[Fluid Mechanics#Conservation of Momentum|Conservation of Momentum]] in fluid mechanics.)*

> [!derivation]-
> 
> We now look at the first moment of the collisionless Boltzmann equation.  We break each integral into three terms to simplify each individually.
> 
>$$\begin{aligned}
>	&\int d^{3} \vec{v} \; v_{j} \left( \frac{\partial f}{\partial t} + \vec{v} \frac{\partial f}{\partial \vec{x}} - \vec{\nabla} \Phi \frac{\partial f}{\partial \vec{v}} \right) = 0 \\
>	&\underbrace{\int d^{3} \vec{v} \; v_{j} \frac{\partial f}{\partial t}}_{\require{enclose}\enclose{circle}{1}} + \underbrace{\int d^{3} \vec{v} \; v_{j} \vec{v} \frac{\partial f}{\partial \vec{x}}}_{\require{enclose}\enclose{circle}{2}} - \underbrace{\int d^{3} \vec{v} \; v_{j} \vec{\nabla} \Phi \frac{\partial f}{\partial \vec{v}}}_{\require{enclose}\enclose{circle}{3}} = 0
>\end{aligned}$$
>
>\frac{\partial n}{\partial t} = - \sum_{i} \frac{\partial }{\partial x_{i}} \left( n \bar{v}_{i} \right)
> $$\begin{alignat}{3}
> 	\require{enclose}\enclose{circle}{1}:& \quad \int d^{3} \vec{v} \; v_{j} \frac{\partial f}{\partial t} &&= \frac{\partial }{\partial t} \int d^{3} \vec{v} \; v_{j} f \\
> 	&&&= \frac{\partial }{\partial t} \left( n \bar{v}_{j} \right) \\
> 	&&&= \frac{\partial n}{\partial t} \bar{v}_{j} + n \frac{\partial v_{j}}{\partial t} \\
> 	&&&= -\bar{v}_{j} \sum_{i} \frac{\partial }{\partial x_{i}}\left( n \bar{v}_{i} \right) + n \frac{\partial \bar{v}_{j}}{\partial t} \\
> 	&&&= n \frac{\partial \bar{v}_{j}}{\partial t} -\bar{v}_{j} \sum_{i} \frac{\partial }{\partial x_{i}} \left(n \bar{v}_{i} \right) \\
> 	\\
> 	\require{enclose}\enclose{circle}{2}:& \quad \int d^{3} \vec{v} \; v_{j} \vec{v} \frac{\partial f}{\partial \vec{x}} &&= \int d^{3} \; v_{j} \sum_{i} \frac{\partial }{\partial x_{i}} \\
> 	&&&= \sum_{i} \frac{\partial }{\partial x_{i}} \int d^{3} \vec{v} \; v_{j} v_{i} f \\
> 	&&&= \sum_{i} \frac{\partial }{\partial x_{i}} \left( n \overline{v_{j} v_{i}} \right) \\
> 	&&&= \sum_{i} \frac{\partial }{\partial x_{i}} \left(n \left(\sigma_{ij}^{2} + \bar{v}_{i} \bar{v}_{j} \right) \right) \\
> 	\\
> 	\require{enclose}\enclose{circle}{3}:& \quad \int d^{3} \vec{v} \; v_{j} \frac{\partial \Phi}{\partial \vec{x}} \frac{\partial f}{\partial \vec{v}} &&= \int d^{3} \vec{v} \; v_{j} \sum_{i} \frac{\partial \Phi}{\partial x_{i}} \frac{\partial f}{\partial v_{i}} \\
> 	&&&= \sum_{i} \frac{\partial \Phi}{\partial x_{i}} \int d^{3} \vec{v} \; v_{j} \frac{\partial f}{\partial v_{i}} \\
> 	&&&= \sum_{i} \frac{\partial \Phi}{\partial x_{i}} \int \mathrm{d} v_{k} \int \mathrm{d} v_{l} \int \mathrm{d} v_{i} \left( v_{j} \frac{\partial f}{\partial v_{i}} \right) \\
> 	&&&= \sum_{i} \frac{\partial \Phi}{\partial x_{i}} \int \mathrm{d} v_{k} \int \mathrm{d} v_{l}  \left[ \Big[ v_{j} f \Big]_{v_{i} = -\infty}^{v_{i} = +\infty} - \int \mathrm{d} v_{i} \frac{\partial v_{j}}{\partial v_{i}} f \right] \\
> 	&&&= -\sum_{i} \frac{\partial \Phi}{\partial x_{i}} \int \mathrm{d} v_{k} \int \mathrm{d} v_{l} \int \mathrm{d} v_{i} \delta_{ij} f \\
> 	&&&= -\sum_{i} \frac{\partial \Phi}{\partial x_{i}} \int d^{3} \vec{v} \delta_{ij} f \\
> 	&&&= -n \frac{\partial \Phi}{\partial x_{j}}
> \end{alignat}$$
> 
> Plugging each term back in, we get...
> 
> $$n \frac{\partial \bar{v}_{j}}{\partial t} - \bar{v}_{j} \sum_{i} \frac{\partial }{\partial x_{i}}(n \bar{v}_{i}) + \sum_{i} \frac{\partial }{\partial x_{i}} \left[ n \left(\sigma_{ij}^{2} + \bar{v}_{i} \bar{v}_{j} \right) \right] + n \frac{\partial \Phi}{\partial x_{i}} = 0$$
> 
> ...which we can rewrite as...
> 
> $$\begin{aligned}
> 	n \frac{\partial \bar{v}_{j}}{\partial t} - \underline{\bar{v}_{j} \sum_{i} \frac{\partial }{\partial x_{i}}(n \bar{v}_{i})} + \sum_{i} \frac{\partial }{\partial x_{i}}(n \sigma_{ij}^{2}) + &\underbrace{\sum_{i} \frac{\partial }{\partial x_{i}}(n \bar{v}_{i} \bar{v}_{j})} + n \frac{\partial \Phi}{\partial x_{j}} = 0 \\
> 	& = \sum_{i} (n \bar{v}_{i}) \frac{\partial }{\partial x_{i}} \bar{v}_{j} + \underline{ \sum_{i} \bar{v}_{j} \frac{\partial }{\partial x_{i}}(n \bar{v}_{i})}
> \end{aligned}$$
> 
> ...where the two underlined terms cancel.
> 
> $$n \frac{\partial \bar{v}_{j}}{\partial t} + \sum_{i} (n\bar{v}_{i}) \frac{\partial }{\partial x_{i}} \bar{v}_{j} + \sum_{i} \frac{\partial }{\partial x_{i}}(n \sigma_{ij}^{2}) + n \frac{\partial \Phi}{\partial x_{j}} = 0$$
> 
> This is the **Jeans Equation**, often written
> 
> $$\boxed{\; \frac{\partial \bar{v}_{j}}{\partial t} + \sum_{i} \bar{v}_{i} \frac{\partial \bar{v}_{j}}{\partial x_{i}} = -\frac{1}{n} \sum_{i} \frac{\partial (n\sigma_{ij}^{2})}{\partial x_{i}} - \frac{\partial \Phi}{\partial x_{j}} \;}$$

> [!note] Jeans Swindle
> You can also derive from Jeans Equation (the first moment of collisionless Boltzmann) + continuity + Jeans swindle (static uniform background). 
> - Find wave equation that is stable for complex exponential solution. 
> - Analogous to comparing free fall and sound times $\implies$ If $t_{\rm sound} < t_{\rm dyn}$, the gas cloud does not have enough time to react to free-fall + cloud is unstable

## Jeans Stability Criteria

The **Jeans Stability Criteria** is the boundary between a cloud of dust or gas undergoing gravitational collapse and expansion. The condition for stability can be expressed in terms of wavelength/radius, mass, or frequency.

It can be derived by considering a static, uniform background, and applying a small perturbation to that background. As the perturbation propagates, it will move at the [[Fluid Mechanics#Speed of Sound|speed of sound]] within the medium, following a density plane wave with the associated dispersion relation.
$$\underbrace{\; \frac{\partial^{2} \rho_{1}}{\partial t^{2}} - 4 \pi G \rho_{0} \rho_{1} - c_{s}^{2} \vec{\nabla}^{2} \rho_{1} = 0 \;}_{\text{wave equation}}$$
$$\underbrace{\; \rho_{1} = C e^{i (\vec{k} \cdot \vec{x} - \omega t)}}_{\text{plane wave}} \hspace{1cm} \text{where} \hspace{1cm} \underbrace{\; \omega^{2} = c_{s}^{2} k^{2} - 4 \pi G \rho_{0} \;}_{\text{dispersion relation}}$$

The frequency/wavelength of this perturbation wave will determine whether the system remains stable or becomes unstable, initiating a gravitational collapse.

*Frequency Stability Conditions:*
-  $\omega^{2} > 0 \; \therefore \; \omega \in \mathbb{R}  \; \therefore \; \rho_{0} \in \mathbb{C} \implies$ stable oscillating modes for $\rho_{1}$
-  $\omega^{2} < 0 \; \therefore \; \omega \in \mathbb{C}  \; \therefore \; \rho_{0} \in \mathbb{R} \implies$ unstable exponentially growing or decaying modes for $\rho_{1}$

*Wavelength/Radius Stability Conditions:*
-  $\lambda < \lambda_{J} \; \therefore \; \omega \in \mathbb{R}  \; \therefore \; \rho_{0} \in \mathbb{C} \implies$ stable oscillating modes for $\rho_{1}$
-  $\lambda > \lambda_{J} \; \therefore \; \omega \in \mathbb{C}  \; \therefore \; \rho_{0} \in \mathbb{R} \implies$ unstable exponentially growing or decaying modes for $\rho_{1}$

*Mass Stability Conditions:*
-  $M < M_{J} \; \therefore \; R = \lambda < \lambda_{J} \implies$ stable oscillating modes for $\rho_{1}$
-  $M > M_{J} \; \therefore \; R = \lambda > \lambda_{J} \implies$ unstable exponentially growing or decaying modes for $\rho_{1}$


> [!derivation]- Derivation: [[#Jeans Equation]] with Jeans Swindle
> 
> Beginning with the [[#Jeans Equation]] and the continuity equation...
> 
> $$\frac{\partial \vec{v}}{\partial t} + \left(\vec{v}\cdot\vec{\nabla}\right)\vec{v} = -\vec{\nabla}\Phi - \frac{1}{\rho}\vec{\nabla}P \hspace{2cm} \frac{\partial \rho}{\partial t} + \vec{\nabla}\cdot\left(\rho\vec{v}\right) = 0$$
> 
> ...we can apply a small perturbation to a static uniform static background such that we have the following expressions for our parameters.
> 
> $$\begin{alignat}{2}
> 	\rho &= \rho_0 &&+ \epsilon \, \rho_1(\vec{x},t \\
> 	\vec{v} &= \vec{v}_0 &&+ \epsilon \, \vec{v}_1(\vec{x},t) \\
> 	P &= P_0 &&+ \epsilon \, P_1(\vec{x},t) \\
> 	\Phi &= \Phi_0 &&+ \epsilon \, \Phi_1(\vec{x},t)
> \end{alignat}$$
> 
> We can now apply the **Jeans Swindle**, where we will choose ($\vec{v}_{0} = \Phi_{0} = 0$) and ($\rho_{0} \, , \, P_{0} =$ non-zero constants) by the static background assumption. 
> 
> > [!note] 
> > 
> > These are not a physical set of conditions because Poisson's equation gives...
> > 
> > $$\nabla^2\Phi_{0}=4\pi G\rho_{0} \hspace{1cm} \text{such that} \hspace{1cm} \Phi_0=0 \; \Rightarrow \; \rho_{0}=0$$
> > 
> > ...but we continue with our calculations ignoring this fact. It's called the "swindle" because even though it is not physical, it surprisingly yields the exact answer.
> 
> Plugging these perturbations into the continuity equation, neglecting terms of order $\mathcal{O}(\epsilon^{2})$:
> 
> $$\frac{\partial }{\partial t} \left( \rho_{0} + \epsilon \, \rho_{1} \right) + \vec{\nabla} \left(\rho_{0} \vec{v}_{0} + \epsilon \rho_{1} \vec{v}_{0} + \epsilon \rho_{0} \vec{v}_{1} + \epsilon^{2} \rho_{1} \vec{v}_{1} \right) = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\partial \rho_{1}}{\partial t} + \rho_{0} \vec{\nabla}\cdot\vec{v}_{1} = 0$$
> 
> Plugging these perturbations into the Jeans equation, neglecting terms of order $\mathcal{O}(\epsilon^{2})$:
> 
> $$\left( \frac{\partial \vec{v}_{0}}{\partial t} + \epsilon \frac{\partial \vec{v}_{1}}{\partial t} \right) + \left( (\vec{v}_{0} + \epsilon \vec{v}_{1}) \cdot \vec{\nabla} \right) \left( \vec{v}_{0} + \epsilon \vec{v}_{1} \right) = -\vec{\nabla} \left( \Phi_{0} + \epsilon \Phi_{1} \right) - \frac{1}{\rho_{0} + \epsilon \rho_{1}} \vec{\nabla} \left( P_{0} + \epsilon P_{1} \right)$$
> $$\Downarrow$$
> $$\frac{\partial \vec{v}_{1}}{\partial t} = - \vec{\nabla} \Phi_{1} \, - \, \frac{\vec{\nabla} P_{1}}{\rho_{0}}$$
> 
> We can re-write the pressure gradient in terms of the [[Fluid Mechanics#Speed of Sound|speed of sound]] ($c_{s}$), or the speed at which perturbations can propagate.
> 
> $$\vec{\nabla} P_{1} = \frac{\partial P_{1}}{\partial \vec{x}} = \frac{\partial P_{1}}{\partial \rho_{1}} \cdot \frac{\partial \rho_{1}}{\partial \vec{x}} = c_{s}^{2} \cdot \frac{\partial \rho_{1}}{\partial \vec{x}} = c_{s}^{2} \, \vec{\nabla} \rho_{1}$$
> 
> This gives us:
> $$\frac{\partial \vec{v}_{1}}{\partial t} = - \vec{\nabla} \Phi_{1} \, - \, \frac{c_{s}^{2}}{\rho_{0}} \, \vec{\nabla} \rho_{1}$$
> 
> Combining these two equations, we use the time derivative of the continuity equation and the Poisson Equation for gravitational potential ($\vec{\nabla}^{2} \Phi = 4 \pi G \rho$).
> 
> $$\frac{\partial^{2} \rho_{1}}{\partial t^{2}} + \rho_{0} \vec{\nabla} \cdot \left( \frac{\partial \vec{v}_{1}}{\partial t} \right)= 0 \hspace{1cm} \Rightarrow \hspace{1cm} \begin{aligned}[t]
> 	\frac{\partial^{2} \rho_{1}}{\partial t^{2}} + \rho_{0} \vec{\nabla} \cdot \left( \;- \vec{\nabla} \Phi_{1} \, - \, \frac{c_{s}^{2}}{\rho_{0}} \, \vec{\nabla} \rho_{1} \;\right) = 0 \\
> 	\frac{\partial^{2} \rho_{1}}{\partial t^{2}} - \rho_{0} \; \underbrace{\vec{\nabla}^{2} \Phi_{1} \ }_{4 \pi G \rho_{1}} \, - \, c_{s}^{2} \; \vec{\nabla}^{2} \rho_{1} = 0
> \end{aligned}$$
> 
> Finally, we get the wave equation for the density perturbations of the background ($\rho_{1}$), effectively describing the time-evolution of the perturbation.
> 
> $$\boxed{ \; \frac{\partial^{2} \rho_{1}}{\partial t^{2}} - 4 \pi G \rho_{0} \rho_{1} - c_{s}^{2} \vec{\nabla}^{2} \rho_{1} = 0 \;}$$
> 
> With the assumed plane wave solution form, we can define a **dispersion relation** that yields a stability condition for some perturbation.
> 
> $$\rho_{n} = C e^{i ( \vec{k} \cdot \vec{x} - \omega t  )} \hspace{1cm} \text{where} \hspace{1cm} \omega^{2} = c_{s}^{2} k^{2} - 4 \pi G \rho_{0}$$
> 
> *Stability Conditions:*
> -  $\omega^{2} > 0 \; \therefore \; \omega \in \mathbb{R}  \; \therefore \; \rho_{0} \in \mathbb{C} \implies$ stable oscillating modes for $\rho_{1}$
> -  $\omega^{2} < 0 \; \therefore \; \omega \in \mathbb{C}  \; \therefore \; \rho_{0} \in \mathbb{R} \implies$ unstable exponentially growing or decaying modes for $\rho_{1}$
> 
> 
> Similarly, if we recast into terms of the wavelength $\lambda = 2\pi / k$, we can evaluate stability condition in terms of scale lengths.
> 
> $$\omega = \frac{2 \pi c_{s}}{\lambda}\sqrt{1 - \left(\frac{G \rho_{0}}{\pi c_{s}^{2}}\right) \lambda^{2}} = \frac{2 \pi c_{s}}{\lambda}\sqrt{1 - \left(\frac{\lambda}{\lambda_{J}}\right)^{2}} \hspace{1cm} \text{where} \hspace{1cm} \underbrace{\lambda_{J} \equiv \sqrt{\frac{\pi c_{s}^{2}}{G \rho_{0}}}}_{\text{Jeans Length}}$$
> 
> *Stability Conditions:*
> -  $\lambda < \lambda_{J} \; \therefore \; \omega \in \mathbb{R}  \; \therefore \; \rho_{0} \in \mathbb{C} \implies$ stable oscillating modes for $\rho_{1}$
> -  $\lambda > \lambda_{J} \; \therefore \; \omega \in \mathbb{C}  \; \therefore \; \rho_{0} \in \mathbb{R} \implies$ unstable exponentially growing or decaying modes for $\rho_{1}$
> 
> This quantity is known as the [[#Jeans Length]] ($\lambda_{J}$); it represents the maximum size a perturbation can remain stable. The associated [[#Jeans Mass]] ($M_{J}$) is the mass enclosed within the [[#Jeans Length]] of a given substance. Therefore, the system has stability when $\lambda<\lambda_J$ and $M<M_J$.  
> 
> $$\boxed{\lambda_{J}^2 = \left(\frac{2 \pi}{k}\right)^2 = \frac{\pi c_{s}^2}{G\rho_{0}}} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{M_{J} = \left( \frac{4}{3} \pi \lambda_{J}^{3} \right) \rho_{0}}$$
^jeans-swindle

> [!derivation]- Derivation: [[Virial Theorem]]
> It can be calculated using the Virial Theorem, such that...
> 
> $$
> 2 \left\langle K \right\rangle + \left\langle U \right\rangle = 0
> \hspace{1cm} \text{where} \hspace{1cm}
> \begin{cases}
> 	\quad | 2 \left\langle K \right\rangle | > | \left\langle U \right\rangle | &\implies \text{expansion} \\
> 	\quad | 2 \left\langle K \right\rangle | < | \left\langle U \right\rangle | &\implies \text{collapse} \\
> \end{cases}
> $$
> 
> If we consider a spherical cloud of gas with constant density, then we can take the average potential energy as the [[Binding Energy#Gravitational Binding Energy|gravitational binding energy]] and the average kinetic energy for a [[Statistical Mechanics#Energy|monatomic ideal gas]].
> 
> $$\left\langle U \right\rangle = - \frac{3}{5} \frac{G M^{2}}{R} \hspace{2cm} \left\langle K \right\rangle = \frac{3}{2} N k_{\rm B} T = \frac{3}{2} \left(\frac{M}{\mu m_{\rm p}}\right) k_{\rm B} T$$
> 
> Solving the Virial Theorem then yields the **[[#Jeans Length]]** ($\lambda_{\rm J} \equiv R_{\rm J}$), and equivalently, the **[[#Jeans Mass]]** ($M_{\rm J}$). For the condition of collapse (unstable)...
> 
> $$
> \begin{aligned}[t]
> 	2 \left\langle K \right\rangle < \left\langle U \right\rangle  \hspace{1cm} \Rightarrow \hspace{1cm} 2 \left(\frac{3 M k_{\rm B} T}{2 \mu m_{\rm p}}\right) &< \frac{3}{5} \frac{G M^{2}}{R} \\
> 	M &> \left(\frac{5 k_{\rm B} T}{G \mu m_{\rm p}}\right) R \\
> 	\frac{4 \pi R^{3} \rho}{3} &> \left(\frac{5 k_{\rm B} T}{G \mu m_{\rm p}}\right) R
> \end{aligned}
> $$
> $$R > R_{J} = \sqrt{\frac{15 k_{\rm B} T}{4 \pi G \mu m_{\rm p} \rho}} = \sqrt{\frac{15 c_{s}^{2}}{4 \pi G \rho}} \simeq \sqrt{\frac{\pi c_{s}^{2}}{G \rho}} = \lambda_{J}$$
> 
> ...where the [[Fluid Mechanics#Speed of Sound|speed of sound]] can be calculated from the [[Thermodynamics#Ideal Gas Law]]. 
> $$\textcolor{gray}{\left[ \; c_{s}^{2} = \frac{\partial P}{\partial \rho} = \frac{\partial }{\partial \rho} \left( \frac{\rho \, k_{\rm B} T}{\mu m_{\rm p}} \right) = \frac{k_{\rm B} T}{\mu m_{\rm p}} \; \right]}$$
> 
> The constant of this calculation differs from the Jeans Length calculated by the [[#Jeans Equation]], but it is gives a good approximation with the proper dependence.
> 
> The [[#Jeans Mass]] can be determined by assuming the spherical volume has a constant density.
> $$M > M_{J} = \left( \frac{4}{3} \pi R_{J}^{3} \right) \rho $$
> 
> This allows us to define the **Jeans Stability Criteria** through the radius and mass of the gas cloud, and determine whether it will collapse or expand.
> 
> $$
> \begin{align}
> 	\left\{ \; M > M_{\rm J} \; , \; R > \lambda_{\rm J} \; \right\} &\hspace{1cm} \Rightarrow \hspace{1cm} \text{Gravitational Collapse} \\
> 	\left\{ \; M < M_{\rm J} \; , \; R < \lambda_{\rm J} \; \right\} &\hspace{1cm} \Rightarrow \hspace{1cm} \text{Expansion}
> \end{align}
> $$
^jeans-virial-theorem

> [!derivation]- Derivation: Comparing Timescales
> 
> Consider sound [[Timescales#Crossing Timescale|crossing time]] of a perturbation in a gas (moving at the [[Fluid Mechanics#Speed of Sound|sound speed]]). If the sound crossing time (the timescale over which the material can respond) is longer than the [[Timescales#Dynamical Timescale|free-fall timescale]], then the material will collapse. If perturbations can be crossed before collapse, pressure can stabilize the collapse.
> 
> $$t_{\rm ff} \sim \frac{1}{\sqrt{G \rho}} \hspace{2cm} t_{\rm cross} \sim \frac{\lambda}{c_{s}}$$
> 
> For the condition of collapse, we find the length scale of...
> 
> $$t_{\rm cross} > t_{\rm ff} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\lambda}{c_{s}} > \frac{1}{\sqrt{G \rho}} \hspace{1cm} \Rightarrow \hspace{1cm} \lambda > \sqrt{\frac{c_{s}^{2}}{G \rho}} \simeq \sqrt{\frac{\pi c_{s}^{2}}{G \rho}} = \lambda_{J}$$
> 
> This means that random motion and pressure can stabilize perturbations on *small scales.*
> 
> -  $\lambda < \lambda_{J} \implies$ system can stabilize and prevent collapse
> -  $\lambda > \lambda_{J} \implies$ system is unstable and will undergo collapse
^jeans-timescales

> [!note]
> The Jeans Stability Criteria does not account for rotation, external pressure (from the ISM), magnetic field lines, etc. (Toomre Stability Criteria accounts for rotation) 

(https://www.christopherlovell.co.uk/blog/2016/04/26/jeans-mass.html)

## Jeans Length

The **Jeans Length** is the length scale above which a body will gravitationally collapse. 

$$\lambda_{J}^2 = \left(\frac{2 \pi}{k}\right)^2 = \frac{\pi c_{s}^2}{G\rho_{0}}$$

It can be derived directly by...
- Perturbing the [[#Jeans Equation]] (see [[#^jeans-swindle|here]])
- The [[Virial Theorem]] balancing thermal energy and gravitational energy (see [[#^jeans-virial-theorem|here]])
- Comparing a perturbation's [[Timescales#Crossing Timescale|crossing time]] with the [[Timescales#Dynamical Timescale|free-fall timescale]] (see [[#^jeans-timescales|here]])

## Jeans Mass

The **Jeans Mass** is the mass contained within a sphere of radius equal to the [[#Jeans Length]].

$$M_{\rm J} = \left( \frac{4}{3} \pi \lambda_{\rm J}^{3} \right) \rho \hspace{1cm} \text{where} \hspace{1cm} \lambda_{J} = \sqrt{\frac{\pi c_{s}^{2}}{G \rho}} \quad , \quad c_{s} = \sqrt{\frac{\partial P}{\partial \rho}}$$