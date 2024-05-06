### Question
---
If a typical interstellar dust grain is 0.2 microns in size, and starlight suffers an extinction of 1 magnitude per kpc, estimate the space density of dust grains.

### Answer
---
We will assume the interstellar dust has [[Radiative Transfer Equation|only absorption and no emission]], such that by [[Optical Depth#Mean Free Path|Lambert-Beer Law]], the light is attenuation is scaled by the [[Optical Depth#Optical Depth|optical depth]].

$$F_{\nu} = F_{\nu,0} \;e^{-\tau_{\nu}} \hWhere \begin{aligned}
	F_{0} &\equiv \text{incident flux} \\
	\tau_{\nu} &\equiv \text{optical depth}
\end{aligned}
$$

The **extinction of light** ($A_{\lambda}$) can be defined as the different in [[Magnitude#Apparent Magnitude|apparent magnitude]] from the emitted/incident flux ($F_{\rm 0}$) and the observed flux at a distance $d$ ($F_{d}$).

$$\begin{align}
	A_{\nu} \equiv \underbrace{m_{\nu,d} - m_{\nu,0}}_{\Delta m_{\nu}} = -2.5 \log_{10} \fpar{F_{\nu,d}}{F_{\nu,0}} = -2.5 \log_{10} \left( e^{-\tau_{\nu}} \right) &= 2.5 \,\tau_{\nu} \log_{10} (e) \simeq \tau_{\nu}\\
	&= 2.5 \left( n \sigma d \right)\log _{10}(e)
\end{align}$$

Here, we choose to write ($n\sigma d$) instead of ($N\sigma$) for the [[Optical Depth#Optical Depth|optical depth]] because we are interested in getting a volume density (not a column density) while also assuming the material is uniform over the distance $d$. 

If we rearrange, the volume density ($n$) can be expressed as...

$$n = \frac{\Delta m}{2.5\,\sigma d \log_{10}(e)}$$

So, for a distance of ($d = 1 \; {\rm kpc}$) and extinction of ($A_{\nu} = \Delta m_{\nu} = 1$), we can approximate the scattering cross section ($\sigma = \pi r^{2} = \pi \, (0.2 \; {\rm \mu m})^{2}$) as completely classical scattering, if the wavelength of light is much smaller than the size of the grain. Plugging in values, we find...

$$n = \frac{1}{2.5 \, \pi \, (0.2 \; {\rm \mu m})^{2} (1 \; {\rm kpc}) \underbrace{\log_{10}(e)}_{\approx \, 1}} \sim 10^{-6} \; {\rm m^{-3}} \sim 10^{-12} \; {\rm cm^{-3}}$$
