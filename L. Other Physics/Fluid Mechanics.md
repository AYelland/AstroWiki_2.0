---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
## Conservation Laws

#### Conservation of Mass
*(Also known as **Continuity**)*

$$
\frac{\partial \rho}{\partial t} + \nabla \cdot \left( \rho \vec{v} \right) = 0
\hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}[t]
	\rho &\equiv {\rm density} \\
	\vec{v} &\equiv {\rm fluid\ velocity}
\end{aligned}
$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\partial \rho}{\partial t} + \frac{1}{r^{2}} \frac{\partial }{\partial r} (r^{2} \rho v) = 0$$

#### Conservation of Momentum

$$
\frac{\partial \vec{v}}{\partial t} + (\vec{v} \cdot \nabla) \vec{v} + \frac{1}{\rho} \nabla P = \frac{1}{\rho} \vec{f}
\hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}[t]
	P &\equiv {\rm pressure} \\
	\vec{f} &\equiv {\rm external\ force\ per\ volume} \\
	&\hspace{1cm} \textcolor{gray}{\left[ \vec{f}_{\rm grav} = -\nabla \Phi_{\rm g} \right]}
\end{aligned}
$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\partial v}{\partial t} + v \frac{\partial v}{\partial r} + \frac{1}{\rho} \frac{\partial P}{\partial r} = \frac{1}{\rho} f_{\rm r}$$

#### Conservation of Energy
 $$\frac{\partial \epsilon}{\partial t} + \nabla \cdot \left[ (\epsilon + P) \vec{v} \right] = 0 \hspace{1cm} \text{where} \hspace{1cm} \epsilon = \underbrace{\left( \frac{1}{2} \rho |\vec{v}|^{2} \right)}_{\substack{\text{dyanmical} \\ \text{energy density}}} + \underbrace{\left( \frac{3}{2} n k_{\rm B} T \right)}_{\substack{\text{gas} \\ \text{energy density}}} + \underbrace{\bigg( \rho \,\Phi_{\rm g} \bigg)}_{\substack{\text{gravitational} \\ \text{energy density}}}$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\partial \epsilon}{\partial t} + \frac{1}{r^{2}} \frac{\partial }{\partial r} \left[ r^{2} (\epsilon + P) v \right] = 0$$

## Ram Pressure

**Ram pressure** is a pressure exerted on a body moving through a fluid medium. This motion causes a drag force on the body, effectively transferring momentum from the fluid into the body. This is caused by the relative bulk motion of the fluid around the body, rather than random thermal motion. 

If we simplify the fluid mechanics and assume that all matter incident upon a surface transfers all of its momentum into the volume, this is equivalent to the matter "entering the volume" in terms of momentum transfer. Furthermore, if only the momentum perpendicular to the surface is transferred and we exclude shear forces, the maximum pressure exerted on that surface is...

$$
P_{\rm{ram}} = \rho v_{\rm n}^{2} \hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}
	\rho &\equiv \text{mass density of fluid} \\
	v_{\rm n} &\equiv \text{velocity of fluid normal to surface}
\end{aligned}
$$

> [!note]
> Without viscosity, the stress tensor is isotropic thermal pressure + ram pressure.

*(Interesting [source](https://royalsocietypublishing.org/doi/10.1098/rspa.2022.0504))*

## Speed of Sound
*([This is a good resource for sound speed.](https://pressbooks.online.ucf.edu/osuniversityphysics/chapter/17-2-speed-of-sound/#:~:text=Derivation%20of%20the%20Speed%20of%20Sound%20in%20Air,equation%20discussed%20in%20Fluid%20Mechanics.&text=dmdt%3Dd,dt%3D%CF%81Av))*

$$\boxed{\;c_{\rm s} \equiv v = \sqrt{\frac{\mathrm{d} P}{\mathrm{d} \rho}} \;}$$

> [!atom] In an ideal gas, the equation for the speed of sound is...
>
> $$
> c_{\rm s} = \sqrt{\frac{\gamma R T}{M}} \hspace{1cm} \text{where} \hspace{1cm} 
> \begin{aligned}
>	 \gamma &= \text{adiabatic index} \\
>	 R &= \text{gas constant} = 8.31 \; {\rm J/(mol \cdot K)} \\
>	 T &= \text{temperature} \\
>	 M &= \text{mass}
> \end{aligned}
> $$

In general, the more rigid (or less compressible) the medium, the faster the speed of sound. Here are some sounds speeds in various mediums.

| Medium                        | _v_ (${\rm m/s}$) |
| ----------------------------- | ----------------- |
| **Gases at $0 \degree C$**    |                   |
| Air                           | 331               |
| Carbon dioxide                | 259               |
| Oxygen                        | 316               |
| Helium                        | 965               |
| Hydrogen                      | 1290              |
|                               |                   |
| **Liquids at $20 \degree C$** |                   |
| Ethanol                       | 1160              |
| Mercury                       | 1450              |
| Water, fresh                  | 1480              |
| Sea Water                     | 1540              |
| Human tissue                  | 1540              |
|                               |                   |
| **Solids**                    |                   |
| Vulcanized rubber             | 54                |
| Polyethylene                  | 920               |
| Marble                        | 3810              |
| Glass, Pyrex                  | 5640              |
| Lead                          | 1960              |
| Aluminum                      | 5120              |
| Steel                         | 5960              |

Through the continuity equation, we can set the mass flow rate entering the volume is equal to the mass flow rate leaving the volume.

![[sound_wave.jpg|align:center|300]]

$$
\frac{\mathrm{d} m}{\mathrm{d} t} = \frac{\mathrm{d} (\rho A x)}{\mathrm{d} t} = \rho A \frac{\mathrm{d} x}{\mathrm{d} t} = \rho A v 
\hspace{1cm} \Rightarrow \hspace{1cm} 
\begin{aligned}[t]
	\rho A v &= (\rho + \mathrm{d} \rho) A (v + \mathrm{d} v) \\
	\rho v &= (\rho + \mathrm{d} \rho) (v + \mathrm{d} v) \\
	\rho v &= \rho v + \rho \, \mathrm{d} v + v \, \mathrm{d} \rho + \underbrace{\mathrm{d} \rho \, \mathrm{d} v}_{\approx 0} \\
	0 &= \rho \, \mathrm{d} v + v \, \mathrm{d} \rho \\
	\rho \, \mathrm{d} v &= - v \, \mathrm{d} \rho	
\end{aligned}
$$

Then, by using the definition of pressure with respect to force, we can find a relationship between velocity and pressure.

$$
\begin{align}
	P = \frac{F}{A} \hspace{1cm} \Rightarrow \hspace{1cm} a = \frac{\mathrm{d} v}{\mathrm{d} t} = - \frac{\mathrm{d} P \, (\mathrm{d} x \, \mathrm{d} y)}{m} &= - \frac{\mathrm{d} P \, (\mathrm{d} y \, \mathrm{d} z)}{\rho \, (\mathrm{d} x \, \mathrm{d} y \, \mathrm{d} z)} = - \frac{\mathrm{d} P}{\rho \, \mathrm{d} x} \\
	\mathrm{d} v &= - \frac{\mathrm{d} P}{\rho} \frac{\mathrm{d} t}{\mathrm{d} x} \\
	\mathrm{d} v &= - \frac{\mathrm{d} P}{\rho} \frac{1}{v} \\
	\mathrm{d} P &= - \rho \, v \; \mathrm{d} v
\end{align}
$$

Bringing these two relationships together, we have a relationship for the speed of sound in terms of pressure ($P$) and density ($\rho$).

$$
\mathrm{d} P = - \rho \, v \; \mathrm{d} v = - v \left( - v \; \mathrm{d} \rho \right) = v^{2} \; \mathrm{d} \rho \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\;c_{\rm s} \equiv v = \sqrt{\frac{\mathrm{d} P}{\mathrm{d} \rho}} \;}
$$

### Supersonic

When the speed of something traveling through a medium is greater than the [[#Speed of Sound|speed of sound]] through that same medium.

$$v_{\rm supersonic} > c_{\rm s} = \sqrt{\frac{\mathrm{d} P}{\mathrm{d} \rho}}$$
