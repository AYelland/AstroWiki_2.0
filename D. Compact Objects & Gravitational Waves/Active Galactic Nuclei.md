---
banner: "![[compact_objects.png]]"
banner_y: 0.5
aliases:
  - AGN
  - active galactic nuclei
---
## General Information

An **Active Galactic Nucleus (AGN)** is the highly compact region in a galactic center with an extremely high luminosity that does not originate from stars. The luminosity is theorized to arise from accretion onto a [[Black Hole#Supermassive Black Hole|SMBH]] in the galactic center.

*(Note: All AGN are found in the center of galaxies, but not all galactic centers are AGN)*

> [!measure] Typical Parameters & Properties
> 
> Approx. Mass: $M_{\rm BH} \lesssim 10^{6} - 10^{9} \; {\rm M_{\odot}}$
> Approx. Schwarzschild Radius: $R_{\rm S} \lesssim 10^{-3} - 10^{-2} \; {\rm pc}$ (highly compact)
> 
> Size of Disk: $\sim 10^{4} \; R_{g} \sim 100 \; \pu{pc}$ 
> Luminosity: $L \sim 10^{42} - 10^{48} \; {\rm erg/s} \quad (\simeq 10^{35} - 10^{41} \; {\rm W} \simeq 10^{9} - 10^{15} \; {\rm L_{\odot}})$

**Invalid Alternative Sources:**
- For a collection of stars to be this bright ($L_{\odot} \sim 10^{26} \; {\rm W}$), there would have to be $\sim 10^{9}$ [[Spectral Classes#G]] stars within $10^{-2} \; {\rm pc}$ $\implies$ unstable as stellar density is too high.
- For a supernovae ($E_{SN} \sim 10^{52} \; {\rm erg}$), they would need to occur a rate of $\sim 3 SN/yr$, requiring continual star production $\implies$ same problem as the source being stars (too dense and unstable).
- For a black hole, the nearby gas is gravitationally pulled into an accretion disk, heating up to temperatures $T \sim 10^{8} \; {\rm K}$. Assuming the accretion is [[Luminosity#Eddington Limit|Eddington-limited]]... $$L_{\rm Edd} \equiv \left(\frac{4 \pi G M c}{\kappa}\right) \simeq 3.2 \times 10^{4} \; \left(\frac{M_{\rm BH}}{M_{\odot}}\right) \, L_{\odot}$$

## Unified AGN Model

The **Unified AGN Model** explains the large differences seen in spectra between AGN when viewed form different lines-of-sight. 

#### Structure

Collectively, AGN are theorized to be consist of the following components.
- Supermassive Black Hole ([[Black Hole#Supermassive Black Hole|SMBH]])
- Accretion Disk
	- Broad Line Region (BLR)
	- Narrow Line Region (NLR)
- Jets at the Poles
- Corona (potentially near poles, but currently unknown)
- Torus shaped dust at edge of accretion disk
- Gas clouds scattering near the BH (outside of accretion disk)

> [!note] Jet Feedback
> - Accretion onto BH -> Jets -> Bubbles -> ICM.
> - Early stage is supersonic expansion until the movement of the bubble itself becomes faster than the expansion, then detachment of bubble. Enough energy in bubbles to balance radiative cooling

In a simplified image...

![[AGN_schematic.png|align:center]]

![[AGN_reverberationMapping_regions.jpg]]

Different coronal configurations:

![[BH_corona.png|Align:center|450]]

## Classifications

The different types of AGN being represented together is what creates the "unified" theory. Below is a diagram that represents all of the classifications of AGN based on the viewing angle, whether or not the AGN produces a significant jet (radio loud or radio quiet), and the rate of accretion onto the central SMBH (low or high electromagnetic power). 

> [!image]
> *(Source: https://zenodo.org/records/6381013)*
> 
> A schematic representation of an AGN in the orientation unified scheme. 
> 
> ![[agn_unification.png|align:center|600]]
> 
> The centre of the schematic shows the typical components of an AGN, though the precise geometry of these components are still unknown.
> 
> - Radio-loud objects are generally thought to display bipolar jet emission whereas it is only shown on the radio-loud side here. 
> 	- Note radio-quiet is not the same as radio-silent as many galaxies have low level radio emission, which is not significantly above that expected from star-formation and therefore it is unknown if these host radio jets or not. 
> - The upper left and upper right quandrants are commonly referred to as low and high excitation radio galaxies (LERG/HERG) respectively. 
> 	- LERGs are also known as hot mode, radio mode, jet mode, and radiatively inefficient sources.
> 	- HERGs are also known as cold mode, quasar mode, radiative mode, and radiatively efficient sources. 
> - We include some of the most commonly used names for different classes of AGN including...
> 	- broad line radio galaxy (BLRG)
> 	- narrow line radio galaxy (NLRG)
> 	- narrow emission line galaxy (NELG)
> 	- flat spectrum radio quasar (FSRQ)
> 	- steep spectrum radio quasar (SSRQ)
> 	- optically violent variables (OVV)
> 	- quasi-stellar objects (QSO)
> - Note that while we separate quasars and QSOs as being radio loud and radio quiet respectively, these names are often used interchangeably. 
> - Surrounding the central schematic we show whether a particular combination of power, radio emission, and geometry is expected to produce broad or narrow emission lines, or MIR, radio, X-ray, or gamma-ray emission. The transparency of the colour in each ring corresponds to the increasing strength or prevalence of a particular emission type.
^agn-schematic

![[AGN_unification_specifics.png|align:center]]

#### Type 1

- Angled view into an AGN, seeing past the torus
- Has both broad line emissions and narrow line emissions because there is little obscuration in the x-ray band

#### Type 2

- Side-on view of an AGN
- Lacks broad line emissions because the [[#Structure|BLR]] is heavily obscured in the x-ray band by the [[#Structure|torus]].

#### Radio Galaxy (RG)

-  $L_{\rm radio} \ge 10^{18}L_{\odot}$
-  radio emission from two external regions (radio lobes)
-  energized by jets (particle acceleration $E_e\sim10^{12}\:eV$
-  $\sim50\%$ E0/S0 galaxies, $\sim50\%$ quasars
-  synchrotron emission of electrons

#### Low Excitation Radio Galaxy (LERG)

- See [[#Radio Galaxy]]
- Radio Loud + Low EM Power
- Also known as hot mode, radio mode, jet mode, and radiatively inefficient sources.

#### High Excitation Radio Galaxy (HERG)

- See [[#Radio Galaxy]]
- Radio Loud + High EM Power
- Also known as cold mode, quasar mode, radiative mode, and radiatively efficient sources.

#### Narrow Line Radio Galaxy (NLRG)

- See [[#Radio Galaxy]]
- Radio Loud + Low/High EM Power
- A subtype of the [[#Type 2]] AGN classification
- Lacks broad line emissions because the [[#Structure|BLR]] is heavily obscured in the x-ray band by the [[#Structure|torus]].

#### Broad Line Radio Galaxy (BLRG)

- See [[#Radio Galaxy]]
- Radio Loud + Low/High EM Power
- A subtype of the [[#Type 1]] AGN classification
- Has both broad line emissions and narrow line emissions because there is little obscuration in the x-ray band

#### Steep Spectrum Radio Quasar (SSRQ)

- See [[#Radio Galaxy]]
- Radio Loud + Low EM Power
- Very similar to [[#Broad Line Radio Galaxy (BLRG)]], but with a steeper flux spectrum

#### Fanaroff–Riley Classification

Classification of [[#Radio Galaxy (RG)|radio galaxies]] with active nuclei based on their radio luminosity or brightness of their radio emissions in relation to their hosting environment 

- FR1 arms can look bent due to [[Fluid Mechanics#Ram Pressure]] as galaxy moves through [[Intracuster Medium|ICM]]
- FR2 often looks one-sided due to relativistic boosting

![[fanaroff_riley.png]]

confirmation is expensive, but is the proposed number of quasar pairs ~10^3? cant we estimate a population of 
What specific models are we trying to understand by quasar pair formation statistics?

#### Quasar / Quasi-Stellar Object (QSO)

- "Quasar" (quasi-stellar radio source): optical point source with radio jet
- "QSO" (quasi-stellar object): like a quasar but no radio emission

- A [[#Quasar]] and [[#Quasi-Stellar Object (QSO)|QSO]] are similar phenomena.
	- Of AGN sources found optically, $90\%$ are radio quiet (QSO), $\sim10\%$ are radio loud (Quasar)
-  Mostly found in elliptical galaxies
-  $L_{\rm quasar}\sim10^{45-48}\:$erg/s
-  synchrotron jets between $0.1 \; {\rm pc} - 1 \; {\rm Mpc}$
-  maximum space density $\sim z=2...3$

**Catalogs**: [[Catalogs#SDSS|SDSS]] and [[Catalogs#LAMOST]] 

**Observation strategies**: To observe the environment of a quasar you can use objects in the background (eg galaxies) and examine their light as absorbed by the environment of the quasar (ref: Christina Eilers talk)

#### Blazar

A [[#Quasar|quasar]] with a relativistic jet pointing along out line of sight. Have spectra dominated by featureless non-thermal continuum, which we would expect for a relativistic jet along the line of sight.

#### BL Lac

BL Lac objects are rapidly varying [[#Blazar|blazars]].

-  [[#Quasar / Quasi-Stellar Object (QSO)|quasar]] with enhanced continuum emission
-  highly variable
-  extremely luminous
-  highly polarized
-  jet pointing towards observer

#### Flat Spectrum Radio Quasar (FSRQ)

- Radio Loud + High EM Power [[#Blazar]]
- Same as [[#Optically Violent Variables (OVV)]]

#### Optically Violent Variables (OVV)

- Radio Loud + High EM Power [[#Blazar]]
- Same as [[#Flat Spectrum Radio Quasar (FSRQ)]]

#### Seyfert Galaxies

A Seyfert galaxy surround and AGN that is "Radio Quiet + Low EM Power", allowing the host galaxy to be easily seen.

-  spiral galaxies
-  bright unresolved nuclei (less luminous than quasars)
-  $L\approx10^{42}-10^{45}\:$erg/s

The different types (1, 1.5, 2) are in association with the [[#Type 1]] and [[#Type 2]] viewing angles.

#### Narrow Emission Line Galaxy (NELG)

Another name for a [[#Type 2]] [[#Seyfert Galaxies|Seyfert galaxy]]. Has 

## Examples

### Sagittarius A*
### Hercules A
### Makarian 501
### Spanish Dancer


