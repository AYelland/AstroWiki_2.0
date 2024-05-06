---
banner: "![[otherphysics.png]]"
banner_y: 0.5
aliases:
---

## Electrostatic Binding Energy
*(Also known as the **ionization energy** or the **electron binding energy**)*

The **electrostatic binding energy** is the minimum energy required to remove the most loosely bound electron of an isolated atom, ion, or molecule. As expected from the Coulomb's force, the binding energy is higher for electrons more closely bound to the nuclei, requiring more and more energy from successive electron removals.

Using **Bohr's Model:**
$$
U_{\rm E} = - \frac{1}{2 a_{0}} \fpar{Z e}{n}^{2}
$$
The electrostatic binding energy ($\varepsilon_{a}$) can be approximated with the elementary charge ($e$) and the Bohr radius ($a_{0}$).
$$\varepsilon_{a} = \frac{e^{2}}{a_{0}} \hWhere k = \frac{1}{4 \pi \epsilon_{0}} = 1$$
$$n \equiv \frac{N}{V} = \frac{\text{\# of particles}}{\text{volume}} = \text{number density}$$
Tightly Packed: $\quad n_{0} = a_{0}^{-3} \hRightarrow n_{0} a_{0}^{3} \sim 1 \hRightarrow \varepsilon_{a} \sim n_{0}^{1/3} e^{2}$

## Gravitational Binding Energy

The **gravitational binding energy** is the minimum potential energy necessary to keep a system/body bound together through gravity. 

For a spherical body with a constant, uniform density, we can apply the *spherical shell method* to calculate this potential energy value.

$$
\begin{align}
	U_{\rm G} &= - \int_{0}^{M} \frac{G M(r) \; \rd m}{r} \\
	&= - \int_{0}^{R} \frac{G \left( \frac{4}{3} \pi r^{3} \rho \right) \left( 4 \pi r^{2} \rho \; \rd r \right)}{r}  \\
	&= - \frac{16 G \pi^{2} \rho^{2}}{3} \int_{0}^{R} r^{4} \; \rd r \\
	&= - \frac{16 G \pi^{2} R^{5} \rho^{2}}{15} \textcolor{gray}{\hWhere M = \rho V = \rho \left( \frac{4}{3} \pi R^{3} \right)} \\
	&= - \frac{3 G M^{2}}{5 R}
\end{align}
$$

## Nuclear Binding Energy

The structure of an atomic nucleus is held together by the strong nuclear force (mediated by gluons). This forces gives rise to the **nuclear binding energy** that determines how much potential energy a nuclei has and/or how much energy it takes to break apart a given nuclei.

The mass of a nuclei ($m_{\rm nuc}$) with mass number $A$ and atomic number $Z$  is always less than the combined mass of number of protons ($Z$) and the number of neutrons ($A-Z$). With this in mind, we can express the nuclear binding energy as...
$$U_{\rm B} = \left[ Z m_{\rm p} + (A - Z) m_{\rm n} - m_{\rm nuc} \right] \, c^{2}$$

The nuclear binding energy *per nucleon* can then be expressed and plotted as:
$$f = \frac{U_{\rm B}}{A}$$

![[binding_energy.png|align:center|500]]

We note that in this plot, iron ($Fe$) is at the peak of this distribution, such that is the most tightly bound nuclei. Therefore...
- If we combine smaller nuclei into larger ones, we will gain energy up to $Fe$.
	- Nuclear fusion is more favorable for $Z < 26$
- If we split larger nuclei into smaller ones, we will gain energy down to $Fe$.
	- Nuclear fission is more favorable for $Z > 26$

We also note that the amount of energy to be gained by fusion is far greater than by fission.
- Example: The atomic bomb works by splitting uranium. The much more powerful hydrogen bomb works by fusing H into heavier elements.

