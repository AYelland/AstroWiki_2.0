### Question
---
What is an HII region? Estimate how the Stromgren radius scales with the luminosity of the ionizing source and with the ambient density.

### Answer
---
##### What is an HII region?

![[Interstellar Medium#HII Regions]]

##### Estimate how the Strömgren radius scales with the luminosity of the ionizing source and with the ambient density.

The **Strömgren Radius** is the radius at which the hydrogen ionization rate (around the young stars) is equal to the recombination rate. 

To calculate this radius, we define the following variables:

$$\begin{alignat}{3}
	N &\equiv \text{rate of ionizing photons produced from source} &\hspace{1cm} &{\rm [N]} &&\equiv {\rm [s^{-1}]} \\
	n_{\rm x} &\equiv \text{number density of species $x$} &\hspace{1cm} &{[n_{\rm x}]} &&\equiv {\rm [cm^{-3}]} \\
	\alpha &\equiv \text{recombination coefficient} &\hspace{1cm} &{[\alpha]} &&\equiv {\rm [cm^{3} \, s^{-1}]} \\
	R_{s} &\equiv \text{Strömgren Radius} &\hspace{1cm} &{[R_{s}]} &&\equiv {\rm [cm]} \\
\end{alignat}$$

> [!note] Comment on $\alpha$
> Given that $\alpha$ is quantum in nature, we define it ${\rm cm^{-3} \, s^{-1}}$ such that $(\alpha \, n_{1} n_{2})$ gives the generation rate of a neutral species from species 1 and 2 (per unit volume). Note that this should not include contributions from recombinations to the ground state, as this will release a photon that can again ionize another H atom.

Assuming the gas is entirely composed of hydrogen, is net neutral ($n_{\rm e} = n_{\rm H} = n$), and contained in a sphere, the recombination rate is...

$$\text{Recombination Rate} \; \equiv \; \alpha \, n_{\rm e} n_{\rm H} \cdot \left( \frac{4}{3} \pi R_{s}^{3} \right) = \alpha \, n^{2} \cdot \left( \frac{4}{3} \pi R_{s}^{3} \right) \quad \quad {\rm \left[ cm^{-3} \, s^{-1} \right]}$$

The boundary where the ionization rate and recombination rate are equal is then...

$$N = \alpha \, n^{2} \cdot \left( \frac{4}{3} \pi R_{s}^{3} \right) \hspace{1cm} \Rightarrow \hspace{1cm} R_{s} = \left( \frac{3 N}{4 \pi \alpha \, n^{2}} \right)^{1/3}$$
We can now relate the ionization rate ($N$) to the [[Luminosity|specific luminosity]] ($L_{\nu}$) and the energy of a photon with frequency ($h \nu$)...

$$N = \int_{E_{\rm th}}^{\infty} \frac{L_{\nu}}{h \nu} \; \mathrm{d} \nu \hspace{1cm} \text{where} \hspace{1cm} E_{\rm th} \equiv 13.6 \; {\rm eV}$$

...where $E_{\rm th}$ is the minimum ionization energy for hydrogen. Any photons with energy less than this will not contribute to our analysis. Assuming we can measure the luminosity ($L$), we can then find $N \propto L$ , and thus, $R_{s} \propto L^{1/3}$.
