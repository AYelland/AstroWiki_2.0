---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
---

![[cosmo_timeline2.png|align:center|550]]

![[particle_content_history.png|align:center]]

## Big Bang

> [!space] Time Since Big Bang: $\quad t = 0 \hspace{1cm} a = 0 \hspace{1cm} z = \infty$

## Cosmic Inflation

> [!space] Time Since Big Bang: $\quad t \sim 10^{-34} \; {\rm s} \hspace{1cm} a \sim  \hspace{1cm} z \sim$

**Cosmic inflation** (**cosmological inflation** or **inflation**) is a theory of exponential expansion of space in the early universe after the Big Bang. 

- We can treat inflation like a $\Lambda$-dominated period where $a \propto e^{\sqrt{\Lambda} t}$
- Expansion by a factor of $\sim 10^{26}$ on a timescale of $10^{-35} \; {\rm s}$
- Energy density remains $\sim$ constant

See [[Question 143]] for motivation of theory.

## Matter-Radiation Equality

> [!space] Time Since Big Bang: $\quad t \simeq 47,000 \; {\rm yr} \hspace{1cm} a \sim 10^{-4} \hspace{1cm} z \sim 3000$

At high redshifts (early times), radiation is the dominate process that drives the Hubble expansion of the universe ($H^{2} \propto z^{4}$). As the universe expands and cools, the matter term will begin to dominate the expansion processes. 

- $z \sim 3000$
- $T \sim 8500 \; {\rm K}$

> [!derivation] Redshift Calculation
> The [[Redshift|redshift]] of this transition can be found is at the Matter-Radiation equality using the [[Friedmann Equation]] and rough [[Instruments#Planck]] fit numbers.
> 
> $$H^{2}(z) = H_{0}^{2} \Big[ \underbrace{\Omega_{M} \, (1+z)^{3}}_{\rm matter} + \underbrace{\Omega_{r} \, (1+z)^{4}}_{\rm radiation} + \Omega_{k} \, (1+z)^{2} + \Omega_{\Lambda} \Big]$$
> 
> $$\Omega_{r} (1+z)^{4} = \Omega_{M} (1+z)^{3} \hRightarrow z = \left( \frac{\Omega_{M}}{\Omega_{r}} -1 \right) \simeq \left( \frac{0.3}{10^{-4}} - 1 \right) \simeq 3000$$
^MR-z

> [!derivation] Temperature Calculation
> With the [[Cosmic Microwave Background|CMB]] temperature ($T_{0} = T_{\rm CMB} \sim 2.7 \;{\rm K}$), we can use the redshift of recombination ($z_{\rm mr} \sim 3000$) to find the temperature at this transition.
> 
> $$T_{\rm mr} = T_{0} (1+z_{\rm mr}) \sim 8500 \; {\rm K}$$
^MR-T

## Recombination

> [!space] Time Since Big Bang: $\quad t \simeq 378,000 \; {\rm yr} \hspace{1cm} a \simeq 10^{-3} \hspace{1cm} z \simeq 1100$

Recombination is the epoch during which the universe had expanded and cooled enough that charged electrons and protons first became bound to form electrically neutral hydrogen atoms. After which [[Thomson Scattering|Thompson scattering (electron scattering)]] occurs far less frequently, such that matter and light are decoupled, and the light travels unimpeded through the universe ([[Cosmic Microwave Background|CMB radiation]]).

> [!note] Bad Naming...
> The name "recombination" is misleading, since the Big Bang theory doesn't posit that protons and electrons had been combined before, but the name exists for historical reasons since it was named before the Big Bang hypothesis became the primary theory of the birth of the universe.

> [!derivation] Redshift Calculation
> If we model the universe as system composed purely of "one level hydrogen atoms" (that is only protons and electrons and a 1-level H atom with ionization energy $\chi_{\rm II} = 13.6\,\pu{eV}$), then we can use the [[Saha Equation]] to determine the ratio of ionized to neutral hydrogen.
> 
> $$\frac{n_{\rm II} \, n_{e}}{n_{\rm I}} = \fpar{g_{e}\,g_{\rm II}}{g_{\rm I}} \fpar{2 \pi m_{e} k_{\rm B} T}{h^{2}}^{3/2} \,e^{-\chi_{r} / k_{\rm B} T}$$
> 
> ...where $T = T_{0} (1 + z)$ from the [[Friedmann Equation]] where $\rho_{rad} \propto (1+z)^4$ and the equation of state follows [[Stellar Structure#Radiative Energy Transport|radiation energy transport]] mechanism.
> 
> $$P = \frac{4\sigma}{3c}T^{4} = \frac{1}{3} a T^{4} \hRightarrow \rho_{rad} \propto P_{rad} \propto T^{4}$$
> 
> Number density of ionized hydrogen (protons) is given by...
> 
> $$n_{\rm II} \equiv n_{\rm p} = \frac{\rho_{b}}{m_{p}} = \frac{ \Omega_{b} \rho_{c} (1+z)^{3}}{m_{p}}$$
> 
> ...such that we can get the redshift when the medium is half ionized ($n_{\rm I} \equiv n_{\rm II} \equiv n_{\rm e}$).
> 
> $$n_{\rm II} = \frac{n_{\rm II}^{2}}{n_{\rm II}} = \frac{n_{\rm II} \, n_{e}}{n_{\rm I}} = \fpar{g_{e}\,g_{\rm II}}{g_{\rm I}} \fpar{2 \pi m_{e} k_{\rm B} T}{h^{2}}^{3/2}  \exp \left[-\frac{\chi_{r}}{k_{\rm B} T_{0}(1+z)}\right]$$
> 
> By solving numerically for $z$, we find $z_{rec}\simeq 1500$, but this is an overestimate. Why?
> - There are other elements which will recombine earlier due to higher ionization energies
> - The H atom does not recombine straight to the ground state. Instead it will spend some time with the electron in an excited state and the de-excite eventually. The 2-level treatment of the hydrogen atom in this context gives a different redshift (see image below)
> 
> ![[cosmo_recombination.png|align:center|400]]
^rec-z

> [!derivation] Temperature Calculation
> With the [[Cosmic Microwave Background|CMB]] temperature ($T_{0} = T_{\rm CMB} \sim 2.7 \;{\rm K}$), we can use the redshift of recombination ($z_{\rm rec} \sim 1100$) to find the temperature at recombination.
> 
> $$T_{\rm rec} = T_{0} (1+z_{\rm rec}) \sim 3000 \; {\rm K}$$
> 
> The ionization energy of hydrogen is about $13.6\,\pu{eV}$ which would correspond to a thermal temperature on the order of $T \simeq E/k_{\rm B} \simeq 10^{5} \,\pu{K}$  (using $k_{\rm B} \simeq 10^{-4}\,\pu{eV K^{-1}}$). This implies we should have recombined much earlier than the redshift at which $T$ was $3000\,\pu{K}$. 
> 
> The reason it takes longer to reach half ionization is that the photon energy distribution has a long tail which keeps things ionized for longer (think of it as a [[Blackbody Radiation#Blackbody radiation|BB]] with peak temperature much smaller than that required to ionize, but the tail is long so it can still do so).
> 
> ![[photon_tail.png|align:center|575]]
> 
^rec-T

## Dark Ages

> [!space] Time Since Big Bang: $\quad t \simeq 0.3 - 380 \; {\rm Gyr} \hspace{1cm} a \sim \hspace{1cm} z \sim$

After [[#Recombination]], matter and light are decoupled, allowing the original [[Cosmic Microwave Background|CMB]] light to travel unimpeded through the universe. Since the all of the matter is neutral in this era and doesn't emit light, we can cannot probe how the clumping matter as it formed structures in association with the underlying density fluctuations.

The dark ages came to an end with the light of the first stars ([[Stellar Populations#Population III (Pop. III)|Pop. III]]).

## Reionization

> [!space] Time Since Big Bang: $\quad t \simeq \hspace{1cm} a \sim \hspace{1cm} z \sim 25-6$

The epoch of reionization occurs when star formation, [[Active Galactic Nuclei|AGNs]], and other ionizing sources become prominent sources in the universe and slowly ionize the [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen]]. 

The epoch of reionization ended when the majority of the universe became ionized ($z \sim 6 - 25$, with large uncertainties)

![[cosmo_reionization_megan.png|align:center]]

**How are these measurements made?**
- [[Lyman-Alpha Forest]] measurements of high $z$ [[Active Galactic Nuclei#Quasar / Quasi-Stellar Object (QSO)|quasars]]
- [[Spectral Features#21cm line|21cm]] $\ce{H}$ intensity mapping
- [[Optical Depth]] of the [[Cosmic Microwave Background|CMB]] $$\tau(z) = \int \sigma_{T} \, n_{e} \; \rd s = \int \sigma_{T} \, n_{e} (1+z)^{3} \; \left( c \; \rd t \right)$$

> [!note] How does the hydrogen get ionized?
> 
> Ionization can occur in hot temperatures. We can estimate the temperature of the early universe from absorption line widths in [[Active Galactic Nuclei#Quasar / Quasi-Stellar Object (QSO)|quasar]] spectra (see [[Lyman-Alpha Forest]]); however, we find that this temperature is not high enough to ionize hydrogen.
> 
> $$\frac{1}{2} m v^{2} \sim k_{\rm B} T \hRightarrow	\Delta v \sim 20\; {\rm km/s} \sim \sqrt{\frac{2 k_{\rm B} T}{m}} \hRightarrow T \sim 30,000 \; {\rm K} \sim 3 \; {\rm eV}$$
> 
> Another option is photoionization. 
> - The integrated light from galaxies and quasars is emitted at a rate of $\Gamma\sim10^{-12}$ ionizing photons per second. The ionization rate is then $n_{\rm HI} \cdot \Gamma$, such that the ionization timescale is...
> 	
> 	$$\frac{n_{\rm HI}}{n_{\rm HI} \, \Gamma}\sim10^{12}\;{\rm s}\sim30,000\;{\rm yr}$$
> 
> - We can compare this timescale with the recombination rate $R \, n_{\rm HII} \, n_{\rm e}$, where $R=4.3\times10^{-13}\left(\frac{T}{10^4\;{\rm K}}\right)^{-0.7}$. This gives a timescale of...
> 	
> 	$$\frac{n_{\rm HII}}{R \, n_{\rm HII} \, n_{\rm e} } \sim 2 \times 10^{17}\;{\rm s} \sim 3 \times 10^{6} \;{\rm yr}$$
> 	
> - This shows that recombination is much slower than ionization, and photoionization is plausible mechanism of ionization. 
> 
> To establish the predicted ionization fraction, we find equilibrium by setting the ionization and recombination timescales equal, and assume that $n_{\rm HII} \sim n_{\rm e} \sim n_{\rm H}$ and $n_{\rm HI}\ll n_{\rm HII}$. 
> 
> $$R \,n_{\rm HII} \,n_{\rm e} = \Gamma \,n_{\rm HI} \hRightarrow R \,n_{\rm H}^2 = X_{\rm HI} \,n_{\rm H} \,\Gamma$$
> 
> This gives a neutral fraction of...
> 
> $$X_{\rm HI} \approx \frac{R n_{\rm H}}{\Gamma} \sim 5\times10^{-6}$$
> 
> So at the present day, the ionization fraction is very small. However, it took a while between [[#Recombination]] and the present day for ionizing sources to form and begin emitting radiation to ionize the neutral gas. 
> 
> ![[ionization_fraction-1.png|align:center|450]]
> 
> Once they formed, the gas was ionized over a period of time. Before recombination, the gas was mostly ionized in the hot universe. Exactly how and when reionization occurred is an active area of research that is being probed by both telescopes like [[Instruments#HERA]] and simulations like THESAN.

## Matter-$\Lambda$ Equality

> [!space] Time Since Big Bang: $\quad t \simeq 9.8 \; {\rm Myr} \hspace{1cm} a \sim 0.75 \hspace{1cm} z \sim 0.33$

Using rough [[Instruments#Planck]] numbers, the time of Matter-$\Lambda$ equality can be found using the [[Friedmann Equation]].

$$H^{2}(z) = H_{0}^{2} \Big[ \Omega_{M} \, (1+z)^{3} + \Omega_{r} \, (1+z)^{4} + \Omega_{k} \, (1+z)^{2} + \Omega_{\Lambda} \Big]$$

$$\Omega_{\Lambda} = \Omega_{M} (1+z)^{3} \hRightarrow z = \left( \frac{\Omega_{M}}{\Omega_{\Lambda}} -1 \right)^{1/3} \simeq 0.33$$