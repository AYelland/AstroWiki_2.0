---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---

> [!key-idea] 
> The **Virial Theorem** relates the time average kinetic energy and time averaged potential energy of a stable system composed of discrete particles, bound by a conservative force.
> $$
> \boxed{\expval{T} = -\frac{1}{2} \expval{\sum_{i} \vec{F}_{i} \cdot \vec{r}_{i}}}
> \hspace{1cm} \xRightarrow{{\rm if} \; U \, \propto \, r^{n}} \hspace{1cm}
> \expval{E} = \left( 1 + \frac{n}{2} \right) \expval{U} \quad , \quad 2 \expval{T} - n \expval{U} = 0
> $$
> 
> The two important assumptions for the Virial Theorem to hold true are:
> - $F$ is a pairwise force.
> - We have a steady state time averaged quantity $\tdd{I}{t} = 0$.

## Derivation

Let us assume that we have $N$ particles (e.g. stars in galaxy) with mass, position, and velocity $(m_{i}, \vec{r}_{i}, \vec{v}_{i})$. We can then define the virial scalar angular momentum $L$ as...

$$\begin{align}
    L &= \sum_{i} \vec{p}_{i} \cdot \vec{r}_{i} \\
    &= \sum_{i} \left( m_{i} \td{\vec{r}_{i}}{t} \right) \cdot \vec{r}_{i} 
        \textcolor{gray}{\hWhere \frac{\rd}{\rd t}(\vec{r} \cdot \vec{r}) = \dot{\vec{r}} \cdot \vec{r} + \vec{r} \cdot \dot{\vec{r}} = 2\dot{\vec{r}}\ \vec{r}} \\
    &= \frac{1}{2}\sum_{i} m_{i} \frac{\rd}{\rd t} (\vec{r}_{i} \cdot \vec{r}_{i}) \\
    &= \frac{1}{2} \td{}{t} \underbrace{\sum_{i} m_{i} r_{i}^{2}}_{\equiv \, I} \hspace{1.5cm} \hRightarrow \boxed{L= \frac{1}{2}\frac{\rd I}{\rd t}}
\end{align}$$
...where $I = \sum_{i} m_{i} r_{i}^{2}$ is the moment of inertia about the origin. 

If we then take the the time derivative of $L$, we can identify a *two-body force* component and a *kinetic energy* component.
$$
\begin{align}
    \td{L}{t} &= \sum_{i} \dot{\vec{p}}_{i} \cdot \vec{r}_{i} + \sum_{i} \vec{p} \cdot \dot{\vec{r}}_{i} \\
    &= \sum_{i} \vec{F}_{i} \cdot \vec{r_{i}} + \sum_{i} m_{i} v_{i}^{2} \\
    &= \sum_{i} \vec{F}_{i} \cdot \vec{r}_{i} + 2 T 
        \hWhere T \equiv \text{kinetic energy}
\end{align}
$$

Then taking the time-average of a steady state system ($\tau$ is large)
$$\expval{\td{L}{t}}_{\tau} = \frac{1}{\tau} \int_{0}^{\tau} \td{L}{t} \rd t = \frac{L(\tau) - L(0)}{\tau} \approx 0$$
...we find the **Virial Theorem**.
$$\expval{\td{L}{t}} = \expval{\sum_{i} \vec{F}_{i} \cdot \vec{r}_{i}} + \expval{2 \, T} = 0 \hRightarrow \boxed{\expval{T} = - \frac{1}{2} \expval{\sum_{i} \vec{F}_{i} \cdot \vec{r}_{i}}}$$

### For a Pairwise Force...

Focusing on the first term containing the two-body force components (pairwise forces), we can re-express it in terms of a a matrix where $F_{j=k} = 0$ and $1 \le j,k \le N$. Splitting $F_{jk}$ into two parts, we can now evaluate the upper and lower portions of the matrix individually.

$$\vec{F}_{k} = \sum_{j=1}^{N} \vec{F}_{jk} (1 - \delta_{jk})
\hRightarrow F_{jk} = 
\begin{pmatrix}
	0 & & \circled{2} \\
	& \ddots & \\
	 \circled{1}& & 0
\end{pmatrix}
\hWhere (j, k) \equiv (\text{row}, \text{column})
$$
where
$$\circled{1} = \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k}
\hspace{1cm} {\rm and} \hspace{1cm}
\circled{2}= \sum_{k=1}^{N-1}\sum_{j=k+1}^{N} \vec{F}_{jk} \cdot \vec{r}_{k}$$

Adding these expressions together gives us the desired term in our $\td{L}{r}$ equation.

$$\sum_{k=1}^{N}\vec{F}_{k} \cdot \vec{r}_{k} = \circled{1} + \circled{2} = \left( \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot \vec{r}_{k} \right) - \left( \sum_{k=1}^{N-1} \sum_{j=k+1}^{N} \vec{F}_{kj} \cdot \vec{r}_{k} \right)$$

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

$$\vec{F}_{jk} = - \nabla_{k} V\left(|\vec{r}_{jk}|\right) = -\nabla_{k} V_{jk} = - \td{V_{jk}}{r} \fpar{\vec{r}_{k} - \vec{r}_{j}}{r_{jk}}$$
$$\Downarrow$$
$$\begin{align}
    \sum_{k=1}^{N} \vec{F}_{k} \cdot \vec{r}_{k} &= \sum_{k=2}^{N} \sum_{j=1}^{k-1} \vec{F}_{jk} \cdot(\vec{r}_{k}-\vec{r}_{j})\\
    &= -\sum_{k=2}^{N} \sum_{j=1}^{k-1} \left( \td{V_{jk}}{r} \frac{|\vec{r}_{k}-\vec{r}_{j}|^{2}}{r_{jk}} \right) \\
    &= -\sum_{k=2}^{N} \sum_{j=1}^{k-1} \left( \td{V_{jk}}{r} r_{jk} \right)
\end{align}$$

### For a Radially Exponential Potential

We now assume the potential is radially exponential.
$$V = V_{0} \, r^{n} \hRightarrow V_{jk}= V_{0} \, r_{jk}^{n}$$
Taking the appropriate derivatives, this gives...

$$\td{V_{jk}}{r} = V_{0} \, n (r_{jk})^{n-1} 
\hRightarrow 
\td{V_{jk}}{r} r_{jk} = n (V_{0} \, (r_{jk})^{n}) = n V_{jk}$$

$$
\begin{align}
    \sum_{k=1}^{N} \vec{F}_{k} \cdot \vec{r}_{k} = - \sum_{k=2}^{N} \sum_{j=1}^{k-1} n V_{jk} = - n \sum_{k-2}^{N} \sum_{j=1}^{k-1} V_{jk} = - n \, V_{\rm tot} \quad \equiv - n\,  U
\end{align}
$$

Bringing it all back together with the time-averaged equation (where  $U \equiv V_{\rm tot}$) ...

$$\expval{\td{L}{t}} = \expval{\sum_{i} \vec{F}_{i} \cdot \vec{r}_{i}} + \expval{2 \, T} = 0 \hRightarrow \boxed{2 \expval{T} - n \expval{U} = 0}$$
