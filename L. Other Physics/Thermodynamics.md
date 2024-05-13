---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---
## Ideal Gas Law

The **ideal gas law** is the equation of state of a hypothetical ideal gas.
$$
\begin{aligned}
	&P V = n R T = N k_{\rm B} T \\
	\\
	&P = \rho \frac{R T}{M} = \frac{\rho}{\mu m_{\rm u}} k_{\rm B} T
\end{aligned}
 \hspace{1cm} \text{where} \hspace{1cm} \left \{ \; \; 
\begin{aligned}
	P &\equiv \text{pressure} \\
	V &\equiv \text{volume} \\
	n &\equiv \text{number density} = N / N_{A} \quad [\ \mathit{moles}\ ] \\
	R &\equiv \text{ideal gas constant} = N_{A} \, k_{\rm B} = 8.314 \; {\rm J/(K\ mol)}\\
	T &\equiv \text{temperature} \\
\end{aligned} \right.
$$
**Assumptions:**
1. The particles/molecules in the gas are non-interacting (no intermolecular forces)
2. The particles/molecules do not take up any space, meaning their atomic volume is completely ignored

## Laws of Thermodynamics

> [!key-idea] Summary of the Laws
> 0) If two systems are in thermal equilibrium with a third, then all three systems are in thermal equilibrium.
> 1) Energy cannot be created or destroyed
> 2) For a spontaneous process, the entropy of the universe increases.
> 3) A perfect crystal at absolute zero ($T = 0 \; {\rm K}$) has zero entropy ($S(T) = 0$).

### 0th Law of Thermodynamics

![[thermoLaw0.png|align:center|400]]

*If two systems, $A$ and $B$, are separately in equilibrium with a third system, $C$, then they are also in equilibrium with each other.*

### 1st Law of Thermodynamics

![[thermoLaw1.png|align:center|400]]

$$
\mathrm{d} U = \rm d \hspace{-0.16em}\bar{}\hspace{0.2em} Q + \rm d \hspace{-0.16em}\bar{}\hspace{0.2em} W
\hspace{1cm} \text{where} \hspace{1cm}
\rm d \hspace{-0.16em}\bar{}\hspace{0.2em} Q = \sum_{i} T_{i} \, \mathrm{d} S_{i}
\hspace{1cm}
\rm d \hspace{-0.16em}\bar{}\hspace{0.2em} W = \sum_{i} J_{i} \, \mathrm{d} x_{i}
$$

*Energy cannot be created or destroyed in an adiabatically isolated system. For any transfer of energy in or out of the system (as work, heat, or matter), the system's internal energy changes in accordance with the law of conservation of energy.*

Above, $J_{i}$ and $x_{i}$ represent generalized forces and displacements, respectively. Some examples of such quantities are:

![[thermoLaw1-forces.png|align:center|450]]

### 2nd Law of Thermodynamics

![[thermoLaw2.jpeg|align:center|450]]

*The sum of the entropies of the interacting thermodynamic systems never decreases in an adiabatically isolated universe.*

$$\Delta Q = T \; \Delta S \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} Q = T \; \mathrm{d} S$$

**Common Corollaries:**
- A common corollary is that heat does not spontaneously pass from a colder body to a warmer body.
- **Kelvin’s statement:** There is no physical process is possible whose sole result is the complete conversion of heat into work. *(i.e. no perfect machine)*
- **Clausius’s statement.** No process is possible whose sole result is the transfer of heat from a colder to a hotter body. *(i.e. no perfect refrigerator)*

### 3rd Law of Thermodynamics

![[thermoLaw3.png|align:center|450]]

$$S(T = 0 \; {\rm K}) = 0$$
*The entropy of all systems at zero absolute temperature is a universal constant that can be taken to be zero.*


## Free Energy Equations

> [!key-idea] Thermodynamic Identities
> $$
> \begin{align}
> 	&\textbf{Total Energy ($U$):} &\hspace{1cm} \mathrm{d} U &= T \, \mathrm{d} S + J \, \mathrm{d} x \\
> 	&\textbf{Enthalpy Energy ($H$):} &\hspace{1cm} \mathrm{d} H &= T \, \mathrm{d} S - x \, \mathrm{d} J \\
> 	&\textbf{Helmholtz Energy ($F$):} &\hspace{1cm} \mathrm{d} F &= - S \, \mathrm{d} T + J \, \mathrm{d} x \\
> 	&\textbf{Gibbs Energy ($G$):} &\hspace{1cm} \mathrm{d} G &= - S \, \mathrm{d} T - x \, \mathrm{d} J 
> \end{align}
> $$
^thermoIDs

**Total Energy ($U$):** *(See [[#2nd Law of Thermodynamics]])*

$$
\mathrm{d} U = \rm d \hspace{-0.16em}\bar{}\hspace{0.2em} Q + \rm d \hspace{-0.16em}\bar{}\hspace{0.2em} W = T \, \mathrm{d} S  + J \, \mathrm{d} x \quad \textcolor{gray}{( + \mu \, \mathrm{d} N + \dots)} 
$$

$$
\begin{alignat}{4}
	&\textbf{Enthalpy ($H$):} &\hspace{1cm} H &= U - J x &\hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} H &= \mathrm{d} U - x \, \mathrm{d} J - J \, \mathrm{d} x \\
		&&&& \mathrm{d} H &= \left( T \, \mathrm{d} S + J \, \mathrm{d} x \right) - x \, \mathrm{d} J - J \, \mathrm{d} x \\
		&&&& \mathrm{d} H &= T \, \mathrm{d} S - x \, \mathrm{d} J \quad \textcolor{gray}{( + \mu \, \mathrm{d} N + \dots)} \\
		\\
	&\textbf{Helmholtz ($F$):} &\hspace{1cm} F &= U - T S &\hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} F &= \mathrm{d} U - S \, \mathrm{d} T - T \, \mathrm{d} S \\
		&&&& \mathrm{d} F &= \left( T \, \mathrm{d} S + J \, \mathrm{d} x \right) - S \, \mathrm{d} T - T \, \mathrm{d} S \\
		&&&& \mathrm{d} F &= - S \, \mathrm{d} T + J \, \mathrm{d} x \quad \textcolor{gray}{( + \mu \, \mathrm{d} N + \dots)} \\
		\\
	&\textbf{Gibbs ($G$):} &\hspace{1cm} G &= U - J x - T S &\hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} G &= \mathrm{d} U - x \, \mathrm{d} J - J \, \mathrm{d} x - S \, \mathrm{d} T - T \, \mathrm{d} S \\
		&&&& \mathrm{d} G &= \left( T \, \mathrm{d} S + J \, \mathrm{d} x \right) - x \, \mathrm{d} J - J \, \mathrm{d} x - S \, \mathrm{d} T - T \, \mathrm{d} S \\
		&&&& \mathrm{d} G &= - S \, \mathrm{d} T - x \, \mathrm{d} J \quad \textcolor{gray}{( + \mu \, \mathrm{d} N + \dots)} \\
		\\
\end{alignat}
$$

> [!note] Partial Derivative Relationships
> 
> By rearranging the **Thermodynamic Identities**, you can find the relationships between the partial derivatives of the various free energies ($U$, $F$, $H$, $G$) w.r.t. the natural variables ($S$, $T$, $J$, $x$, $N$, $\mu$, $\dots$). By choosing to keep certain values constant, you can find the following relationships.
> $$
> \begin{alignat}{3}
> 	\left( \frac{\partial U}{\partial S} \right)_{x, N, \dots} &= T &\hspace{1.5cm} \left( \frac{\partial U}{\partial x} \right)_{S, N, \dots} &= J \\
> 	\left( \frac{\partial H}{\partial S} \right)_{J, N, \dots} &= T &\hspace{1.5cm} \left( \frac{\partial H}{\partial J} \right)_{S, N, \dots} &= -x \\
> 	\left( \frac{\partial F}{\partial T} \right)_{x, N, \dots} &= -S &\hspace{1.5cm} \left( \frac{\partial F}{\partial x} \right)_{T, N, \dots} &= J\\
> 	\left( \frac{\partial G}{\partial T} \right)_{J, N, \dots} &= -S &\hspace{1.5cm} \left( \frac{\partial G}{\partial J} \right)_{T, N, \dots} &= -x
> \end{alignat}
> $$

^partialDerivativeRelationships


## Maxwell Relations

By reordering the second derivatives of each free energy value, we can find the **Maxwell Relations** between the natural variables.

$$
\begin{alignat}{3}
	&\require{enclose}\enclose{circle}{1} &\hspace{1cm} \left( \frac{\partial T}{\partial x} \right)_{S} &= \left( \frac{\partial J}{\partial S} \right)_{x} \\
	\\
	&\require{enclose}\enclose{circle}{2} &\hspace{1cm} \left( \frac{\partial J}{\partial T} \right)_{x} &= - \left( \frac{\partial S}{\partial x} \right)_{T} \\
	\\
	&\require{enclose}\enclose{circle}{3} &\hspace{1cm} \left( \frac{\partial T}{\partial J} \right)_{S} &= - \left( \frac{\partial x}{\partial S} \right)_{J} \\
	\\
	&\require{enclose}\enclose{circle}{4} &\hspace{1cm} \left( \frac{\partial x}{\partial T} \right)_{J} &= \left( \frac{\partial S}{\partial J} \right)_{T} \\
\end{alignat}
$$

> [!derivation]
> Beginning with the free energy relationships, we can rearrange the expressions for the first partial derivatives with respect to constant natural variables. *(See [[#^partialDerivativeRelationships|Partial Derivative Relationships]])*
> $$
> \begin{alignat}{3}
> 	\left( \frac{\partial U}{\partial S} \right)_{x} &= T &\hspace{1.5cm} \left( \frac{\partial U}{\partial x} \right)_{S} &= J \\
> 	\left( \frac{\partial H}{\partial S} \right)_{J} &= T &\hspace{1.5cm} \left( \frac{\partial H}{\partial J} \right)_{S} &= -x \\
> 	\left( \frac{\partial F}{\partial T} \right)_{x} &= -S &\hspace{1.5cm} \left( \frac{\partial F}{\partial x} \right)_{T} &= J\\
> 	\left( \frac{\partial G}{\partial T} \right)_{J} &= -S &\hspace{1.5cm} \left( \frac{\partial G}{\partial J} \right)_{T} &= -x
> \end{alignat}
> $$
> Taking the second derivative of these expressions, we can compare their resulting answers by using the *commutative property of partial derivative* (i.e. the order in which partial derivatives act doesn't matter).
> $$
> \begin{alignat}{3}
> 	\left( \frac{\partial U}{\partial S \, \partial x} \right)_{x, S} &= \left( \frac{\partial T}{\partial x} \right)_{S} &\hspace{1.5cm} \left( \frac{\partial U}{\partial x \, \partial S} \right)_{S, x} &= \left( \frac{\partial J}{\partial S} \right)_{x} \\
> 	\left( \frac{\partial H}{\partial S \, \partial J} \right)_{J, S} &= \left( \frac{\partial T}{\partial J} \right)_{S} &\hspace{1.5cm} \left( \frac{\partial H}{\partial J \, \partial S} \right)_{S, J} &= -\left( \frac{\partial x}{\partial S} \right)_{J} \\
> 	\left( \frac{\partial F}{\partial T \, \partial x} \right)_{x, T} &= -\left( \frac{\partial S}{\partial x} \right)_{T} &\hspace{1.5cm} \left( \frac{\partial F}{\partial x \, \partial T} \right)_{T, x} &= \left( \frac{\partial J}{\partial T} \right)_{x}\\
> 	\left( \frac{\partial G}{\partial T \, \partial J} \right)_{J, T} &= -\left( \frac{\partial S}{\partial J} \right)_{T} &\hspace{1.5cm} \left( \frac{\partial G}{\partial J \, \partial T} \right)_{T, J} &= -\left( \frac{\partial x}{\partial T} \right)_{J}
> \end{alignat}
> $$
> This directly yield the **Maxwell Equations**, by reading each line...
> $$
> \begin{align}
> 	\left( \frac{\partial T}{\partial x} \right)_{S} &= \left( \frac{\partial J}{\partial S} \right)_{x} \\
> 	\left( \frac{\partial J}{\partial T} \right)_{x} &= - \left( \frac{\partial S}{\partial x} \right)_{T} \\
> 	\left( \frac{\partial T}{\partial J} \right)_{S} &= - \left( \frac{\partial x}{\partial S} \right)_{J} \\
> 	\left( \frac{\partial x}{\partial T} \right)_{J} &= \left( \frac{\partial S}{\partial J} \right)_{T}
> \end{align}
> $$

## The Magic Square

![[magicSquare.png|align:center]]

To quickly recall all of the thermodynamic relationships, we can use the magic square. Here are the steps and necessary knowledge for this to be useful.

**For the [[#^thermoIDs|Thermodynamic Identities]]:**

![[magicSquare-identities.png|align:center]]

1. Choose one of the free-energy quantities (i.e. $U$, $H$, $F$, $G$) on the magic square.
	- *Example: Let us choose the Helmholtz Free Energy ($F$)*
2. The all of the variables sharing the same side of the magic square as the free-energy become differential. 
	- *Example: The free-energy variable ($F$), along with the two natural variables ($x$ and $T$) become differential variables.* $$F \to \mathrm{d} F \hspace{1cm} x \to \mathrm{d} x \hspace{1cm} T \to \mathrm{d} T$$
3. The opposite corners of the differential natural variables are the paired together. Following the positive-negative axis, you can determine the sign of the term.
	- *Example: Pairing up the terms, we can construct the final identity relationship.* $$\mathrm{d} x \to J \, \mathrm{d} x \hspace{1cm} \mathrm{d} T \to -S \, \mathrm{d} T \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\mathrm{d} F = J \, \mathrm{d} x - S \, \mathrm{d} T}$$

**For the [[#Maxwell Relations]]:**

![[magicSquare-maxwellRelations.png|align:center]]

1. Choose one side of the magic square and a direction.
	- *Example: Let us choose the left-side of the square and the top-to-bottom direction*
2. Drawing the arrow from one corner to the other, we construct the partial derivative on left-hand-side of the equality. (first term = numerator, second term = denominator) Drawing another arrow from the starting corner to the opposite corner, we can determine which natural variable is constant w.r.t the partial derivative.
	- *Example: Starting in the top-left corner ($T$), we draw an arrow to the bottom-left corner ($x$). The second arrow is drawn from the top-left corner ($T$) to the bottom-right corner ($S$). This creates the left-hand-side of the equality.* $$\left( \frac{\partial T}{\partial x} \right)_{S} = \; ?$$
3. Repeat this on the opposite side of the magic square, where we keep the same initial direction. This will construct the right-hand-side of the equality.
	- *Example: Starting on the top-right corner ($J$), we draw an arrow to the bottom-right corner ($S$). The second arrow is drawn from the top-right corner ($J$) to the bottom-left corner ($x$). This creates the right-hand-side of the equality.* $$\left( \frac{\partial T}{\partial x} \right)_{S} = \left( \frac{\partial J}{\partial S} \right)_{x}$$
4. If $S$ and $x$ are both within the partial derivative (i.e. $\frac{\partial S}{\partial x}$ or $\frac{\partial x}{\partial S}$), then we add a negative sign into the equation. **(This additional rule is represented on the Magic Square by the circled bottom row)**
	- *Example: This is not needed in this example; therefore, both sides of the equality are positive.*

## Negative Heat Capacity

$$\text{Heat Capacity} \equiv C = \frac{\mathrm{d} Q}{\mathrm{d} T} \hspace{1cm} \Rightarrow \hspace{1cm} C_{\rm V} = \left. \frac{\mathrm{d} Q}{\mathrm{d} T} \right|_{V} \quad , \quad \left. C_{\rm P} = \frac{\mathrm{d} Q}{\mathrm{d} T} \right|_{P}$$

Most physical systems exhibit a *positive heat capacity*; however, there are some systems for which the heat capacity is negative. This includes some inhomogeneous systems that are not in thermodynamic equilibrium, such as gravitating objects like stars, black holes, and galaxies.

According to the [[virial theorem]], the energy for a self-gravitating body (like a star or an interstellar gas cloud) can be expressed by...

$$\left\langle E \right\rangle = \left\langle T \right\rangle + \left\langle U \right\rangle \quad , \quad \left\langle E \right\rangle = \frac{1}{2} \left\langle U \right\rangle \hspace{1cm} \Rightarrow \hspace{1cm} \left\langle E \right\rangle = - \left\langle T \right\rangle$$

Therefore, if the system loses energy ($\left\langle E \right\rangle \downarrow$), the average kinetic energy actually increases ($\left\langle K \right\rangle \uparrow$). If a temperature is defined by the average kinetic energy, then the system can be said to have a *negative heat capacity* and get hotter.

More specifically for self-gravitating systems...
- If $\left\langle E \right\rangle$ goes **down** by $1 \varepsilon$
- then $\left\langle E_{\rm therm} \right\rangle \equiv \left\langle T \right\rangle$ goes **up** by $1 \varepsilon$
- and $\left\langle E_{\rm grav} \right\rangle \equiv \left\langle U \right\rangle$ goes **down** by $2 \varepsilon$ 
...such that as a star loses energy, it grows hotter and becomes more gravitationally bound (i.e. $\left\langle E_{\rm grav} \right\rangle$ becomes more negative).

> [!example] **For black holes...**
> A more extreme version of this occurs with black holes. The more mass and energy a black hole absorbs, the colder it becomes. In contrast, if it is a net emitter of energy (i.e. Hawking radiation), it will become hotter and hotter until it boils away.
> 
> A smaller (less massive) a black hole will have a...
> - smaller Schwarzschild radius
> - greater the curvature of its event horizon
> - higher temperature
> 
> Thus, the smaller the black hole, the more thermal radiation it will emit and the more quickly it will evaporate.
