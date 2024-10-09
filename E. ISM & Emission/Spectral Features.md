---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - spectra
---

> [!note] Spectral Lines Notation
> The spectral lines are notated according to the level of ionization of a chemical element. Neutral atoms are denoted with the Roman numeral $I$, singly ionized atoms with $II$, and so on. (i.e. $\ce{HI}$, $\ce{HII}$, $\ce{HeI}$)

## Parts of a Stellar Spectrum

### Absorption Lines

A [[Bound-Bound Absorption|bound-bound transition]] between two sharply defined states of energy. These are the distinguishing features in a stellar spectrum we call "spectral lines" that we use to determine a variety of stellar parameters. ([[Metallicity|metallicity]], radial velocity, chemical composition, temperature, surface gravity, etc.)

These spectral lines only pertain to a small range of energies, but can generate large changes in [[Intensity#Specific Intensity|specific intensity]] within this narrow energy range.

In a star, the a given nuclear fusion releases photons at a specific temperature. From there, the photon has to travel to the surface of the star before it is emitted and traveled to an observer. Similar to the photosphere of the Sun, we define the “surface” at the depth into the star where it becomes completely opaque. Based on the temperature of the star, the surface of the star is associated with different radial distances from the fusion reactions (in other words, height from the core). From there, the remainder of the star creates the stellar atmosphere. 

Thus, these absorption lines come from the atoms in the star itself, not the atmosphere. The strength of the spectral line is directly proportional to chemical abundance.

![[absorption_lines.png|align:center|500]]

> [!example] Considering two stars of equal mass and in the same stage in evolution...
> - For two stars with equal temperatures, the star with a higher metallicity will have more absorption lines, since the metals can absorb more photons at various energy levels.
> - For two stars with equal metallicity, a higher temperature (smaller photospheric shell and closer to the fusion reactions), the star would have less absorption lines since there is less physical area the light is traveling through before escaping the star.

### Continuum

Ions (such as $\ce{H^{-}}$) can capture free electrons in a [[Free-Bound Emission|free-bound transition]], emitting a photon. The energy of the photon is the difference between the original energy of the electron and its new energy in its bound state. This difference can have any value, and the cumulative effect of many of these [[Free-Bound Emission|free-bound transition]] is a continuous spectrum.

## Profile Effects
### P Cygni Line Profile

The **P Cygni line profile** is a spectroscopic feature that appears when a star has some expanding shell of gas surrounding it or strong stellar winds. The associated profile includes both a blue-shifted absorption line and a broadened, rest-wavelength emission line.

![[PCygniLineProfile_with_emission.png|align:center|600]]

The absorption line is blue-shifted as the light is accelerated by the expanding shell, such that it arrives to the observer faster. On the other hand, the emission line is composed of red-shifted, blue-shifted, and rest-frame emission light. This provides an overall net rest-frame spectral distribution, but it is broader than the normal emission distribution.

This feature arises from an expanding envelope around an ionizing source. Originally, it was found in the stellar wind from "P Cygni", a very luminous, blue variable star. It can also be found in [[Active Galactic Nuclei|AGN]] and other systems showing strong outflows.


### Relativistic Effects on Profiles

![[lineshape_effects.png|align:center|600]]
In the image above, the two dotted lines' spectra are shown with various effects included. The dotted lines are thin annuli on a non-relativistic disk. This spectral effect can be prevalent for rotating [[Black Hole|black holes]].

**Newtonian Effects:** 
- In a non-relativistic disk, each radius of the disk produces a symmetric double-horned line profile corresponding to emission from material on both the approaching (blue-shifted, right-hand) and receding (red-shifted, left-hand) side. 
- The inner regions of the disk, where the material is moving the fastest, produce the broadest parts of the line. 

**Special Relativity:** 
- Near a black hole, the orbital velocities of the disk are mildly relativistic.
- Through [[Redshift#Relativistic Doppler Effect]] ("moving clocks run slowly”), "beaming" enhances the blue peak of the line from each radius. 
	- This occurs when the relativistic material (usually through jets or relativistic [[Stellar Classes#Bipolar Flows|bipolar flows]]) traveling towards the observer.

**General Relativity:**
- Through the [[Redshift#Gravitational Redshift]] (“clocks near black holes run slowly”), the entire spectrum redshifts as the contribution from each radius moves to a lower energy. 

Summing the line emission from all radii of the relativistic disk gives a skewed and highly broadened line profile.


## Hydrogen Spectra

### Energy Levels

The energy levels of hydrogen are...

$$E_{n} = \left( \frac{- m_{\rm e} e^{4}}{2 \left( 4 \pi \varepsilon_{0} \hbar \right)^{2}} \right) \frac{1}{n^{2}} = \frac{-13.6 \; {\rm eV}}{n^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} \lambda = \frac{h c}{E_{\rm initial} - E_{\rm final}}$$

### Rydberg Formula

If some hydrogen atom $(Z=1)$ is in a stationary state of $\Psi_{nlm}$, then it could stay in that state forever; however, any perturbation such as a collision with another particle or light shining on the atom can cause a transition to another energy state. These *electron* transitions (or quantum jumps) are always occurring, causing the atom to gain or lose energy - moving up or down between energy states. When a hydrogen atom loses energy, it emits a photon through electromagnetic radiation. 

The **Rydberg formula** calculates the wavelengths of a spectral lines of electron transitions for a given hydrogen-like element.

$$
\frac{1}{\lambda} = R Z^{2} \left( \frac{1}{n_{1}^{2}} - \frac{1}{n_{2}^{2}} \right)
\hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}
	R &\equiv \text{Rydberg Constant} \\
	Z &\equiv \text{atomic number} \\
	n_{1} &\equiv \text{lower energy state} \\
	n_{2} &\equiv \text{higher energy state}
\end{aligned}
$$

The **Rydberg Constant** ($R_{\rm \infty}$) is combined with the reduced mass ($\mu$) of the nuclei-electron system prior to being used in the expression above.

$$R_{Z} = R_{\infty} \, \mu  = \left(\frac{m_{\rm e} e^{4}}{3 \varepsilon_{0}^{2} h^{3} c}\right) \left(\frac{(Z m_{\rm p})(m_{\rm e})}{Z m_{\rm p} + m_{\rm e}}\right) \approx 1.0973 \times 10^{7} \; {\rm [m]} \left(\frac{(Z m_{\rm p})(m_{\rm e})}{Z m_{\rm p} + m_{\rm e}}\right)$$

For hydrogen ($Z=1$), these expressions simplify to...

$$
\frac{1}{\lambda} = R_{\rm H} \left( \frac{1}{n_{1}^{2}} - \frac{1}{n_{2}^{2}} \right)
\hspace{1cm} \text{where} \hspace{1cm}
R_{\rm H} \approx 1.09678 \times 10^{7} \; {\rm m^{-1}}
$$

Using the Rydberg formula allows us to classify the different electron transitions by the energy they release. The first six sets (series) of transitions have been given names, with greek letters specifying the exact transitions.

| Name               | $n_{1}$ |    $n_{2}$     | <nobr>Convergence $(n=\infty)$</nobr> |
| :----------------- | :-----: | :------------: | :-----------------------------------: |
| [[#Lyman Series]]  |   $1$   | $2 \to \infty$ |    $\lambda \simeq 91 \; {\rm nm}$    |
| [[#Balmer Series]] |   $2$   | $3 \to \infty$ |   $\lambda \simeq 365 \; {\rm nm}$    |
| Paschen Series     |   $3$   | $4 \to \infty$ |   $\lambda \simeq 821 \; {\rm nm}$    |
| Brackett Series    |   $4$   | $5 \to \infty$ |   $\lambda \simeq 1459 \; {\rm nm}$   |
| Pfund Series       |   $5$   | $6 \to \infty$ |   $\lambda \simeq 2280 \; {\rm nm}$   |
| Humphreys Series   |   $6$   | $7 \to \infty$ |   $\lambda \simeq 3283 \; {\rm nm}$   |


### Lyman Series

The **Lyman Series** is transitions of electrons in atomic hydrogen to $n=1$ energy state. All wavelengths are emission in the [[Electromagnetic Spectrum|ultraviolet]]. ultraviolet

Using the notation from [[#Rydberg Formula]]...

| Name           | $n_{2}$  | $n_{1}$ | Wavelength ($\lambda$) | EM Spectrum Color |
| :------------- | :------: | :-----: | :--------------------: | :---------------: |
| Lyman-$\alpha$ |   $2$    |   $1$   |   $121 \; {\rm nm}$    |    Ultraviolet    |
| Lyman-$\beta$  |   $3$    |   $1$   |   $102 \; {\rm nm}$    |    Ultraviolet    |
| Lyman-$\gamma$ |   $4$    |   $1$   |    $97 \; {\rm nm}$    |    Ultraviolet    |
| Lyman-$\delta$ |   $5$    |   $1$   |    $95 \; {\rm nm}$    |    Ultraviolet    |
| $\dots$        | $\dots$  | $\dots$ |        $\dots$         |      $\dots$      |
| *Convergence*  | $\infty$ |   $1$   |    $91 \; {\rm nm}$    |    Ultraviolet    |

#### Lyman Limit

The **Lyman Limit** (or **break** or **discontinuity**) is the short-wavelength limit of the [[#Lyman Series]] ($\lambda = 91.13 \,\pu{nm}$), where electrons become completely ionized directly from the first energy/ground level of a hydrogen atom. This wavelength corresponds to the normal ionization energy of ground state hydrogen $\chi_{\rm H} = 13.6\,\pu{eV}$.

![[LymanLimit.svg|align:center|430]]
![[LymanLimit_spectra.jpeg|align:center|500]]


When there are a significant number of [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen atoms]] along some line-of-sight, any light with $\lambda < 912 \; {\rm \mathring{A}}$ (more energetic) will be absorbed. 

Since we know the wavelength of the Lyman Break in the rest frame (experimentally), by observing the break in the spectra of a source, we can determine its redshift (since at that stage the spectrum was the "most energetic"). For far away sources, we assume the light of a source hits the Lyman Limit along the line of sight, meaning we shouldn't see any flux at wavelengths smaller than $\lambda = 912\,\pu{Å} (1+z)$. 

For instance...

![[lymanLimit_sources.png]]

We should see source disappear in bluer filters if its at high redshift *(Rohan Naidu here at MKI uses this).*

![[LymanLimit_Sources_colored.jpeg|align:center|450]]

### Balmer Series
*(Historically the H-series with H-$\alpha$, H-$\beta$, etc.)*

The **Balmer Series** is transitions of electrons in atomic hydrogen to $n=2$ energy state. All wavelengths are emission in the [[Electromagnetic Spectrum|visible light and ultraviolet]].

Using the notation from [[#Rydberg Formula]]...

| Name              | $n_{2}$  | $n_{1}$ | Wavelength ($\lambda$) | EM Spectrum Color |
| :---------------- | :------: | :-----: | :--------------------: | :---------------: |
| Balmer/H-$\alpha$ |   $3$    |   $2$   |   $656 \; {\rm nm}$    |   Visible - Red   |
| Balmer/H-$\beta$  |   $4$    |   $2$   |   $486 \; {\rm nm}$    |  Visible - Cyan   |
| Balmer/H-$\gamma$ |   $5$    |   $2$   |   $434 \; {\rm nm}$    |  Visible - Blue   |
| Balmer/H-$\delta$ |   $6$    |   $2$   |   $410 \; {\rm nm}$    | Visible - Violet  |
| $\dots$           | $\dots$  | $\dots$ |        $\dots$         |      $\dots$      |
| *Convergence*     | $\infty$ |   $2$   |   $364 \; {\rm nm}$    |    Ultraviolet    |

#### H-alpha

The H-$\alpha$ (Balmer-$\alpha$) line comes from the electron transition from $n=3$ to $n=2$ in the atomic hydrogen atom (wavelength: $\lambda \simeq 656 \; {\rm nm}$).

It is important signature that appears in the spectra of many astrophysical sources, including:
- [[Nebulae#Emission Nebula]]
- The [[Sun|Solar]] Atmosphere (specifically, in solar prominences and the chromosphere)
- [[Interstellar Medium#HII Regions]] of the [[Interstellar Medium|ISM]]
- Star Forming Regions

#### Balmer Jump

The **Balmer Jump** (or **break** or **discontinuity**) is a large jump (difference of intensity) in the spectrum's continuum at the limit of the [[#Balmer Series]] ($\lambda \sim 364.5 \; {\rm nm}$), where electrons become completely ionized directly from the second energy level of a hydrogen atom. This is caused by the pair of effects:

- [[Bound-Free Absorption]] -  the ability of photons with high enough energies ($\lambda < 364.5 \; {\rm nm}$) to ionize the hydrogen atom.
- [[Bound-Bound Absorption]] -  the restriction of photons with lower energies ($\lambda > 364.5 \; {\rm nm}$) not being able to ionize the hydrogen atom.

When the atoms become ionized, the [[Optical depth#Opacity|opacity]] of a material will increase at the wavelengths shorter than the critical edge ($\lambda \simeq 364.5 \; {\rm nm}$). Therefore, if we have a source light behind some material, and a particular wavelength can ionize the material, you won't see much of that light on the other side. For [[Bound-Bound Absorption|bound-bound absorption]] though, we would just see lines.

This "jump" is related to (but distinct from) the [[#Lyman Limit]], which occurs at the wavelength which will just ionize a hydrogen atom from its ground state.

### 21cm line
The **21cm line** is a spectral feature representing the spin flip (hyperfine) transition in the ground state of neutral hydrogen ($\ce{HI}$). The corresponding energy of this transition is:
$$
\lambda = \frac{h c}{E_{1} - E_{2}} \sim 21.1 \; {\rm cm}
\hspace{1cm} \Rightarrow \hspace{1cm}
\nu \sim 1.42 \; {\rm GHz}
\hspace{1cm} \Rightarrow \hspace{1cm}
\nu \sim 0.7 \; {\rm ns}$$

![[21cm_spinflip.png|align:center|450]]

The degeneracy of the anti-aligned state is $g=1$ since the total spin quantum number is $S = (-\tfrac{1}{2}+\tfrac{1}{2}) = 0$. Alternatively, the aligned state has a degeneracy is $g=3$, with the total spin being $S = (\tfrac{1}{2}+\tfrac{1}{2}) = 1$.

|       Spin        |         Degeneracy          |                                  States                                   |
| :---------------: | :-------------------------: | :-----------------------------------------------------------------------: |
| $S=s_{1} + s_{2}$ |        $g = 2S + 1$         |                $\{ -S, \, -S+1, \, \dots, \, S-1, \, S \}$                |
|       $S=0$       |      $g = 2(0)+1 = 1$       |                                 $\{ 0 \}$                                 |
| $S=\tfrac{1}{2}$  | $g = 2(\tfrac{1}{2})+1 = 2$ |                  $\{ -\tfrac{1}{2}, \, \tfrac{1}{2} \}$                   |
|       $S=1$       |      $g = 2(1)+1 = 3$       |                          $\{ -1, \, 0, \, 1 \}$                           |
| $S=\tfrac{3}{2}$  | $g = 2(\tfrac{3}{2})+1 = 4$ | $\{ -\tfrac{3}{2}, \, -\tfrac{1}{2}, \, \tfrac{1}{2}, \, \tfrac{3}{2} \}$ |
|      $\dots$      |           $\dots$           |                                  $\dots$                                  |

The spin transition temperature ($T_{\rm spin}$) can be found from the Boltzmann relation:

$$\frac{n_{\rm u}}{n_{\rm d}} = \frac{g_{\rm u}}{g_{\rm d}} e^{-(E_{\rm u} - E_{\rm d}) / k_{\rm B} T_{\rm spin}} \hspace{1cm} \Rightarrow \hspace{1cm} k_{\rm B} T_{\rm spin} = \frac{E_{\rm d} - E_{\rm u}}{\ln (3 n_{\rm u} / n_{\rm d})}$$

For all but the coldest spin temperatures, $n_{\rm u} / n_{\rm d} \approx 3$.

**Observational characteristics**:
- Transition is very rare and happens on a timescale of $\sim 10\,\pu{Myr}$, but observable for very large amounts of neutral $H$ (low density to avoid collisional de-excitation) 
- Can be used to map neutral hydrogen in the "dark ages" between $z=1100$ and $z=6-20$ (i.e. the times between recombination and reionization) in radio wavelengths. 
- [[Instruments#CHIME]] and [[Instruments#HERA]] can observe it at low [[Redshift|redshifts]]. [[Instruments#MEERKAT|MEERKAT]] also did this recently. [[Instruments#SKA|SKA]] will observe out to $z=27$ 
- Can map neutral hydrogen in spiral arms of a galaxy, and can therefore use to constrain rotation curves.
- Comes from cold gas $\implies$ little thermal broadening.
- $(\lambda \sim 21 \; {\rm cm})$ is a  [[Electromagnetic Spectrum|microwave]] wavelengths, which pass mostly unobstructed through the atmosphere, and is therefore suitable for ground-based astronomy.

> [!bonus] Fun Fact!
> This hydrogen transition is depicted in the Pioneer Plaque on the top left. It is used as the unit of length and time for all of the other images depicted on the plaque as well. (Also, [[Instruments#Voyager]])
> 
> ![[Pioneer_plaque.svg|align:center|350]]



## Specific Spectral Lines

### Fe K-alpha Line

![[feKalpha_line.png|align:center|600]]

A fluorescent line that is a key feature in reflection spectra when observing an [[Active Galactic Nuclei|AGN]]. It shows up in [[Electromagnetic Spectrum|x-ray spectrum]] (6.4 keV). The $\ce{Fe K-\alpha}$ line is intrinsically a rather narrow line. Hence, when it is broadened (through [[#Relativistic Effects on Spectra|relativistic effects]]), we can use it to study the dynamics of the accretion disk. 

https://cxc.harvard.edu/ciao/workshop/oct17_pune/agn_chandra_workshop.pdf


### OII Doublet

Traces cool, ionized gas. Has been used to trace [[Circumgalactic Medium|CGM]]. Ratio of two lines depends on the temperature.



## Types of Sources

### Radio source
Atmosphere not too problematic, can perform radio observations even on cloudy days

**Solar system**:
- [[Sun]]
- Jupiter 

**Galactic**:
- [[Anatomy of a Galaxy#Galactic Center]]
- [[Neutron Star#Pulsar]]

**Extragalactic**
- [[Galaxy Classification#Radio Galaxy]]
- [[Fast Radio Burst#Fast Radio Burst]]


### X-ray background
**Sources**:
- Focused onto detector - Diffuse hot gas from Milky Way + unresolved point sources. Below 1-2keV, XRB dominates signal
- Particle BG - cosmic rays
- Unfocused cosmic hard X-ray background, constant in time

Apparently better to model your Xray background rather than to subtract it.



