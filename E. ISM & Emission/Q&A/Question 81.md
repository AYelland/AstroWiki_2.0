### Question
---
Qualitatively describe the "equipartition energy" of a synchrotron source? What can we learn about cosmic rays from this?

### Answer
---
##### Qualitatively describe the "equipartition energy" of a synchrotron source?
*(More detailed derivation: [Section 5.4.1](https://www.cv.nrao.edu/~sransom/web/Ch5.html) or Longair, Section 16.5)*

In a [[Synchrotron Radiation|synchrotron]] source (i.e. relativistic charged particles in an approximately uniform magnetic field), there are two relevant energy densities:

1) **The Magnetic Field** ($U_{\rm B}$)

$$U_{\rm B} = \frac{B^{2}}{2 \mu_{0}} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{ \; U_{\rm B} \propto B^{2} \; }$$

2) **The Particle Energy Density** ($U_{\rm E}$) - a bit more involved...
	
	- From the [[Synchrotron Radiation#^peak-frequency]] frequency and the energy of the radiation-emitting electron, we can express the minimum and maximum energy values ($E_{\rm min}$, $E_{\rm max}$) in relation to the associated frequencies and the magnetic field. $$E = \gamma \, m_{e} c^{2} \hspace{1cm} \nu = \gamma^{2} \,\nu_{c} = \gamma^{2} \left(\frac{q B}{2 \pi m c}\right) \hspace{1cm} \Rightarrow \hspace{1cm} \begin{aligned}[t] \gamma^{2} \propto E^{2} &\; \propto \frac{\nu}{B} \\ \\ \Downarrow \\ \\ E_{\rm min} \propto &\; B^{\ -1/2} \\ E_{\rm max} \propto &\; B^{\ -1/2} \end{aligned}$$
	- We assume the number density ($n(E)$) scales with a power-law energy distribution. $$n(E) \; \mathrm{d} E \; \propto \; E^{-P} \; \mathrm{d} E$$
	- The power emitted (luminosity, $L$) by the source electron comes from [[Larmor Formula#Relativistic Power|Larmor Formula]]. $$L \propto\frac{\mathrm{d} E}{\mathrm{d} t} \propto \left\langle P \right\rangle = \frac{4}{3} \, \sigma_{\rm T} \, \beta^{2} \, \gamma^{2} \, c \, U_{\rm B} \hspace{1cm} \Rightarrow \hspace{1cm} L \propto E^{2} B^{2}$$
	- Taking a ratio of the electron-associated energy density and the luminosity... $$\begin{align} \frac{U_{\rm e}}{L} &\propto \frac{\int_{E_{\rm min}}^{E_{\rm max}} E \; n(E) \; \mathrm{d} E}{\int_{E_{\rm min}}^{E_{\rm max}} \left( \frac{\mathrm{d} E}{\mathrm{d} t} \right)\; n(E) \; \mathrm{d} E} \propto \frac{\left. E^{2} \; n(E) \; \right|_{E_{\rm min}}^{E_{\rm max}}}{\left. \left( \frac{\mathrm{d} E}{\mathrm{d} t} \right) E\; n(E) \; \right|_{E_{\rm min}}^{E_{\rm max}}} \\ \\ &\Rightarrow \hspace{1cm} \propto \frac{\left. E^{2} \; E^{-P} \; \right|_{E_{\rm min}}^{E_{\rm max}}}{\left. \left( E^{3} B^{2} \right)\; E^{-P} \; \right|_{E_{\rm min}}^{E_{\rm max}}} \propto \frac{B^{-(2-P)/2}}{B^{2} B^{-(3-P)/2}} \propto \frac{B^{-1} B^{P/2}}{B^{1/2} B^{P/2}} \propto B^{-3/2}\end{align}$$ $$\boxed{ \; U_{\rm E} \; \propto \; U_{\rm e} \; \propto \; B^{-3/2} \; }$$

> [!note]
> [[Synchrotron Radiation|Synchrotron emission]] originates mostly in relativistic electrons, but other species also contribute to the particle energy density.
> 
> The “invisible” cosmic-ray protons and heavier ions emit negligible synchrotron power but they still contribute to the total cosmic-ray particle energy. If the ion/electron energy ratio is $\eta$, then the total particle energy density in cosmic rays is... 
> 
> $$U_{\rm E} = \left( 1 + \eta \right) \; U_{\rm e}$$

The [[Statistical Mechanics#Equipartition Energy|equipartition principle]] suggests that the lowest energy configuration for any system is when the energy is distributed equally across all of it degrees of freedom. Here, that means (roughly speaking) having equal energy density contributions from both the particles and the magnetic field.

Therefore, the total energy density ($U$) from both contributions is:

$$U = U_{\rm E} + U_{\rm B} = \left( 1 + \eta \right) \; U_{\rm e} + U_{\rm B}$$

Plotting this energy density as a function of the magnetic field strength ($B$), we see a very sharp drop in energy toward the $B$-value where both energy densities are approximately equal. The minimum of this spectrum is at $U_E/U_B = 4/3$. *(see [equation 5.101](https://www.cv.nrao.edu/~sransom/web/Ch5.html))*

![[equipartition.png|align:center|450]]

##### What can we learn about cosmic rays from this?

![[Interstellar Medium#Cosmic Rays]]

Radio astronomers often assume [[Synchrotron Radiation|synchrotron]] sources are in equipartition because:
- It is physically plausible; systems with interacting components often tend toward equipartition.
- If know the [[Luminosity|luminosity]] of a source, we can obtain an estimate of the magnetic field, and thus, an estimate of the magnetic and particle energy densities of the source
	- This allows us to an overall estimate of the [[Interstellar Medium#Cosmic Rays|cosmic ray]] energy. If we don't know $\eta$ very well, we can still get within an order of magnitude or two.
- There is an "energy problem" for large extragalactic radio sources, which would require enormous total energies to explain their luminosities (e.g. [[Question 168|Cyg A]]). The "least bad" this problem can be is when equipartition is assumed, at which the total energy for a given $L$ is minimized.