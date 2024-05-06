---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
## Conservation Laws

#### Conservation of Mass
*(Also known as **Continuity**)*

$$
\pd{\rho}{t} + \nabla \cdot \left( \rho \vec{v} \right) = 0
\hWhere 
\begin{aligned}[t]
	\rho &\equiv {\rm density} \\
	\vec{v} &\equiv {\rm fluid\ velocity}
\end{aligned}
$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hRightarrow \pd{\rho}{t} + \frac{1}{r^{2}} \pd{}{r} (r^{2} \rho v) = 0$$

#### Conservation of Momentum

$$
\pd{\vec{v}}{t} + (\vec{v} \cdot \nabla) \vec{v} + \frac{1}{\rho} \nabla P = \frac{1}{\rho} \vec{f}
\hWhere 
\begin{aligned}[t]
	P &\equiv {\rm pressure} \\
	\vec{f} &\equiv {\rm external\ force\ per\ volume} \\
	&\hspace{1cm} \textcolor{gray}{\left[ \vec{f}_{\rm grav} = -\nabla \Phi_{\rm g} \right]}
\end{aligned}
$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hRightarrow \pd{v}{t} + v \pd{v}{r} + \frac{1}{\rho} \pd{P}{r} = \frac{1}{\rho} f_{\rm r}$$

#### Conservation of Energy
 $$\pd{\epsilon}{t} + \nabla \cdot \left[ (\epsilon + P) \vec{v} \right] = 0 \hWhere \epsilon = \underbrace{\left( \frac{1}{2} \rho |\vec{v}|^{2} \right)}_{\substack{\text{dyanmical} \\ \text{energy density}}} + \underbrace{\left( \frac{3}{2} n k_{\rm B} T \right)}_{\substack{\text{gas} \\ \text{energy density}}} + \underbrace{\bigg( \rho \,\Phi_{\rm g} \bigg)}_{\substack{\text{gravitational} \\ \text{energy density}}}$$

> [!math] Spherical Symmetry
> $$\vec{v} = v \, \hat{r} \quad,\quad \vec{f} = f \, \hat{r} \hRightarrow \pd{\epsilon}{t} + \frac{1}{r^{2}} \pd{}{r} \left[ r^{2} (\epsilon + P) v \right] = 0$$

## Ram Pressure

**Ram pressure** is a pressure exerted on a body moving through a fluid medium. This motion causes a drag force on the body, effectively transferring momentum from the fluid into the body. This is caused by the relative bulk motion of the fluid around the body, rather than random thermal motion. 

If we simplify the fluid mechanics and assume that all matter incident upon a surface transfers all of its momentum into the volume, this is equivalent to the matter "entering the volume" in terms of momentum transfer. Furthermore, if only the momentum perpendicular to the surface is transferred and we exclude shear forces, the maximum pressure exerted on that surface is...

$$
P_{\rm{ram}} = \rho v_{\rm n}^{2} \hWhere 
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

$$\boxed{\;c_{\rm s} \equiv v = \sqrt{\td{P}{\rho}} \;}$$

> [!atom] In an ideal gas, the equation for the speed of sound is...
>
> $$
> c_{\rm s} = \sqrt{\frac{\gamma R T}{M}} \hWhere 
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
\td{m}{t} = \td{(\rho A x)}{t} = \rho A \td{x}{t} = \rho A v 
\hRightarrow 
\begin{aligned}[t]
	\rho A v &= (\rho + \rd \rho) A (v + \rd v) \\
	\rho v &= (\rho + \rd \rho) (v + \rd v) \\
	\rho v &= \rho v + \rho \, \rd v + v \, \rd \rho + \underbrace{\rd \rho \, \rd v}_{\approx 0} \\
	0 &= \rho \, \rd v + v \, \rd \rho \\
	\rho \, \rd v &= - v \, \rd \rho	
\end{aligned}
$$

Then, by using the definition of pressure with respect to force, we can find a relationship between velocity and pressure.

$$
\begin{align}
	P = \frac{F}{A} \hRightarrow a = \td{v}{t} = - \frac{\rd P \, (\rd x \, \rd y)}{m} &= - \frac{\rd P \, (\rd y \, \rd z)}{\rho \, (\rd x \, \rd y \, \rd z)} = - \frac{\rd P}{\rho \, \rd x} \\
	\rd v &= - \frac{\rd P}{\rho} \td{t}{x} \\
	\rd v &= - \frac{\rd P}{\rho} \frac{1}{v} \\
	\rd P &= - \rho \, v \; \rd v
\end{align}
$$

Bringing these two relationships together, we have a relationship for the speed of sound in terms of pressure ($P$) and density ($\rho$).

$$
\rd P = - \rho \, v \; \rd v = - v \left( - v \; \rd \rho \right) = v^{2} \; \rd \rho \hRightarrow \boxed{\;c_{\rm s} \equiv v = \sqrt{\td{P}{\rho}} \;}
$$

### Supersonic

When the speed of something traveling through a medium is greater than the [[#Speed of Sound|speed of sound]] through that same medium.

$$v_{\rm supersonic} > c_{\rm s} = \sqrt{\td{P}{\rho}}$$
