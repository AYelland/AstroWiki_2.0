---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - synchrotron
  - synchrotron radiation
---

*Summary and detailed notes [here](https://www.cv.nrao.edu/~sransom/web/Ch5.html). A highly detailed overview of all this in [this article](https://arxiv.org/pdf/1202.5949.pdf) (radiative processes in high energy astrophysics by Ghisellini)*

Electromagnetic radiation emitted by **relativistic accelerating charged particles deflected by a magnetic field**. *($v\sim c \implies \gamma \gg 1$ )*

The non-relativistic counterpart to this is [[Cyclotron Radiation]].

![[synchrotron.png|align:center|400]]

![[synchrotron_diagram.png|align:center|400]]

> [!note] Synchrotron Frequency
> 
> The **synchrotron frequency** ($\omega_{\rm s}$) is an angular frequency of a relativistic charged particle ($q$) moving perpendicular to the direction of a uniform magnetic field ($B$). 
> 
> It is very similar to the **cyclotron frequency** ($\omega_{\rm c}$), with a relativistic correction.
> 
> $$F_{\rm B} = \frac{q}{c} \, \left( \vec{v} \times \vec{B} \right) = \frac{q B v}{c} \hspace{2.5cm} F_{\rm circ} = \left( \gamma \, m_{0} \right) \frac{v^{2}}{r} = \gamma \, m_{0} \, \omega_{\rm c} \, v$$
> $$\gamma \, m_{0} \, \omega_{\rm c} \, v = \frac{q B v}{c} \hspace{1cm} \Rightarrow \hspace{1cm} \omega_{\rm s} = \frac{\omega_{\rm c}}{\gamma} = \frac{q B}{\gamma \,m_{0} c}$$
> 
> *Note: The mass ($m_{0}$) is the rest mass.*

^19855b

Similar to the cyclotron radiation, the power emitted from synchrotron radiation is:

$$P = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, \alpha^{2} = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, (\gamma^{2} a)^{2} = \left(\frac{q^{4} B}{6 \pi \epsilon_{0} c^{3}}\right) \frac{\gamma^{4} \beta^{2}}{m_{0}^{2}}$$
$$P = \frac{4}{3} \sigma_{\rm T} \beta^{2} \gamma^{2} c \, U_{\rm B} \hspace{1cm} \text{where} \hspace{1cm} \begin{aligned}
	\sigma_{\rm T} &\equiv \text{Thompson cross section} \\
	U_{\rm B} &\equiv \text{B-field energy density} = B^{2}/2 \mu_{0}
\end{aligned}$$
...which tells us that there is much stronger emission from lighter particles that heavier particles ($P \propto m_{0}^{-2}$). Additionally, if $E = \gamma m_{0} c^{2}$, then $P \propto E^{4}$ .

When the charged particles moves relativistically, its radiation is is affected by being **beamed** and **pulse shortening**.

1) Beamed Radiation - radiation with a Lorentz factor ($\gamma$) is emitted in a cone with opening angle ($\theta = \gamma^{-1}$) ![[synchrotron_beamed.png|align:center|450]]
2) Pulse Shortening - the electron is almost same speed as radiation emitted, such that the duration of the pulse is shorted $[ \, \Delta t' = \tfrac{\Delta x}{v} \left( 1 - \tfrac{v}{c} \right) \, ]$ *(see [[#^peak-frequency|timing of emission]])* ![[sychrotron_pulse.png|align:center|450]]

### Spectrum

The net outcome is that the spectra is spread out into two regimes:
- **Optically thick** (low-frequency) - self-absorption becomes important as the radiation acts more like a [[Blackbody Radiation|blackbody]] (blackbody = perfect emitter/absorber = most efficient radiator)
- **Optically thin** (high-frequency) - photons escape before the electrons can re-absorb them.

![[synchrotron_spectrum.png|align:center|450]]

> [!note]- Single Emission vs Many Emissions Spectrum
> 
> The emission of a single electron propagating around a magnetic field is only a small contribution to the overall system. The individual contribution add together yielding the overall observed spectrum.
> 
> ![[synchrotron_spectrum_many.png|align:center|450]]

> [!note]- Timing of Emission & Peak Pulse Frequency
> ![[synchrotron_timing.png|align:center|400]]
> 
> - $t_{\rm A} \equiv$ time of radiation emitted from $A$ 
> - $t_{\rm B} \equiv$ time of radiation emitted from $B$ 
> - $t'_{\rm A} \equiv$ time of radiation received from $A$ 
> - $t'_{\rm B} \equiv$ time of radiation received from $B$ 
> 
> $$t_{\rm B} = t_{\rm A} + \frac{x}{v} \hspace{1.5cm} t'_{\rm A} = t_{\rm A} + \frac{x}{c} + \frac{d}{c} \hspace{1.5cm} t'_{\rm B} = t_{\rm B} + \frac{d}{c}$$
> 
> For time observed between the pulses...
> $$\Delta t' = t'_{\rm B} - t'_{\rm A} = \frac{x}{v} - \frac{x}{c} = \frac{x}{v} \left( 1 - \frac{v}{c} \right) = \frac{1}{\nu_{c}} \left( 1 - \frac{v}{c} \right)$$
> ...we can substitute the cyclotron (gyration) frequency ($\nu_{c} = v/x$) into the expression for the time it takes for 1 cycle around the field line. 
> 
> Going a step further, we can express this time duration ($\Delta t'$) in Lorentz factors ($\gamma$) for when $v \sim c$.
> $$\left( 1 - \frac{v}{c} \right) = \frac{\left( 1 - \frac{v}{c} \right) \left( 1 + \frac{v}{c} \right)}{\left( 1 + \frac{v}{c} \right)} = \frac{\left( 1 - \frac{v^{2}}{c^{2}} \right)}{\left( 1 + \frac{v}{c} \right)} \approx \frac{1}{2 \gamma^{2}}$$
> This means the time between the observed pulses and the associated (peak) pulse frequency is...
> $$\Delta t' = \frac{1}{2 \gamma^{2} \nu_{c}} \hspace{1cm} \Rightarrow \hspace{1cm} \nu_{peak} = \frac{1}{\Delta t'} = 2 \gamma^{2} \nu_{c}$$
^peak-frequency

For *optically thin* (high-frequency) regime, we consider a power-law energy distribution of an electron population.

$$n(E) \; \mathrm{d} E \; \propto \; E^{-P} \; \mathrm{d} E$$

Looking at the proportionality between [[#^peak-frequency|peak frequency]] ($\nu \equiv \nu_{peak}$) and (mean?) electron energy...

$$E = \gamma \, m_{e} c^{2} \hspace{1cm}  
\nu = \gamma^{2} \,\nu_{c} = \gamma^{2} \left(\frac{q B}{2 \pi m c}\right)\hspace{1cm} \Rightarrow \hspace{1cm}
\begin{aligned}[t]
	E^{2} &\propto \gamma^{2} \propto \nu \\
	\\
	&\Downarrow \\
	\\
	2 E \; \mathrm{d} E &\propto \mathrm{d} \nu \\
	\mathrm{d} E &\propto \frac{\mathrm{d} \nu}{E} \\
	\mathrm{d} E &\propto \nu^{-1/2} \; \mathrm{d} \nu \\
\end{aligned}$$

...we can relate the energy distribution to the spectrum, $f(\nu)$.

$$
\begin{aligned}[t]
	F_{\nu} \propto \; f(\nu) \; \mathrm{d} \nu \; &\propto \; \nu \; n(E) \; \mathrm{d} E \\
	&\propto \; \Big( E^{2} \Big) \, \Big( E^{-P} \Big) \Big( \mathrm{d} E \Big)  \\
	&\propto \; \Big( \nu \Big) \, \Big( \nu^{-P/2} \Big) \Big( \nu^{-1/2} \Big) \\
	&\propto \nu^{-(P-1)/2}
\end{aligned}$$
$$\boxed{F_{\nu} \propto \nu^{-(P-1)/2}}$$

For *optically thick* (low-frequency) regime, self-absorption becomes important such that the spectrum becomes [[Blackbody Radiation|blackbody]] limited. Following [[Blackbody Radiation#Rayleigh-Jeans Law]], the energy of the emission (i.e. photons) will be proportional to the frequency-squared and the temperature.

$$F_{\nu} \propto B_{\nu} = \frac{2 h}{c^{2}} \left(\frac{\nu^{3}}{e^{h \nu / k_{\rm B} T} - 1}\right) \propto \left(\frac{\nu^{3}}{h \nu / k_{\rm B} T}\right) \propto \nu^{2} \, k_{\rm B} T$$

Similarly, the electron energy will also be temperature dependent, because it's a blackbody. This allows us to relate the [[#^peak-frequency|peak frequency]] back to the spectrum, like before.

$$E \propto k_{\rm B} T \quad , \quad E^{2} \propto \nu \hspace{1cm} \Rightarrow \hspace{1cm} k_{\rm B} T \propto \nu^{1/2}$$
$$F_{\nu} \propto \nu^{2} \, k_{\rm B} T \propto \nu^{2} \Big( \nu^{1/2} \Big) \propto \nu^{5/2} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{F_{\nu} \propto \nu^{5/2}}$$

>[!cian]- Why is it a spectrum and not a spike?
> 
> (Formally it isn't a spectrum, but effectively it is; see link at beginning of section)
> - The electric field at a detector from a cyclotron source (ignoring the high-frequency wiggles due to the electric field of individual photons) will be approximately sinusoidal. 
> - Since the frequency spectrum goes as the Fourier Transform of the time signal, the FT will be a delta function (+ harmonics) as in [[Cyclotron radiation]]. 
> - The doppler relativistic beaming effectively turns the source into a flashlight that points in the direction of motion of the particle. So, our spectrum at the detector will look like a series of thinner peaks with a low continuum between. The timescale over which we can "see" the pulse is much smaller than the timescale of the rotation. ![[synchrotron_comb.png|align:center|400]]
> - The FT of such a signal will be a series of broad spikes which are very close together, resulting in an effective spectrum.
