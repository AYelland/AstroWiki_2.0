### Question
---
What mass should a neutrino have to close the universe? Compare it with current upper bounds (or detections).

### Answer
---
##### What mass should a neutrino have to close the universe?

To find the mass to "close the universe", we analyze the threshold (or tipping point) between an open universe and a closed universe (i.e. a flat the universe, $\Omega = 1$) in the context of the [[Friedmann Equation]]. 

If all of the universe's mass is made of neutrinos, then by the definition of the [[Friedmann Equation#Critical Density|critical density]], the condition for a flat universe would be:

$$\rho_{\nu} = \rho_{\rm crit} = \frac{3 H_{0}^{2}}{8 \pi G}$$

If we only needed neutrinos to account for all the [[Dark Matter|dark matter]], then we would instead have the condition of...

$$\rho_{\nu} = \Omega_{\rm DM} \, \rho_{\rm crit} = \frac{3 \,\Omega_{\rm DM} H_{0}^{2}}{8 \pi G}$$

...where $\Omega_{DM}\simeq 0.3$ (see [[Instruments#Planck]]). However, if this were true, then there would be no large scale structure, as things would be moving too quickly to collapse.

To work out the mass, we need the number density of neutrinos in the universe. One can calculate the neutrino-to-photon temperature ratio via conservation of neutrino entropy (I guess it's conserved because they don't interact with other things, so their thermal properties don't change).

$$\frac{T_{\nu}}{T_{\gamma}} = \left(\frac{4}{11}\right)^{1/3} \simeq 0.7\hspace{1cm} \Rightarrow \hspace{1cm} T_{\nu,0} \simeq 2\,\pu{K}$$

Converting to the neutrino-to-photon density where  $\rho \propto T^{4}$...

$$\frac{\rho_{\nu}}{\rho_{\gamma}} \simeq \frac{7}{8} \, N_{\rm eff}\left(\frac{4}{11}\right)^{4/3} \hspace{1cm} \Rightarrow \hspace{1cm} \rho_{\nu} \simeq 0.7 \, \rho_{\gamma} \hspace{1.5cm} n_{\nu} \simeq 0.7 \, n_{\gamma}$$

...where $N_{eff} =  3$ comes from the greater number of degrees of freedom of neutrinos relative to photons since 3 neutrino flavors, and the factor of $7/8$ comes from the fermion vs. boson integral.

There are about 300 neutrinos per $\pu{cm^{3}}$ and about 400 photons per $\pu{cm^{3}}$ ([[Question 145]]). This leads to neutrino masses of $m_\nu \simeq 18\,\pu{eV}$ and $5\,\pu{eV}$, respectively for the above two cases.

$$\begin{alignat}{2}
	m_{\nu} &= \frac{\rho_{\rm crit}}{n_{\nu}} \simeq \frac{10^{-29} \; {\rm g \, cm^{-3}}}{3 \times 10^{2} \; {\rm cm^{-3}}} \sim 3 \times 10^{-32} \; {\rm g} &&\sim 18 \; {\rm eV} &\hspace{2cm} &\text{(all mass is neutrinos)} \\
	m_{\nu} &= \frac{\rho_{\rm crit} \cdot \Omega_{\rm DM}}{n_{\nu}} \simeq \frac{(10^{-29} \; {\rm g \, cm^{-3}}) \cdot 0.3}{3 \times 10^{2} \; {\rm cm^{-3}}} \sim 10^{-32} \; {\rm g} &\quad&\sim 4 \; {\rm eV} &\hspace{2cm} &\text{(just DM is neutrinos)}
\end{alignat}$$

##### Compare it with current upper bounds (or detections).

Current upper bound is $m_\nu < 0.8\,\pu{eV}$ from [[Instruments#KATRIN]], which uses [[Beta Decay]] of tritium for its constraints.

Below, there is an experimental neutrino mass timeline, but the x axis is $m^2$ so actually this may be confusing. Just use it for experimental history and relative sizes of error bars. Also cosmological constraints using [[Baryon Acoustic Oscillations|BAO]] and other probes finding constraints $m_\nu \lesssim 0.1\,\pu{eV}$ , but bounds depend on cosmological assumptions.

![[NeutrinoMassTimeline2022.png|align:center|500]]

