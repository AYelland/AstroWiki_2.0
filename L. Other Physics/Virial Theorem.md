---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---

> [!key-idea] 
> The **Virial Theorem** relates the time average kinetic energy and time averaged potential energy of a stable system composed of discrete particles, bound by a conservative force.
> $$
> \boxed{\left\langle T \right\rangle = -\frac{1}{2} \left\langle \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} \right\rangle}
> \hspace{1cm} \xRightarrow{{\rm if} \; U \, \propto \, r^{n}} \hspace{1cm}
> \left\langle E \right\rangle = \left( 1 + \frac{n}{2} \right) \left\langle U \right\rangle \quad , \quad 2 \left\langle T \right\rangle - n \left\langle U \right\rangle = 0
> $$
> 
> The two important assumptions for the Virial Theorem to hold true are:
> - $F$ is a pairwise force.
> - We have a steady state time averaged quantity $\frac{\mathrm{d}^{2} I}{\mathrm{d} t^{2}} = 0$.

## Derivation

Let us assume that we have $N$ particles (e.g. stars in galaxy) with mass, position, and velocity $(m_{i}, \vec{r}_{i}, \vec{v}_{i})$. We can then define the virial scalar angular momentum $L$ as...

$$\begin{align}
    L &= \sum_{i} \vec{p}_{i} \cdot \vec{r}_{i} \\
    &= \sum_{i} \left( m_{i} \frac{\mathrm{d} \vec{r}_{i}}{\mathrm{d} t} \right) \cdot \vec{r}_{i} 
        \textcolor{gray}{\hspace{1cm} \text{where} \hspace{1cm} \frac{\mathrm{d}}{\mathrm{d} t}(\vec{r} \cdot \vec{r}) = \dot{\vec{r}} \cdot \vec{r} + \vec{r} \cdot \dot{\vec{r}} = 2\dot{\vec{r}}\ \vec{r}} \\
    &= \frac{1}{2}\sum_{i} m_{i} \frac{\mathrm{d}}{\mathrm{d} t} (\vec{r}_{i} \cdot \vec{r}_{i}) \\
    &= \frac{1}{2} \frac{\mathrm{d} }{\mathrm{d} t} \underbrace{\sum_{i} m_{i} r_{i}^{2}}_{\equiv \, I} \hspace{1.5cm} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{L= \frac{1}{2}\frac{\mathrm{d} I}{\mathrm{d} t}}
\end{align}$$
...where $I = \sum_{i} m_{i} r_{i}^{2}$ is the moment of inertia about the origin. 

If we then take the the time derivative of $L$, we can identify a *two-body force* component and a *kinetic energy* component.
$$
\begin{align}
    \frac{\mathrm{d} L}{\mathrm{d} t} &= \sum_{i} \dot{\vec{p}}_{i} \cdot \vec{r}_{i} + \sum_{i} \vec{p} \cdot \dot{\vec{r}}_{i} \\
    &= \sum_{i} \vec{F}_{i} \cdot \vec{r_{i}} + \sum_{i} m_{i} v_{i}^{2} \\
    &= \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} + 2 T 
        \hspace{1cm} \text{where} \hspace{1cm} T \equiv \text{kinetic energy}
\end{align}
$$

Then taking the time-average of a steady state system ($\tau$ is large)
$$\left\langle \frac{\mathrm{d} L}{\mathrm{d} t} \right\rangle_{\tau} = \frac{1}{\tau} \int_{0}^{\tau} \frac{\mathrm{d} L}{\mathrm{d} t} \mathrm{d} t = \frac{L(\tau) - L(0)}{\tau} \approx 0$$
...we find the **Virial Theorem**.
$$\left\langle\frac{\mathrm{d} L}{\mathrm{d} t}\right\rangle = \left\langle \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} \right\rangle + \left\langle 2 \, T \right\rangle = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\left\langle T \right\rangle = - \frac{1}{2} \left\langle \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} \right\rangle}$$

### For a Pairwise Force...

Focusing on the first term containing the two-body force components (pairwise forces), we can re-express it in terms of a a matrix where $F_{j=k} = 0$ and $1 \le j,k \le N$. Splitting $F_{jk}$ into two parts, we can now evaluate the upper and lower portions of the matrix individually.

$$\vec{F}_{k} = \sum_{j=1}^{N} \vec{F}_{jk} (1 - \delta_{jk})
\hspace{1cm} \Rightarrow \hspace{1cm} F_{jk} = 
\begin{pmatrix}
	0 & & \require{enclose}\enclose{circle}{2} \\
	& \ddots & \\
	 \require{enclose}\enclose{circle}{1}& & 0
\end{pmatrix}
\hspace{1cm} \text{where} \hspace{1cm} (j, k) \equiv (\text{row}, \text{column})
$$
where
$$\require{enclose}\enclose{circle}{1} = \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k}
\hspace{1cm} {\rm and} \hspace{1cm}
\require{enclose}\enclose{circle}{2}= \sum_{k=1}^{N-1}\sum_{j=k+1}^{N} \vec{F}_{jk} \cdot \vec{r}_{k}$$

Adding these expressions together gives us the desired term in our $\frac{\mathrm{d} L}{\mathrm{d} r}$ equation.

$$\sum_{k=1}^{N}\vec{F}_{k} \cdot \vec{r}_{k} = \require{enclose}\enclose{circle}{1} + \require{enclose}\enclose{circle}{2} = \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{k=1}^{N-1} \sum_{j=k+1}^{N} \vec{F}_{kj} \cdot \vec{r}_{k} \right)$$

With the symmetry of a pairwise force, we know $-\vec{F}_{kj}=\vec{F}_{jk}$, such that we can simplify this above expression.
$$\begin{align}
    \sum_{k=1}^{N} \vec{F}_{k} \cdot \vec{r}_{k}
    &= \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{k=1}^{N-1} \sum_{j=k+1}^{N} \vec{F}_{kj} \cdot \vec{r}_{k} \right) \\
    &= \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{k=1}^{N-1} \sum_{j=k+1}^{N} \vec{F}_{kj} \cdot \vec{r}_{k} \right) \\
    &= \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{j=1}^{N-1}\sum_{k=j+1}^{N} \vec{F}_{jk} \cdot \vec{r}_{j} \right) \\
    &= \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{j} \right) \\
    &= \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot (\vec{r}_{k} - \vec{r}_{j})
\end{align}$$

In terms of some potential $V$, we find...

$$\vec{F}_{jk} = - \nabla_{k} V\left(|\vec{r}_{jk}|\right) = -\nabla_{k} V_{jk} = - \frac{\mathrm{d} V_{jk}}{\mathrm{d} r} \left(\frac{\vec{r}_{k} - \vec{r}_{j}}{r_{jk}}\right)$$
$$\Downarrow$$
$$\begin{align}
    \sum_{k=1}^{N} \vec{F}_{k} \cdot \vec{r}_{k} &= \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot(\vec{r}_{k}-\vec{r}_{j})\\
    &= -\sum_{k=2}^{N} \sum_{j=1}^{k-1} \left( \frac{\mathrm{d} V_{jk}}{\mathrm{d} r} \frac{|\vec{r}_{k}-\vec{r}_{j}|^{2}}{r_{jk}} \right) \\
    &= -\sum_{k=2}^{N} \sum_{j=1}^{k-1} \left( \frac{\mathrm{d} V_{jk}}{\mathrm{d} r} r_{jk} \right)
\end{align}$$

### For a Radially Exponential Potential

We now assume the potential is radially exponential.
$$V = V_{0} \, r^{n} \hspace{1cm} \Rightarrow \hspace{1cm} V_{jk}= V_{0} \, r_{jk}^{n}$$
Taking the appropriate derivatives, this gives...

$$\frac{\mathrm{d} V_{jk}}{\mathrm{d} r} = V_{0} \, n (r_{jk})^{n-1} 
\hspace{1cm} \Rightarrow \hspace{1cm} 
\frac{\mathrm{d} V_{jk}}{\mathrm{d} r} r_{jk} = n (V_{0} \, (r_{jk})^{n}) = n V_{jk}$$

$$
\begin{align}
    \sum_{k=1}^{N} \vec{F}_{k} \cdot \vec{r}_{k} = - \sum_{k=2}^{N} \sum_{j=1}^{k-1} n V_{jk} = - n \sum_{k-2}^{N} \sum_{j=1}^{k-1} V_{jk} = - n \, V_{\rm tot} \quad \equiv - n\,  U
\end{align}
$$

Bringing it all back together with the time-averaged equation (where  $U \equiv V_{\rm tot}$) ...

$$\left\langle \frac{\mathrm{d} L}{\mathrm{d} t} \right\rangle = \left\langle \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} \right\rangle + \left\langle 2 \, T \right\rangle = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{2 \left\langle T \right\rangle - n \left\langle U \right\rangle = 0}$$
