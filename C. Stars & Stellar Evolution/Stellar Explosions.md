---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
---
## Nova

A **nova** is the sudden appearance of a bright, apparently "new" star  that slowly fades over weeks or months. There are different types of mechanism that can cause this abrupt increase in brightness.

Star systems that showcase nova activity are considered to be [[Binary Stars#Cataclysmic Variables (CVs)]]. Meaning, they all involve [[Stellar Classes#White Dwarf|white dwarfs]] in close [[Binary Stars|binary systems]] with accretion from the secondary, donor star.

#### Classical Novae

When matter is accreted onto the surface a [[Stellar Classes#White Dwarf|white dwarf]] from the companion, creating a shallow, dense atmosphere mostly consisting of hydrogen. The atmosphere is heated and ignites hydrogen fusion on the surface in a runaway thermonuclear reaction.

- The hydrogen fusion uses the [[Carbon-Nitrogen-Oxygen Cycle|CNO cycle]]. 
	- Fusion begins $\rightarrow$ increases temperature $\rightarrow$ increases burn rate $\rightarrow$ repeat $\implies$ runaway reaction
- The nova event **blows off the rest of the hydrogen shell and can leave a nebulous remnant**
	- Mass Outflow Rate: $\sim 10^{2} - 10^{3} \; {\rm km/s}$

- Observations:
	- Often found in optical and IR
		- $10 - 20$ found in the Milky Way each year
	- Observe a [[Flux|flux]] increase by $\sim 10^{5} - 10^{6}$ ($> 12$ [[Magnitude|magnitude]] brightening)
	- Light curves rise on timescale of $\mathcal{O}(\rm hours - days)$, and decays on $\mathcal{O}(\rm weeks - months)$

#### Recurrent Novae (RNe)

Follows the same mechanism as the as the [[#Classical Novae]], except that the fusion ignition may be repetitive because the companion star will continue to feed the dense atmosphere of the [[Stellar Classes#White Dwarf|white dwarf.]]

#### Dwarf Novae

Smaller and less luminous outbursts that occur when accretion disk instabilities lead to sudden increase in mass accretion ($\dot{M}$) and a loss in gravitational potential energy. *(similar to the [[Pulsation#Kappa Opacity Mechanism]], but with viscosity)*

- Mechanism:
	1. There is thermal instability in accretion disk near the $\ce{H}$ (hydrogen) ionization temperature
	2. When $\ce{H}$ ionizes, the [[Optical depth#Opacity|opacity]] of the disk increases causing an effective increase in viscosity
	3. The higher viscosity allows the gas to flow and accrete faster (increases $\dot{M}$) from the donor to the accretion disk
	4. This increases the rate gravitational potential energy loss by material falling into the disk
	5. This energy loss is released through the luminous outbursts
	6. As it radiates and the disk's mass drops, the opacity and viscosity to also decrease causing to the luminosity to drop as well
	7. Returns to beginning of the cycle
   - This mechanism **does not eject material** from binary
   
- Observations:
	- Most abundant type of nova
	- Observe [[Flux|flux]] increase by $\sim 10-100$
	   - Lasts between 2 and 20 days and can exhibit quasi-periodicity on day to decade scales

## Supernova

A **supernova** is a very powerful and luminous explosion of a star. They occur during the last evolutionary stages of a massive star or when a [[Stellar Classes#White Dwarf|white dwarf]] is triggered into runaway nuclear reaction. The original object (called the progenitor) either collapses to a [[neutron star]] or [[black hole]], or is completely destroyed to form a diffuse [[Nebulae|nebula]]. The peak optical luminosity of a supernova can be comparable to that of an entire galaxy before fading over several weeks or months.

Theoretical studies indicate that most supernovae are triggered by one of two basic mechanisms: 

1. **The sudden re-ignition of nuclear fusion in a white dwarf** ("thermal runaway")
   In the re-ignition of a [[Stellar Classes#White Dwarf|white dwarf]], the object's temperature is raised enough to trigger runaway nuclear fusion, completely disrupting the star. Possible causes are an accumulation of material from a binary companion through accretion ("single-degenerate" progenitor), or by a merger with another white dwarf ("double-degenerate" progenitor). After the supernova, nothing remains as a remnant.
   
2. **The sudden gravitational collapse of a massive star's core** ("core collapse")
   In the case of a massive star's sudden implosion, the core of a massive star will undergo sudden [[Core-Collapse|collapse]] once it is unable to produce sufficient energy from fusion to counteract the star's own gravity. (This must happen once the star begins fusing iron, but may happen during an earlier stage of metal fusion.) A complete collapse will prevented by neutron degeneracy pressure, such that the collapsing material will "bounce" back and trigger a shockwave to move throughout the stellar envelope. When the shock wave reaches the surface, it expels the stellar material into the [[Interstellar Medium|ISM]], leaving behind a [[Neutron Star|neutron star]] or a [[Black Hole|black hole]].

For the final state of stars of different masses, see [[Question 40]].

### SNe Classification

![[sne_observational_chars.png|align:center]]

Supernovae are classified based on observational characteristics (i.e. light curves & spectral lines), not necessarily the exact nature of the progenitor system (which is not completely understood).

![[sne_classification_scheme.png|align:center|450]]

> [!note]
> The classification of supernovae is challenging and requires a complex ruleset, especially with the more specialized cases. For example, in the above image, it is entirely possible for a [SLSN to be associated with a long GRB](https://www.eso.org/public/archives/releases/sciencepapers/eso1527/eso1527a.pdf), or a [Type Ia to be cloaked in hydrogen](http://iopscience.iop.org/article/10.1086/420698/meta).
> 
> ([Helpful Source](https://astrobites.org/2016/12/02/classifying-supernovae/#:~:text=Type%20Ib%3A%20Type%20Ib%20supernovae,these%20spectra%20of%20these%20objects.))

### Type I

An overarching classification of supernovae that do not showcase hydrogen lines in their spectra. 

Subclasses include:
- [[#Type Ia]]
- [[#Type Ib]]
- [[#Type Ic]]
- [[#Type Ic-BL]]
- [[#GRB-SNe]]
- [[#Type I/II SLSN]]

### Type Ia

![[sne_type1a.png|aling:center|400]]

**Progenitor:** [[Stellar Classes#White Dwarf|white dwarf]] with mass above the [[Chandrasekhar Limit]] ($M \gtrsim 1.4 \; {\rm M_{\odot}}$)
**Remnant:** Nothing

Type Ia supernova are though to originate from the sudden re-ignition of nuclear fusion in a [[Stellar Classes#White Dwarf|white dwarf]] in a thermonuclear runaway. Provided that [[Stellar Classes#White Dwarf|white dwarfs]] shed their hydrogen envelope during the [[Hertzsprung-Russell Diagram#Post-Asymptotic Giant Branch (Post-AGB)|post-AGB]] stage (leaving only the hot, dense helium core), the supernova spectra lack hydrogen lines while having a strong silicon absorption line near its maximum luminosity.

**Other Notes:**
- Type Ia supernovae are the most common type of supernova event we observe.
- They produce most of the iron in the universe (during the explosion)
- All Type Ia SNe evolve with nearly the same evolution
	- Similar peaks in absolute, redshift-corrected [[Luminosity|luminosity]] ($M_{\rm V} \sim -19.5$ and $L \sim 10^{10} \; {\rm L_{\odot}}$)
	- Used as [[Cosmic Distance Ladder|standard candles]] to study cosmology

> [!spectra]
> - No hydrogen lines
> - Strong Silicon II (singly-ionized) lines

### Type Ib

**Progenitor:** [[Core-Collapse|core-collapse]] of a [[Stellar Classes#Wolf-Rayet Star]] ($M \gtrsim 30 \ {\rm M_{\odot}}$)
**Remnant:** Neutron Star

Type Ib supernovae originate when a massive star undergoes [[Core-Collapse|core-collapse]]. This star must been massive enough that its outer envelope of hydrogen would have been stripped away during the [[Hertzsprung-Russell Diagram#Post-Asymptotic Giant Branch (Post-AGB)|post-AGB]] stage by strong stellar winds. This is because we do not observe hydrogen in these spectra of these objects; however, we do observe the second ‘onion layer’ of helium.

> [!spectra]
> - No hydrogen lines
> - No silicon lines
> - Strong Helium II (singly-ionized) lines

### Type Ic

Type Ic supernovae form when a massive star undergoes [[Core-Collapse|core-collapse]]. The stars that produce these supernovae have both their hydrogen and helium layers stripped away during the [[Hertzsprung-Russell Diagram#Post-Asymptotic Giant Branch (Post-AGB)|post-AGB]] stage because we do not see hydrogen or helium in the spectra.

> [!spectra]
> - No hydrogen lines
> - No silicon lines
> - No helium lines

### Type Ic-BL

Type Ic – "Broad Lined" supernovae have very broad lines (a speed of 20,000 km/s for the bulk of the material!) compared to normal [[#Type Ic]]. These supernovae typically have higher kinetic energies than normal [[#Type Ic]], but the origin of the increased energy is unclear and a highly debated topic.

> [!spectra]
> - No hydrogen lines
> - No silicon lines
> - No helium lines
> - Broad spectral lines

### GRB-SNe

Some [[#Type Ic-BL]] supernovae are associated with [[Gamma Ray Burst|gamma-ray bursts (GRBs)]]. These events have been interpreted as the collapse of a massive star with the formation of a jet pointed in our direction, but the answer is unclear yet.

### Type II

An overarching classification of supernovae that showcase hydrogen lines in their spectra, and originate from very massive stars with short lifetimes ($M \gtrsim 8 \; {\rm M_{\odot}}$). Thus, they tend to be found in star-forming regions. 

These supernovae have a large variety in their light curves due to originating from a variety of progenitors. The attributes in the light curve and spectral line widths give rise to a handful of subclasses.

Subclasses include:
- [[#Type IIn]]
- [[#Type IIb]]
- [[#Type IIP/II L]]
- [[#Type IIpec]]
- [[#Type I/II SLSN]]

> [!spectra]
> - Hydrogen lines
> - Variety of light curves

### Type IIn 

Type IIn supernovae have very narrow (or slow) hydrogen lines in their spectra, superimposed on the typical broad lines. These narrow lines are interpreted as hydrogen which was blown off of the star _before_ it exploded.

> [!spectra]
> - Narrow (n) hydrogen lines

### Type IIP/II L

Type IIP/IIL supernovae contain relatively broad hydrogen lines. These explosions are thought to be the deaths of red supergiant stars, which are enshrined by their hydrogen envelopes. The light curves of Type IIP and Type IIL supernovae have distinctive shapes: a long plateau (P) lasting for hundreds of days and a "more" linear (L) shape - though not a straight line.

> [!spectra]
> - Broad (n) hydrogen lines

### Type IIb

Type IIb supernovae largely break our classification system. They begin with strong hydrogen lines, putting them in the Type II category; however, at late times they lose this hydrogen emission and instead resemble [[#Type Ib]]. These explosions are likely from stars which have lost part of their hydrogen envelopes.

> [!spectra]
> - Hydrogen lines (in the beginning) - decrease over time
> - No silicon lines
> - Strong Helium II lines (not until later) - increase over time

### Type IIpec
*(previously known as **Type III**, **Type IV**, or **Type V**)*

An additional supernovae class for SNe that do not cleanly fit the parameters for type I or type II supernovae.

### Type I/II SLSN

Type I/II SLSNe are *Superluminous Supernovae* that appear to be a subset of all supernovae and are ~100 times brighter than most other supernovae. Like normal, they are divided into Type I (lacking hydrogen) and Type II (showing hydrogen).
 
## Kilonova
*(also known as a **neutron star merger**)*

A **Kilonova** is a transient astronomical event that occurs in a compact [[Binary Stars|binary]] system (two [[Neutron Star|neutron stars]] or a [[Neutron Star|neutron star]] and a [[Black Hole|black hole]]) when the two companions merge. These mergers are thought to produce [[Gamma Ray Burst#Short Duration GRBs|short GRBs]] and emit bright [[Electromagnetic Spectrum|electromagnetic radiation]] due to the radioactive decay of heavy [[Neutron Capture#r-process]] nuclei that are produced and ejected fairly isotropically during the merger process.

It is called "kilonovae" since its peak brightness (within a week of the merger) is about a thousand times brighter than a [[#Nova|classical nova]] ($10-100$ times dimmer that a [[#Supernova]])

