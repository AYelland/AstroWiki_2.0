---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
The **Einstein coefficients** describe the probability of absorption or emission of a photon by an atom or molecule. The Einstein $A$ coefficient is related to the rate of [[#spontaneous emission]], and the Einstein $B$ coefficients are related to the [[#absorption]] and [[#stimulated emission]].

![[einstein_coefficents.jpg|align:center]]

| Einstein Coefficient |             Atomic Process             |               Reaction               |                      Units                      |
| :------------------: | :------------------------------------: | :----------------------------------: | :---------------------------------------------: |
|       $A_{21}$       | <nobr>[[#Spontaneous Emission]]</nobr> |     $E_2 \rightarrow E_1 + h\nu$     |                  $\pu{s^{-1}}$                  |
|       $B_{12}$       |            [[#Absorption]]             |     $h\nu + E_1 \rightarrow E_2$     | $\pu{s^{-1}\,(\text{specific intensity})^{-1}}$ |
|       $B_{21}$       |        [[#Stimulated Emission]]        | $h\nu + E_2 \rightarrow E_1 + 2h\nu$ | $\pu{s^{-1}\,(\text{specific intensity})^{-1}}$ |

> [!note]
> The coefficients are in units of [[Intensity#Specific Intensity|specific intensity]] since these processes depend on the photon "density". 
> - $A$ does not depend on nearby light (spontaneous)
> - $B$ does depend on nearby light *(B = Buddies)*

With these coefficients defined, we can use the volume number density of particles in each energy state ($n_{1}$, $n_{2}$) with the [[Intensity#Specific Mean Intensity|specific mean intensity]] to identify the transition rate (per unit volume) at which the processes occur.

> [!example] For example...
> $$
> \left[ A_{ij} n_{i} J_{\nu} \right] \equiv \left[ \frac{1}{{\rm second} \cdot {\rm intensity}} \cdot \frac{\rm particles}{{\rm volume}} \cdot \frac{\rm intensity}{1} \right] = \left[ \frac{\rm particles}{{\rm second} \cdot {\rm volume}} \right] = \left[ \frac{\rm transitions}{\rm volume} \right]
> $$

## Spontaneous Emission

The **"Einstein $A$ coefficient for spontaneous emission"** ($A_{21}$) represents the probability (per unit time) of an electron "spontaneously" decaying from a higher energy level to a lower one.

In terms of number density of the two states...

$$
\left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm spontaneous} = A_{21} n_{2} \hspace{2cm} \left( \frac{\mathrm{d} n_{2}}{\mathrm{d} t} \right)_{\rm spontaneous} = - A_{21} n_{2}
$$

## Stimulated Emission

The **"Einstein $B$ coefficient for stimulated emission"** ($B_{21}$) represents the probability (per unit time) of an electron transitioning from a higher energy level to a lower one

$$
\left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm stimulated} = B_{21} n_{2} J_{\nu} \hspace{2cm} \left( \frac{\mathrm{d} n_{2}}{\mathrm{d} t} \right)_{\rm stimulated} = - B_{21} n_{2} J_{\nu}
$$

## Absorption

The **"Einstein $B$ coefficient for absorption"** ($B_{12}$) represents the probability (per unit time) of an electron moving to a higher level from a lower level through the absorption of a photon. 

$$
\left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm absorption} = - B_{12} n_{1} J_{\nu} \hspace{2cm} \left( \frac{\mathrm{d} n_{2}}{\mathrm{d} t} \right)_{\rm absorption} = B_{12} n_{1} J_{\nu}
$$

## Detailed Balancing

In thermal equilibrium, the rate of transitions from ($1 \to 2$) should be equal to the rate of transitions ($2 \to 1$). Meaning, if we look specifically at a single energy level, the total inflow and outflow of particles should be equal to zero.

$$
\begin{align}
	(\text{Transitions } \uparrow)_{12} +(\text{Transitions } \downarrow)_{21} &= 0 \\
	\\
	\left[ \left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm absorption} \right] + \left[ \left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm spontaneous} + \left( \frac{\mathrm{d} n_{1}}{\mathrm{d} t} \right)_{\rm stimulated} \right]&= 0 \\
	\\
	\Big[ - B_{12} n_{1} J_{\nu} \Big] + \Big[ A_{21} n_{2} + B_{21} n_{2} J_{\nu} \Big] &= 0 \\
	\\
	n_{2} \Big[ A_{21}  + B_{21} J_{\nu} \Big] &= n_{1} \Big[ B_{12} J_{\nu} \Big] \\
	\frac{n_{2}}{n_{1}} &= \frac{B_{12} J_{\nu}}{A_{21} + B_{21} J_{\nu}}
\end{align}
$$

From the [[Statistical Mechanics#Maxwell-Boltzmann]] distribution, we can re-express the ratio number densities ($n_{i}$) in terms of the energy ($E_{i}$) and the degeneracy ($g_{i}$) of the states.

$$\frac{n_{i}}{n} = \frac{1}{Z} \left( g_{i} \, e^{- E_{i} / k_{\rm B} T} \right) \hspace{1cm} \Rightarrow \hspace{1cm} \frac{n_{2}}{n_{1}} = \frac{g_{2}}{g_{1}} \; e^{- (E_{2} - E_{1}) / k_{\rm B} T}$$

Applying this to the balancing equation where $(E_{2} - E_{1}) = h \nu$...

$$
\frac{n_{2}}{n_{1}} = \frac{B_{12} J_{\nu}}{A_{21} + B_{21} J_{\nu}} = \frac{g_{2}}{g_{1}} \; e^{- h \nu / k_{\rm B} T} \hspace{1cm} \Rightarrow \hspace{1cm}
\begin{aligned}[t]
	J_{\nu} &= \frac{A_{21} \left( \frac{g_{2}}{g_{1}} \; e^{- h \nu / k_{\rm B} T} \right)}{B_{12} - B_{21}\left( \frac{g_{2}}{g_{1}} \; e^{- h \nu / k_{\rm B} T} \right)} \\
	\\
	J_{\nu} &= \frac{\left(\frac{A_{21}}{B_{21}}\right)}{\left(\frac{g_{1} B_{12}}{g_{2} B_{21}}\right) e^{h \nu / k_{\rm B} T} - 1} \\
\end{aligned}
$$

For a thermal process, we can take $J_{\nu}$ as the [[Blackbody Radiation#Blackbody Specific Intensity]] ($B_{\nu}$).

$$B_{\nu} = \frac{2 h \nu^{3}}{c^{2}} \left(\frac{1}{e^{h \nu / k_{\rm B} T} - 1}\right)$$

Comparing the two expressions, we can find the **Einstein Coefficient Relationships**, such that if we know one of the numbers, then we know all three.

$$J_{\nu} = B_{\nu} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{\frac{A_{21}}{B_{21}} = \left(\frac{2 h \nu^{3}}{c^{2}}\right)} \hspace{1cm} , \hspace{1cm} \boxed{\frac{B_{12}}{B_{21}} = \frac{g_{2}}{g_{1}}}$$

> [!note]
> Though these relationships were derived while in thermal equilibrium, they still hold true outside of equilibrium as well. - Cian
