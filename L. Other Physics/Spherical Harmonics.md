---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
The **spherical harmonic** are defined as special set of orthonormal functions that solve the Laplace Equation on the surface of a sphere. The Laplacian can be defined as:

$$\begin{alignat}{2}
&\textbf{Cartesian: } \hspace{0.2cm} &&\vec{\nabla}^{2} = \frac{\partial^{2} }{\partial x^{2}} + \frac{\partial^{2} }{\partial y^{2}} + \frac{\partial^{2} }{\partial z^{2}} \\
&\textbf{Cylindrical: } \hspace{0.2cm} &&\vec{\nabla}^{2} = \frac{1}{r} \frac{\partial }{\partial r} \left( r \frac{\partial }{\partial r} \right) + \frac{1}{r^{2}} \frac{\partial^{2} }{\partial \theta^{2}} + \frac{\partial^{2} }{\partial z^{2}} \\
&\textbf{Spherical: } \hspace{0.2cm} &&\vec{\nabla}^{2} = \frac{1}{r^{2}} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial }{\partial r} \right) + \frac{1}{r^{2} \sin{\theta}} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial }{\partial \theta} \right) + \frac{1}{r^{2} \sin^{2}\theta} \left( \frac{\partial^{2} }{\partial \phi^{2}} \right)
\end{alignat}$$

Below, we derive the harmonics ($Y_{l}^{m}$) through the separation of variables.

$$
\left( -\frac{\hbar^{2}}{2 m} \vec{\nabla}^{2} + V(r) \right) \Psi = E \Psi \hspace{1cm} \Rightarrow \hspace{1cm} \vec{\nabla}^{2} \Psi = - \frac{2 m (E-V(r))}{\hbar^{2}} \Psi
$$

## The Angular Equation
### Step 1 - Separation of Variables (Radial & Angular)

$$\Psi(r, \theta, \phi) = R(r) Y(\theta, \phi) = R Y \hspace{1cm} \Rightarrow \hspace{1cm} \vec{\nabla}^{2} \Psi = \vec{\nabla}^{2} R Y = 0$$

$$\begin{align}
\frac{1}{r^{2}} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial \Psi}{\partial r} \right) &+ \frac{1}{r^{2} \sin{\theta}} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Psi}{\partial \theta} \right) + \frac{1}{r^{2} \sin^{2}\theta} \left( \frac{\partial^{2} \Psi}{\partial \phi^{2}} \right) = 0 \\
\frac{Y}{r^{2}} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) &+ \frac{R}{r^{2} \sin{\theta}} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial Y}{\partial \theta} \right) + \frac{R}{r^{2} \sin^{2}\theta} \left( \frac{\partial^{2} Y}{\partial \phi^{2}} \right) = 0 \\
-\left[ \frac{1}{R} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) \right] &= \left[ \frac{1}{Y \sin \theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial Y}{\partial \theta} \right) + \frac{1}{Y \sin^{2}\theta} \left( \frac{\partial^{2} Y}{\partial \phi^{2}} \right) \right] = -\lambda
\end{align}$$

Here, we have set the separation constant to be $-\lambda$ such that we can solve for each equation individually. For now, we focus on the angular equation $Y(\theta, \phi)$ and save the radial equation for later.

### Step 2 - Separation of Variables (Azimuthal & Polar)

Separating the azimuthal and polar angle coordinates through a second implementation of a separation of variables...

$$Y(\theta, \phi) = \Theta(\theta)\Phi(\phi) = \Theta \Phi$$

$$\begin{align}
\left[ \frac{1}{Y \sin \theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial Y}{\partial \theta} \right) + \frac{1}{Y \sin^{2}\theta} \left( \frac{\partial^{2} Y}{\partial \phi^{2}} \right) \right] &= -\lambda \\
\sin \theta \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial Y}{\partial \theta} \right) + \left( \frac{\partial^{2} Y}{\partial \phi^{2}} \right) &= -\lambda Y \sin^{2} \theta \\
\Phi \sin \theta \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \left(\Theta \frac{\partial^{2} \Phi}{\partial \phi^{2}} \right) &= -\lambda \Theta \Phi \sin^{2} \theta \\
\frac{\sin \theta}{\Theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \left( \frac{1}{\Phi} \frac{\partial^{2} \Phi}{\partial \phi^{2}} \right) &= -\lambda \sin^{2} \theta \\
\left[ \frac{\sin \theta}{\Theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \lambda \sin^{2} \theta \right] &= - \left[ \frac{1}{\Phi} \frac{\partial^{2} \Phi}{\partial \phi^{2}} \right] = m^{2}
\end{align}$$

Here, we have set the separation constant to be $m^{2}$ for simple solving of the azimuthal differential equation.

### Step 3 - Azimuthal Equation

$$\begin{align}
- \left[ \frac{1}{\Phi} \frac{\partial^{2} \Phi}{\partial \phi^{2}} \right] = m^{2} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\partial^{2} \Phi}{\partial \phi^{2}} &= -m^{2} \Phi \\
\Phi &= A e^{i m \phi} + B e^{-i m \phi} \rightarrow e^{i m \phi}
\end{align}$$

If we allow $m$ to be positive and negative, we can drop one of the terms, and additional coefficient will absorbed into the Polar D.E. solution $\Theta(\theta)$. 

Then, since we are working in spherical coordinates, we must apply the periodic boundary condition. 

$$\Phi(\phi) = \Phi(\phi+2\pi) \hspace{1cm} \Rightarrow \hspace{1cm} e^{i m \phi} = e^{i m (\phi + 2 \pi)} \text{,} \hspace{0.5cm} m \in \mathbb{Z}$$

Here, we find that $m$ must be an integer.

### Step 4 - Polar Equation

Here, we will now use the Associated Legendre Functions $P_{l}^{m}(\cos \theta)$ to solve for the polar equation.

$$\begin{alignat}{2}
\left[ \frac{\sin \theta}{\Theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \lambda \sin^{2} \theta \right] &= m^{2} && \\
\frac{\sin \theta}{\Theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \left[ \lambda \sin^{2} \theta - m^{2} \right] &= 0 \\
\frac{1}{\sin \theta} \frac{\partial }{\partial \theta} \left( \sin \theta \frac{\partial \Theta}{\partial \theta} \right) + \left[ \lambda - \frac{m^{2}}{\sin^{2}\theta} \right] \Theta &= 0
\end{alignat}$$

This differential equation is of a specific form in mathematics that leads to the *Associated Legendre Functions*.

$$
\frac{\mathrm{d} }{\mathrm{d} x}\left[(1-x^{2})\frac{\mathrm{d} y}{\mathrm{d} x}\right] + \left[l(l+1) - \frac{m^{2}}{1-x^{2}}\right] y = 0 \hspace{1cm} \Rightarrow \hspace{1cm} y = P_{l}^{m}(x)
$$

$$\begin{alignat}{2}
&\underline{\text{Associated Legendre Functions: }} \hspace{0.5cm} &&P_{l}^{m}(x) \equiv (-1)^{m} (1-x^{2})^{m/2} \left( \frac{\mathrm{d} }{\mathrm{d} x} \right)^{m} P_{l}(x)\\
&\underline{\text{Legendre Polynomials: }} &&P_{l}(x) \equiv \frac{1}{2^{l} l!} \left( \frac{\mathrm{d} }{\mathrm{d} x} \right)^{l} (x^{2}-1)^{l}
\end{alignat}$$

If we take $x = \cos \theta$ and $y = \Theta$, we can showcase this form such that $\lambda = l(l+1)$, $l \in +\mathbb{Z}$.

$$\begin{align}
\frac{\mathrm{d} }{\mathrm{d} (\cos\theta)}\left[(\sin^{2}\theta)\frac{\mathrm{d} \Theta}{\mathrm{d} (\cos\theta)}\right] + \left[l(l+1) - \frac{m^{2}}{\sin^{2}\theta}\right] \Theta &= 0\\
\frac{1}{\sin\theta}\frac{\mathrm{d} }{\mathrm{d} \theta}\left[(\sin\theta)\frac{\mathrm{d} y}{\mathrm{d} (\theta)}\right] + \left[l(l+1) - \frac{m^{2}}{\sin^{2}\theta}\right] \Theta &= 0
\end{align}$$

By this, we know the solution form of the Polar Equation will be:

$$
\Theta(\theta) \sim P_{l}^{m}(\cos \theta) \hspace{1cm} l \in + \mathbb{Z}
$$

We note, for $m>l$, the associated Legendre function is $P_{l}^{m}(\cos\theta) = 0$. Therefore, we can restrict the domain of $m$ such that are $(2l+1)$ possibilities given any $l$.

$$
l = 0, 1, 2 \dots \hspace{1cm} m = -l, -l+1, \dots, -1, 0, 1, \dots, l-1, l
$$

### Step 5 - Normalize Angular Equation

$$\int (Y_{l}^{m})^{*} Y_{l}^{m} dV = 1$$

Though the algebraic details are not expressed, the normalization constant is found via the normal integration:

$$\begin{align}
&Y_{l}^{m} = \mathcal{N} P_{l}^{m}(\cos\theta) e^{i m \phi} \\
&\int (Y_{l}^{m})^{*} Y_{l}^{m} (r^{2} \sin\theta dr d\theta d\phi) = 1 \hspace{1cm} \Rightarrow \hspace{1cm} \mathcal{N} = (-1)^{m} \sqrt{\frac{(2l+1)}{4 \pi} \frac{(l-m)!}{(l+m)!}}
\end{align}$$

### The Spherical Harmonics

$$\begin{align}
	\boxed{Y_{l}^{m}(\theta, \phi) = \left[ (-1)^{m} \sqrt{\frac{(2l+1)}{4 \pi} \frac{(l-m)!}{(l+m)!}} \right] P_{l}^{m}(\cos \theta) e^{i m \phi} \hspace{1cm} \text{where} \hspace{1cm}
	\begin{aligned}
		l &\in +\mathbb{Z} \\
		m &\in \{ -l \le m \le l \, | \, \mathbb{Z} \}
	\end{aligned}}
\end{align}$$

## The Radial Equation, V(r)

Using the differential defined the the first separation of variables [[#Step 1 - Separation of Variables (Radial & Angular)|here]], we can solve for a [[#Homogeneous Laplace Equation]] or a [[#Non-Homogeneous Laplace Equation]].

### Homogeneous Laplace Equation

Assume a power law in radius: $R(r) = \sum_{s} c_{s} r^{s}$...

$$\begin{align}
    -\left[ \frac{1}{R} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) \right] &= -\lambda \\
    \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) &= \lambda R \\
    2 r \frac{\partial R}{\partial r} + r^{2} \frac{\partial^{2} R}{\partial r^{2}} - \lambda R &= 0 \\
    \frac{\partial^{2} R}{\partial r^{2}} + \left(\frac{2}{r}\right) \frac{\partial R}{\partial r} + \left(\frac{-\lambda}{r^{2}}\right) R &= 0 \\
    \sum_{s} c_{s} \left[ s (s-1) r^{s-2} + \left(\frac{2}{r}\right) s r^{s-1} + \left(\frac{-\lambda}{r^{2}}\right) r^{s} \right] &= 0 \\
    \sum_{s} c_{s} r^{s-2} \left[ s (s-1) + 2 s - \lambda \right] &= 0 \\
    s (s-1) + 2 s - \lambda &= 0 \\
    \lambda &= s(s+1)
\end{align}$$

Combine with [[#Step 4 - Polar Equation|Polar Equation]] results of an integer integration constant ($\ell$).

$$\begin{align}
    \lambda = s (s +1) &= l (l+1) \hspace{2cm} l \in +\mathbb{Z} \\
    s^{2} + s &= l^{2} + l \\
    s^{2} + s + \frac{1}{4} &= l^{2} + l + \frac{1}{4} \\
    \left( s + \frac{1}{2} \right)^{2} &= \left( l +\frac{1}{2} \right)^{2} \\
    s + \frac{1}{2} &= \pm \left( l +\frac{1}{2} \right) \\
    & \nonumber \\
    \therefore s + \frac{1}{2} &= + \left( l +\frac{1}{2} \right) \hspace{0.5cm} \rightarrow \hspace{0.5cm} s = l \\
    \therefore s + \frac{1}{2} &= - \left( l +\frac{1}{2} \right) \hspace{0.5cm} \rightarrow \hspace{0.5cm} s = - l - 1    
\end{align}$$

Given we assume a power series structure, the radial equation can be reduced to two terms. However, given $r<0$ is undefined, the second term also drops.

$$R(r) = \sum_{s} c_{s} \, r^{s} = a \, r^{l} + b \, r^{-(l+1)} \hspace{1cm} \Rightarrow R(r) \sim r^{l}$$

This would then simply mix the radial factor into the [[#The Spherical Harmonics|spherical harmonics]] equation.

$$\begin{align}
    \boxed{ \; Y_{l}^{m}(\theta, \phi) = \left[ (-1)^{m} \sqrt{\frac{(2l+1)}{4 \pi} \frac{(l-m)!}{(l+m)!}} \right] P_{l}^{m}(\cos \theta) e^{i m \phi} r^{l} \; } \hspace{1cm} \text{where} \hspace{1cm} 
    \begin{aligned}
        l &\in +\mathbb{Z} \\
        m &\in \{ -l \le m \le l \, | \, \mathbb{Z} \}
    \end{aligned}
\end{align}$$

### Non-Homogeneous Laplace Equation

If the Laplace equation is non-homogeneous and the potential is radially dependent $V(r)$, then we must use a different method of solving. 

Our non-homogeneous Laplace equation, with a general potential $V(r)$, will take on the form of:
$$\begin{align}
    - \left[ \frac{1}{R} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) + \left(\frac{2 m (E - V)}{\hbar^{2}}\right) r^{2} \right] &= -\lambda \\
    - \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) + \left(\left(\frac{2 m V}{\hbar^{2}}\right) r^{2} + \lambda \right) R &= \frac{2 m E}{\hbar^{2}} r^{2} R \\
    - \frac{\hbar^{2}}{2 m} \frac{\partial }{\partial r} \left( r^{2} \frac{\partial R}{\partial r} \right) + \left(V r^{2} + \frac{\hbar^{2}}{2 m} \lambda \right) R &= E r^{2} R
\end{align}$$

By setting $u(r) = r R(r)$ such that $\frac{\partial R}{\partial r} = \frac{r u' - u}{r^{2}}$, we can restructure the expression in a way that is more familiar.

$$\begin{align}
    - \frac{\hbar^{2}}{2 m} \frac{\partial }{\partial r} \left( r \frac{\partial u}{\partial r} - u \right) + \left(V r^{2} + \frac{\hbar^{2}}{2 m} \lambda \right) \frac{u}{r} &= E r u \\
    - \frac{\hbar^{2}}{2 m} \left( \frac{\partial u}{\partial r} + r \frac{\partial^{2} u}{\partial r^{2}} - \frac{\partial u}{\partial r} \right) + \left(V r^{2} + \frac{\hbar^{2}}{2 m} \lambda \right) \frac{u}{r} &= E r u \\
    - \frac{\hbar^{2}}{2 m} \frac{\partial^{2} u}{\partial r^{2}} + \left(V + \frac{\hbar^{2}}{2 m} \frac{\lambda}{ r^{2}} \right) u &= E u \\
    \left[ - \frac{\hbar^{2}}{2 m} \frac{\partial^{2} }{\partial r^{2}} + \left(V + \frac{\hbar^{2}}{2 m} \frac{\lambda}{ r^{2}} \right) \right] u &= E u \\
    \left[ - \frac{\hbar^{2}}{2 m} \frac{\partial^{2} }{\partial r^{2}} + V_{eff} \right] u &= E u
\end{align}$$

From this, we can see the emergence of an *effective potential* where the extra term represents the *centrifugal effects*, moving the particle away from the origin. Given we know $\lambda$ from the angular equation, we can represent the final radial equation (without knowing the potential) as:

$$\boxed{ \,\left[ - \frac{\hbar^{2}}{2 m} \frac{\partial^{2} }{\partial r^{2}} + \left(V + \frac{\hbar^{2}}{2 m} \frac{l (l+1)}{ r^{2}} \right) \right] u = E u \,}$$

From here, we can normalize the radial equation using the standard integral: $\int u^{*}u dr = 1$. 

> [!note] Normalization
> 
> The normalization of the radial equation is not dependent on the normalization of the angular equation. This is because of the separation of variables. Therefore, when we combine them together in the end ($\Psi = R(r) Y(\theta, \phi)$), we are effectively multiplying $1*1$.