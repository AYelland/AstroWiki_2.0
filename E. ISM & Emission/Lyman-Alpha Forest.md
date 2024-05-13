---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
## General Overview

The **Lyman-$\mathbf{\alpha}$ forest** is a series of absorption lines corresponding to a distant [[Active Galactic Nuclei#Quasar / Quasi-Stellar Object (QSO)|quasar]] (or a very bright, distant background source). The absorption lines originate from gas clouds at different redshifts, each absorbing at the [[Spectral Features#Lyman Series|Lyman-alpha transition]] ($n=2 \to n=1$ at $\lambda = 1216 \; {\rm \mathring{A}}$) in their own rest frames.
 
![[lyman-alpha_schematic.png|align:center|600]]

In principle, the absorption spectrum can serve as a map of the gas between the observer and the source through the [[Intergalactic Medium|IGM]]. We can gain information about  [[Redshift|redshift]] and structure of the [[Intergalactic Medium|IGM]], in addition to probing the density, ionization, temperature, and chemistry. making it very interesting for cosmologists. For instance, using the depth of the absorption lines, we can determine the [[Optical Depth#Optical Depth|optical depth]] ($\tau_{\nu}$) of the [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen]] as a function of redshift ($z$).

Each cloud absorbs the line at a wavelength $\lambda = (1+z) \lambda_{0}$. We can then convert them back to the emitted wavelength as in the plot below, rather than observed wavelength. For a real spectra showcasing the Lyman-$\alpha$ forest...

![[lyman-alpha_spectra.png|aling:center|600]]

![[Lyman-alpha_forest.gif|align:center|600]]

> [!note] It's called a "forest" because the lines looks like a bunch of trees.


**Other Notes:**
- Identify lines in general through doublets: $\mu_{0II}$ ($\lambda=2795 \; {\rm \mathring{A}}$,  $2802 \; {\rm \mathring{A}}$, ...)
- Lyman-$\alpha$ forest is only visible if it extends to shorter wavelengths. 
	- Then, the observed Ly$\alpha$ emission line at $(1+z_{\rm em})1216\;{\rm \mathring{A}}$. 
	- Photons emitted with $1216 \; {\rm \mathring{A}} (1+z_{\rm em}) < \lambda < 1216 \; {\rm \mathring{A}}$ will at some point have the right rest frame wavelength ($1216 \; {\rm \mathring{A}}$) to be absorbed.
- There are three cases for HI along the line of sight:
	1. column density $N_{\rm H} \lesssim 10^{17}\;{\rm cm}^{-2}$ gives narrow lines (i.e. the forest)
	2. column density $N_{\rm H} \gtrsim 10^{17}\;{\rm cm}^{-2}$ are [[Spectral Features#Lyman Limit]] systems (i.e. photons with $\lambda\lesssim 912 \; {\rm \mathring{A}} = 13.6 \; {\rm eV}$) 
		- In the rest frame, are completely absorbed as the light moves through the cloud.
	3. column density $N_{\rm H} \gtrsim 10^{32}\:{\rm cm}^{-2}$ are damped Ly-$\alpha$ systems (i.e. absorption lines become very broad)


## The Gunn-Peterson Test

The absorption spectra provides clues about [[Cosmological Timeline#Reionization]], how baryons are distributed in the universe, and what state they are in. The key idea is that neutral hydrogen along the line-of-sight leads to absorption, so if there is a significant amount of neutral hydrogen, then the spectrum should be totally absorbed. 

During the time between [[Cosmological Timeline#Recombination]] and [[Cosmological Timeline#Reionization]] (high $z$), the hydrogen is almost entirely neutral; such that the high-wavelength region of the spectrum should be almost totally absorbed. This is called the **Gunn-Peterson trough**.

![[lyman-alpha_gunn-peterson.png|align:center|650]]


For a close-by source ($z \lesssim 6$), we see very little suppression due to little [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen]] along the line of sight, and thus, very few absorption lines. 

![[lyman-alpha_low-z-source.png|align:center|400]]

For something far away ($z \gtrsim 6$), we see lots of suppression due to significant [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen]] along the line of sight, and thus, many of the wavelengths of the original spectrum will be absorbed by the time the light reaches us. 

![[lyman-alpha_high-z-source.png|align:center|400]]

This implies that hydrogen above $z\approx6$ is mostly neutral and mostly ionized below $z\approx6$.

![[hydrogen_ionization-time.png|align:center|400]]


> [!image] For a real spectra of a nearby (top) and far away (bottom) quasar...
> ![[Lya-forest-60.gif|align:center|500]]


## Absorption Process

We now look in more detail at the absorption process:

$$F(\lambda_{\rm obs})=F(\lambda_{\rm em}(1+z)) \,e^{-\tau} \hspace{1cm} \text{where} \hspace{1cm} \tau \equiv \text{optical depth}$$

Photons en route to the observer that pass through a $\ce{HI}$ cloud hit atoms in the ground state, which then transition to an excited state. Each transition has a frequency dependent cross-section, such that when the atoms relaxes to the ground state, a photon is emitted in some other direction within the solid angle $4\pi$.

Therefore, we can calculate the [[Optical Depth#Optical Depth|optical depth]] by...

$$\mathrm{d} \tau = n_{\rm HI} \, \sigma(\nu) \; \mathrm{d} l$$

- From atomic physics, we know the cross section ($\sigma$)...
	
	$$\sigma(\nu) = \left(\frac{\pi e^{2}}{m_{\rm e} c}\right) f_{12} \;\phi(\nu-\nu_{0})$$
	
	...where $f_{12}$ is the oscillator strength (i.e. the probability for absorption) and $\phi$ is the Voigt profile with $\int \phi \; \mathrm{d}\nu = 1$. For the [[Spectral Features#Lyman Series|Lyman]]-$\alpha$ transition, $\sigma(\nu)=10^{-2}\;{\rm cm}^{2}\phi(\nu-\nu_0)$ with units $\equiv {\rm cm^{2} \, Hz^{-1}}$.

- The [[Distances#Proper Distance|proper length]] ($\mathrm{d} l$) can be related to [[Redshift|redshift]] (taking only the magnitude and ignoring signs):
	
	$$\begin{aligned}
		\mathrm{d} l &= c \; \mathrm{d} t = c \, \frac{\mathrm{d} a}{\dot{a}} = \frac{c}{a}\frac{\mathrm{d} a}{\dot{a}/a} = \frac{c}{a}\frac{\mathrm{d} a}{H}
		= c (1+z) \, \frac{\mathrm{d} a}{\mathrm{d} z} \frac{\mathrm{d} z}{H} = \frac{c \; \mathrm{d} z}{(1 + z) H}
	\end{aligned}$$
	$$\mathrm{d} l = c \,\left(H_{0}(1+z)\sqrt{\Omega_{M}(1+z)^{3}+\Omega_{\Lambda}}\right)^{-1} \; \mathrm{d} z$$
	
	... where $a=1/(1+z)$ then $\frac{\mathrm{d} a}{\mathrm{d} z}=1/(1+z)^2$. For the matter dominated regime ($z\gtrsim1$), we get $$\mathrm{d} l = \frac{c \; \mathrm{d} z}{H_{0} \sqrt{\Omega_{M} (1+z)^{5}}}$$

The [[Optical Depth#Optical Depth|optical depth]] can then be calculated, assuming that $\phi$, which has a Gaussian shape, is very narrow such that we can approximate it as a delta function.

$$\begin{aligned}
	\tau_\nu &= \sigma_{0} \frac{c}{H_{0} \sqrt{\Omega_{M}}} \int_{0}^{z} \mathrm{d} z' \left[ \frac{n_{\rm HI}(z')}{(1+z')^{\frac{5}{2}}} \, \phi(\nu(1+z')-\nu_{0}) \right] \\
	&\approx \sigma_0\frac{c}{H_{0} \sqrt{\Omega_{M}}} \int_{0}^{z} \mathrm{d} z' \left[ \frac{n_{\rm HI}(z')}{(1+z')^{\frac{5}{2}}} \delta(\nu(1+z')-\nu_{0}) \right] \\
	&= \sigma_{0} \frac{n_{\rm HI}(z)}{H_{0} \sqrt{\Omega_{M}}} \cdot \frac{c}{\nu_{0}} \cdot \frac{1}{(1+z)^{\frac{3}{2}}} \\
	&= \sigma_{0} \frac{n_{\rm HI}(z)\lambda_{0}}{H_{0} \sqrt{\Omega_{M}(1+z)^{3}}}
\end{aligned}$$

...where $\sigma_0=10^{-2}\;{\rm cm}^2$ and $z$ is the redshift when $\lambda_{0} \equiv \frac{c}{\nu_{0}}= \lambda(1+z)$ (i.e. when absorption happens). This gives the optical depth for one frequency, such that it is necessary to evaluate at many frequencies to get the optical depth for different parts of a spectrum.

> [!example] 
> For instance, we can evaluate $\tau_\nu(z=3)$ assuming hydrogen is uniformly distributed and neutral. Using the following values...
> 
> $$\begin{aligned}
> 	H_{0} &= 70\;{\rm km/s/Mpc} = 2.3 \times 10^{-18}\;{\rm s}^{-1} \\
> 	n_{\rm HI} &= \frac{\rho_{\rm crit} \Omega_{b,0}}{m_{\rm H}}(1+z)^{3} \sim 10^{-5} \; {\rm cm^{-3}} \left(\frac{1+z}{4}\right)^{3} \approx 10^{-5} \; {\rm cm^{-3}} \hspace{1cm} {\rm at\ }z=3 \\
> 	\lambda_{0} &= 1216 \; {\rm \mathring{A}} \\
> 	\sigma_{0} &= 10^{-2}\;{\rm cm^{2}}
> \end{aligned}$$
> 
>  ...we find $\tau_{{\rm Ly}\alpha} \sim 10^{5}$, but we observe $\tau\sim1$.
> 
> The are a couple possible solutions to this discrepancy.
> - It could be that gas isn't in intergalactic space; however, we know that this is not the case since we have observed it.
> - The gas isn't neutral.
> 
> To bring $\tau_{{\rm Ly}\alpha}(z=3)$ down to $\sim1$, we need a neutral hydrogen fraction $X_{\rm HI}\equiv\frac{n_{\rm HI}}{n_{\rm H}}\sim10^{-5}$.
