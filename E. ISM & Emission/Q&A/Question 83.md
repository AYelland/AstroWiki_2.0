### Question
---
Why is the gas in the interstellar medium largely transparent at visible wavelengths? How does the transparency of the ISM depend on wavelength in the optical and near-IR, and why?

### Answer
---
The [[Optical Depth#Opacity|opacity]] of the [[Interstellar Medium|ISM]] has many sources. 

$$\rho\kappa = \frac{1}{l} = n\sigma = \alpha = \frac{\mathrm{d} \tau}{\mathrm{d} z} \textcolor{gray}{\hspace{1cm} \text{where} \hspace{1cm} \mathrm{d} z \equiv \text{path of light}}$$

Ignoring emissions from the ISM, the relevant light-matter interactions are:

- [[Bound-Bound Absorption]] 
	- Leads to absorption lines at specific energies, but does not attenuate the whole continuum.
- [[Bound-Free Absorption]] 
	- Originate from the ionization of hydrogen (primarily), leading to absorption lines at $\sim 13.6\,\pu{eV}$ in the [[Electromagnetic Spectrum|UV spectrum]].
- [[Free-Free Absorption]] and [[Thomson Scattering|Electron Scattering]] 
	- Both require ionized gas to occur, such as in the [[Interstellar Medium#Hot Ionized Medium (HIM)]] or [[Interstellar Medium#HII Regions]], but the density is too low to contribute significantly to  [[Optical Depth#Opacity|opacity]].
- $\rm{H}^-$ Opacity
	- Occurs when [[Interstellar Medium#Atomic Hydrogen|neutron hydrogen]] captures another electron to fill its $1s$ orbital
	- Requires neutral $\rm{H}$ and free electrons, which can happen with partially ionized metals in a stellar atmosphere.

Overall, there is not much opacity in the [[Interstellar Medium|ISM]], on the exception of [[Interstellar Medium#Dust|dust]] which absorbs light in the optical/UV and re-emits thermally in the IR. 

This is due to having such a low particle density in the [[Interstellar Medium|ISM]]. Even in the densest phases (i.e. [[Interstellar Medium#Molecular Clouds|molecular clouds]]), the density is still very low compared to stellar atmospheres. $\implies$ low optical depths ($\tau$) in the visible band.

$$\tau = \int_{0}^{z} \alpha \; \mathrm{d} z = \int_{0}^{z} n\sigma \; \mathrm{d} z$$

The wavelength dependence of the optical depth can be plotted as..

![[ISM_extinction.png|align:center|450]]

*(Image and Details: https://ned.ipac.caltech.edu/level5/Sept07/Li2/Li2.html)*

Most of the extinction in the UV-band is associated with the scattering/absorbing of light from dust with sizes comparable to the with light's wavelength ([[Mie Scattering]]).

$$\tau_{\lambda} \; \propto \; \sigma_{\lambda} N \; \propto \; \lambda^{-1} \hspace{2.5cm} \lambda \sim a \equiv\text{size of dust grain}$$

The observed "extinction bump" can additionally provide information about the composition of the dust.
