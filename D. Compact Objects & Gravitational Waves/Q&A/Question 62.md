### Question
---
How much rotational kinetic energy can be stored in a neutron star? How does this help resolve the "energy budget" for the Crab nebula?

### Answer
---
##### How much rotational kinetic energy can be stored in a neutron star?

Rotational kinetic energy is the moment of inertia ($I$) times the squared-frequency ($\Omega$).

$$T_{\rm rot} = \frac{1}{2} I \Omega^{2}$$

For a solid sphere of mass $M$ and radius $R$, the moment of inertia is...

$$I = \frac{2}{5} M R^{2}$$

Applying the typical [[Neutron Star|neutron star]] parameters...

$$T_{\rm rot} = \frac{1}{2} \fpar{2 M R^{2}}{5} \fpar{2 \pi}{P}^{2} = \frac{4 \pi^{2} M R^{2}}{5 P^{2}} \sim 10^{43} \; {\rm J}$$
$$
\textcolor{gray}{\left[ \; T_{\rm rot} \sim \fpar{4 \pi^{2} \cdot (1.4) \cdot (2 \times 10^{30}) \cdot \left( 10^{4} \right)^{2}}{5 \cdot \left( 10^{-2} \right)^{2}} \sim \left( \frac{100}{5} \times 10^{42} \right) \sim 10^{43} \; {\rm J} \; \right]}
$$

![[Neutron Star#^typical-parameters]]

##### How does this help resolve the "energy budget" for the Crab nebula?

The [[Nebulae#Pulsar Wind Nebula|Crab Nebula]] was originally observed in 1054 and was recorded through drawings. It has a [[Luminosity|luminosity]] of $L \sim 10^{31} \; {\rm W}$.

Given the expression for rotational kinetic energy above, we can determine how much of that power could come from the spinning [[Neutron Star|neutron star]]. For the Crab nebula, $P \sim 30 \; {\rm ms}$ and $\dot{P} \sim 10^{-13} \; {\rm s\ Hz}$.

$$\td{T_{\rm rot}}{t} = I \Omega \dot{\Omega} = I \Omega \frac{- 2 \pi \dot{P}}{P} = - \fpar{8 \pi^{2} M R^{2}}{5} \frac{\dot{P}}{P^{3}} \sim - 10^{31} \; {\rm W}$$

$$\textcolor{gray}{\left[ \; \td{T_{\rm rot}}{t} \sim - \fpar{8 \pi^{2} \cdot (1.4) \cdot (2 \times 10^{30}) \cdot \left( 10^{4} \right)^{2}}{5} \times \fpar{10^{-13}}{\left( 3 \times 10^{-2} \right)^{3}} \sim \left( - 10^{39} \times 10^{-8} \right) \sim - 10^{31} \; {\rm W} \; \right]}$$

The two [[Luminosity|luminosities]] being the same order of magnitude means the entire power output can come from energy losses in the spinning [[Neutron Star|neutron star]].

![[Mnemonics#^crab]]
