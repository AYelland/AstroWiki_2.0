---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
  - HR-Diagram
  - HR diagram
  - H-R diagram
  - HRD
---
The **Hertzsprung–Russell diagram** is a scatter plot of stars showing the relationship between the intrinsic stellar [[Luminosity|luminosities]] (or [[Magnitude#Absolute Magnitude|absolute magnitudes]]) versus their [[Blackbody Radiation#Effective Temperature|effective temperatures]] (or [[Spectral Classes|spectral classifications]]). The clustering and structure that emerges represents the evolution of stars for various mass ranges.

![[HR_diagram1.png|align:center|600]]

![[HR_stages.png|align:center]]

As we look at the evolutionary stages below, we can keep this image in mind. This cycle represents the normal progression a star will repeat throughout its lifetime.

![[HR_cycle.png|align:center]]

*(Also see [[Mass Cut Diagram]] for a good overview for the evolutionary tracks of different massed stars)*

## Pre-Main Sequence

Star-formation begins when a molecular cloud (diffuse gas with low density and low temperature) satisfies the [[Jeans Formalism]] and begins to collapse.
- Initially, the collapse has negligible thermal pressure and acts on the [[Timescales#Dynamical Timescale|dynamical (free-fall) timescale]].
- Once the gas becomes optically thick ($\tau_{\nu} \gg 1$), the collapsing cloud is classified as a [[Stellar Classes#Protostar|protostar]] and begins collapsing under gravitational contraction on the [[Timescales#Thermal Timescale|thermal (KH) timescale]] while heating up.
	- This happens at $R \sim 100 \; {\rm R_{\odot}}$ and $T \sim 10^{3.6} \; {\rm K}$.
	- This is the star of the "pre-main sequence" stage. 

There are two phases as a protostar proceeds towards the [[#Zero-Age Main Sequence (ZAMS)]] line:
1. [[#Hayashi Track]] : Constant Effective Temperature (Isothermal) Contraction
	- Vertical Line on HR diagram
2. [[#Henyey Track]] : Constant Luminosity Contraction
	- Horizontal Line on HR diagram

The transition from the [[#Hayashi Track]] to the [[#Henyey Track]] corresponds to the transition from a convective to a radiative stellar envelope.

![[HR_hayashi_2.png|align:center|400]]
![[HR_preMS.png|align:center|700]]

### Hayashi Track

The **Hayashi Track** is where a protostar undergoes isothermal contraction ($T_{\rm eff} \sim$ constant) while in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]]. It represents a boundary called the **Hayashi Limit** between "allowed" and "forbidden" regions on the HR diagram for stars in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]], along with their lower bound on temperature and upper bound on radius.

![[HR_hayashi.png|align:center]]

> [!derivation]- Limiting Case of a fully Convective Star
> To calculate the boundary, we look at the limiting case of a fully convective star in hydrostatic equilibrium. We need...
> 
> - [[Stellar Structure#Hydrostatic Equilibrium]] $$\td{P}{r} = - \frac{G \rho \, m(r)}{r^{2}}$$
> - [[Blackbody Radiation#Effective Temperature]]-[[Luminosity]] Relationship $$L = 4 \pi R^{2} \sigma T_{\rm eff}^{4}$$
> - [[Thermodynamics#Ideal Gas Law]] for a hydrogen gas $$P = \frac{\rho k_{\rm B} T}{\mu m_{\rm p}}$$
> - [[Optical Depth#Opacity Law]] $$\kappa_{R} = \kappa_{0} \, \rho^{a} \, T^{b}$$
> - [[Polytropes|Polytropic Model]] for a Convective Star $$P(\rho, M, R) = K(M, R)\, \rho^{\gamma} \hWhere \gamma = 5/3$$
> 
> This all [combines together](https://en.wikipedia.org/wiki/Hayashi_track#Derivation) to yield...
> $$\log L \simeq 30 \log T_{\rm eff} - 4 \log M + {\rm constant}$$
> ...which is a very steep function of $T_{\rm eff}$. For constant $T_{\rm eff}$ and fixed $M$, the nearly-vertical line on the HR diagram is located around $\log (T_{\rm eff}) \simeq 3.6$ or $T_{\rm eff} \sim 4000 \; {\rm K}$.

**Important Notes:**
- Energy transport is *highly convective*.
- Newborn protostars start out in the forbidden zone, but rapidly move towards the Hayashi Track as their molecular cloud collapses
	- When it achieves [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]] at large radius and high temperature ($R \sim 100 \; {\rm R_{\odot}}$ and $T \sim 10^{3.6} \; {\rm K}$), it begins at the top of the Hayashi track
	- Progressing down the track, the protostar undergoes contraction on [[Timescales#Thermal Timescale|thermal (KH) timescale]] with $T_{\rm eff} \sim$ constant (adiabatic temperature gradient)
		- In the forbidden zone, temperature is superadiabatic
- As central density and temperature rise with contraction:
	- Radius decreases
	- Ionization increases
	- Opacity decreases
		- *Because neutral hydrogen does a lot of absorbing and ionized hydrogen just does a lot of scattering?*
	- Luminosity increases slowly ($T_{\rm eff}$ still low enough)
	- Energy transport becomes radiation dominant (transitioning to the [[#Henyey Track]])

### Henyey Track

The **Henyey Track** is where a protostar undergoes contraction with near-constant luminosity ($L \sim$ constant) until it reaches the [[#Zero-Age Main Sequence (ZAMS)]].

![[HR_henyey.png|align:center|400]]

**Important Notes:**
- Energy transport is *radiative*. (thermal radiation escapes as $\sim$ [[Blackbody Radiation|blackbody radiation]])
- Opacity follows [Kramer's Rule](https://en.wikipedia.org/wiki/Kramers%27_opacity_law)
	- Gas heated & ionized by gravitational contraction leading to decreased opacity
- Luminosity ($L$) remains roughly constant while radius ($R$) decreases.
$$T_{\rm eff} \propto \fpar{L}{R^{2}}^{1/4} \hRightarrow \text{protostar moves left on HR diagram}$$
- When central temperature becomes hot enough for [[_Stellar Nucleosynthesis#^methods-of-fusion|hydrogen fusion]], the [[Stellar Classes#Protostar|protostar]] becomes a [[Stellar Classes#Main Sequence]] star and it reaches the [[#Zero-Age Main Sequence (ZAMS)|ZAMS]] line.
	- Given that low-mass stars star the [[#Hayashi Track]] near the bottom, they don't have a [[#Henyey Track]] and begin immediately on the [[#Main Sequence (MS)]]
	- If the [[Stellar Classes#Protostar|protostar]] did not accrete enough mass for hydrogen fusion but it can still undergo [[Deuteron Fusion|deuteron burning]], then it will instead transition into a [[Stellar Classes#Brown Dwarf]].

## Zero-Age Main Sequence (ZAMS)

![[HR_preMS2b.jpeg|align:center|500]]

The **Zero-Age Main Sequence" (ZAMS) Line** is a theoretical locus of points in the [[#Hertzsprung-Russel diagram|HR-diagram]] where the luminosities of young stars (at a range of masses) are mostly supplied by the nuclear reactions that have begun in their cores. In other words, it is the line that represents when a [[Stellar Classes#Protostar|protostar]] becomes a [[Stellar Classes#Main Sequence|main sequence star]].

We often refer to the time since ZAMS as the age of the star, although the time for the collapse of the protostar prior to the ZAMS can be very significant. Additionally, we often use the *"mass at ZAMS"* as the mass of a star when discussing the evolution process the star will go through. (i.e. mass of star = mass when it entered the main sequence = ZAMS mass)

## Main Sequence (MS)

The **main sequence** comprises $\sim 90\%$ of known stars, including the [[Sun]], containing stars which are stably burning hydrogen in their core to fuse helium. This helium builds up in the core during the main sequence phase, but is not fused into carbon until core reaches $T_{c} \sim 10^{8} \; {\rm K}$. 

**For stars in the main sequence...**
- We can compute the structure numerically using the [[Stellar Structure|stellar structure equations]] and [[Nuclear Energy Generation Rate|nuclear reaction rates]].
- The mass of the MS stars can be correlated their luminosity.
	- The low-mass stars are at the bottom (low $L$) end of the MS.
	- The high-mass stars are at the top (high $L$) end of the MS.
- The means of energy transport can be distinguished by stellar mass.
	- Low-mass stars ($M \lesssim 0.5 \; {\rm M_{\odot}}$) 
		- *fully convective*
		- Low $M$ $\rightarrow$ Low $T$ $\rightarrow$ High $\tau_{\nu}$ $\rightarrow$ Convective transport
		- Essentially, star remain at the [[#Hayashi Track|Hayashi line]] after nuclear ignition
	- Medium-mass stars ($0.5 \; {\rm M_{\odot}} \lesssim M \lesssim 2 \; {\rm M_{\odot}}$) 
		- *radiative core & convective envelope*
		- As helium ash is produced, the convective region moves away from center
		- With higher temperatures, opacity decreases
	- Large-mass stars ($\gtrsim 2 \; {\rm M_{\odot}}$) 
		- *convective core & radiative envelope*
		- CNO burning becomes dominate energy generation method
		- Steep $T$ dependence yields a steep $\left|\td{T}{r} \right|$
- Changes in Composition of Core
	- At [[#Zero-Age Main Sequence (ZAMS)|ZAMS]]: $\left[ \; X = 0.74 \, , \, Y = 0.24 \, \implies \, \mu = 0.60 \; \right]$ (from [[Interstellar Medium|ISM]])
	- At [[#Terminal-Age Main Sequence (TAMS)|TAMS]]: $\left[ \; X = 0 \, , \, Y = 0.98 \, \implies \, \mu = 1.34 \; \right]$ (after H-core burning)
	- In stars with radiative cores, the composition changes shell by shell
	- In stars with convective cores, the shells are well mixed and the composition is homogeneous
- Their lifetime follows the [[Timescales#Nuclear Timescale]].
	- For radiative cores $f \approx 0.1$
	- For convective cores $f \approx 1$

When the fusible hydrogen in the core is exhausted, the star will transition into the [[#Post-Main Sequence]] stage.

## Terminal-Age Main Sequence (TAMS)

![[HR_TAMS.jpeg|align:center|300]]

The **Terminal-Age Main Sequence" (TAMS) Line** is not a term used often, but it is a theoretical line on the [[#Hertzsprung-Russel diagram|HR-diagram]] drawn for when stars "turn-off" (or leave) the [[#Main Sequence (MS)|main sequence]] and begin their evolutionary process.

## Post-Main Sequence

### Subgiant Branch (SGB)

The **Subgiant Branch** is the phase in stellar evolution after [[#Main Sequence (MS)|main sequence]] turn-off when the (non-fusing) helium core contracts and the hydrogen-rich envelope expands. All the while, the hydrogen shell burning adds more helium to the core. 

![[HR_SGB.png|align:center|600]]

**What happens when the hydrogen fuel is exhausted in the core?**
- The star accumulates an inert helium core, not undergoing helium fusion ($\varepsilon_{\rm m} = 0$).
	- The helium core is *isothermal* (seen from [[Stellar Structure|stellar structure equations]] of the core) $$\left\{ \begin{align} &\td{L}{r} = 4 \pi \rho r^{2} \varepsilon_{\rm m} = 0 \\ &\quad L(r=0) = 0 \end{align} \right\} \quad + \quad \left\{ \td{T}{r} = - \frac{3 \kappa_{\rm R} \rho L(r)}{16 \pi a c T^{3} r^{2}} = 0 \right\} \hRightarrow T = \text{constant}$$
- Core surrounded by thick hydrogen-rich envelope.
- At the bottom of the envelope, there is a hydrogen burning shell continuing deposit helium ash into core. 
	- This thermal pressure is enough to sustain the star and maintain equilibrium.
	- Overtime, this creates an instability since the isothermal core cannot support an arbitrary large envelope.
- The core pressure will eventually be overcome by gravity.
	- For $M \lesssim 2 \; {\rm M_{\odot}}$ stars, electron degeneracy pressure kicks in before the [[Schoenberg Chandrasekhar Limit]] is reached, providing additional core support. 
		- The degenerate core will continue to contract as mass is added ($R \propto M^{-1/3}$). This heats up $\ce{H}$-burning shell, increasing the burning rate and luminosity.
		- The excess energy from the contraction of the core causes the stellar envelope to expand, increasing $R$ and decreasing $T_{\rm eff}$.
	- For $M \gtrsim 2 \; {\rm M_{\odot}}$ stars, the [[Schoenberg Chandrasekhar Limit]] is reached and the core can no longer maintain [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]].
		- Core collapses on [[Timescales#Thermal Timescale|thermal timescale]] causing it to heat up quickly (relative to smaller stars) through gravitational contractions
		- The excess energy from the *gravitational* contraction of the core causes the stellar envelope to expand, increasing $R$ and decreasing $T_{\rm eff}$.

The star moves up and to the right on the HR diagram transitioning to the [[#Red Giant Branch (RGB)]] stage.

> [!note]
> The SGB phase is effectively the reverse of the [[#Henyey Track]] from [[#Pre-Main Sequence]]!

### Red Giant Branch (RGB)

The **Red Giant Branch** is when a star "isothermally" expands along the [[#Hayashi Track|Hayashi Limit]] and becomes more luminous due to the continued hydrogen shell-burning. Additionally, the convective envelope causes a "dredge-up" of nuclear ash to be visible on the stellar surface.

![[HR_RGB.png|align:center|500]]

**What happens with the star reaches the Hayashi limit?**
- The star is unable to virially adjust to the shell-burning's excess energy by further cooling while remaining in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]].
- Instead, it grows larger and more luminous.
	- $T_{\rm eff} \sim$ constant
	- $R$ increases
	- $L$ increases
- [[Stellar Classes#Red Giant|Red Giants]] have a convective envelope from the surface to the core, causing convective mixing and a *"dredge-up"* of nuclear ash in the core to the surface.
	- Directly alters surface composition.
	- Visible signatures of partial [[Carbon-Nitrogen-Oxygen Cycle|CNO burning]].
- The RGB phase only last about a small percent of the [[#Main Sequence (MS)|main sequence]] phase due to the higher luminosity ($L_{\rm RGB} \sim 50 L_{\rm MS}$). Since both act on the [[Timescales#Nuclear Timescale|nuclear timescale]]... $$t_{\rm RGB} \approx \frac{f \, \eta \, M \, c^{2}}{L} \sim \frac{f_{\rm MS} \, \eta_{\rm MS} \, M \, c^{2}}{50 \, L_{\rm MS}} \sim \text{few \% of }t_{\rm MS}$$
The star moves up on the HR diagram along the [[#Hayashi Track|Hayashi Limit]] ($T_{\rm eff} \sim$ constant). In larger stars, the [[#Red Giant Branch (RGB)|RGB]] stage is short but still present before the reversal with helium burning.

> [!note]
> The RGB phase is effectively the reverse of the [[#Hayashi Track]] from [[#Pre-Main Sequence]]!

### Helium Burning

At this point in the evolutionary process, the next phase after the [[#Red Giant Branch (RGB)|RGB]] is determined by the mass of the star.

**Very Low Mass Stars:** ($M \sim 0.08 - 0.5 \; {\rm M_{\odot}}$)
- The helium cores never get hot enough to ignite helium burning, but they are dense enough to be completely degenerate
- For $M \lesssim 0.3 \; {\rm M_{\odot}}$, the star is completely convective such that there is no build-up of a helium core. Eventually, H-burning will continue until star is completely helium.
	- Later will form a [[Stellar Classes#Red Dwarf]].
- For $0.3 \; {\rm M_{\odot}} \lesssim M \lesssim 0.5 \; {\rm M_{\odot}}$, the star develops a radiative core and convective envelope with a hydrogen burning shell, but still is unable to burn helium in the core.
	- Though not observed, stellar models expect that the weakly-bound envelopes are radiated away through stellar winds in the [[#Red Giant Branch (RGB)|Red Giant phase]] leaving behind a bare helium core, classified as a [[Stellar Classes#White Dwarf]].
	- Could also later form [[Stellar Classes#Red Dwarf]] instead?

**Low Mass Stars:** ($M \sim 0.5 - 2 \; {\rm M_{\odot}}$)
- The helium ignition in degenerate conditions leads to a thermonuclear runaway called a [[#Helium Flash]].
- After the flash, the core expands and cools, lifting degeneracy in the core and stabilizing the helium fusion
- Hydrogen shell-burning continues, but it is no longer being driven out of equilibrium by core contraction. The convective envelope stops expanding.
- The star begins a gradual transition to new equilibrium with stable helium fusion in the core. ($R$ decreases, $T_{\rm eff}$ increases $\implies$ [[#Horizontal Branch]])

> [!note] Lifetime on Low Mass Stars
> The timescale for a $M \sim 0.8 \; {\rm M_{\odot}}$ to turn off the [[#Main Sequence (MS)|main sequence]] is about the age of the universe. Meaning, very low mass stars are still stuck on the [[#Main Sequence (MS)|main sequence]] today. Much of the evolutionary process is still undetermined and speculative.

**Intermediate & Heavier Mass Stars:** ($2 \; {\rm M_{\odot}} \lesssim M \lesssim 8 \; {\rm M_{\odot}}$ & $M \gtrsim 8 \; {\rm M_{\odot}}$)
- The contracting core becomes hot enough to ignite helium burning ($T_{\rm c} \sim 10^{8} \; {\rm K}$) under non-degenerate conditions. The helium burning halts core contraction.
- Hydrogen shell-burning continues, but it is no longer being driven out of equilibrium by core contraction. The convective envelope stops expanding.
- The star begins a gradual transition to new equilibrium with stable helium fusion in the core. ($R$ decreases, $T_{\rm eff}$ increases $\implies$ [[#Horizontal Branch]])

#### Helium Flash

A **Helium Flash** occurs when the stellar core is degenerate ($M \sim 2.0 \; {\rm M_{\odot}}$) and the nuclear ignition becomes explosive through thermo-nuclear runaways. This appears at the "tip of the [[#Red Giant Branch (RGB)|red giant branch]]".

![[HR_heliumFlash.png|align:center|500]]

**Why does a helium flash occur in low mass stars?**
- The temperature of the core grows until it is hot enough for nuclear ignition; however, since degeneracy pressure is only dependent on density (not temperature)...
	- the core doesn't expand and cool
	- $T_{\rm eff}$ continues to increase but helium doesn't ignite
	- critical mass of $M \sim 0.45 \; {\rm M_{\odot}}$ is reached (determined by balancing degeneracy pressure  & thermal pressure)
	- many rapid nuclear reactions all occur at once, converting about 6% of the core into carbon through the [[Triple-Alpha Process|triple-alpha process]]
	- A total of $\sim 10^{11} \; {\rm L_{\odot}}$ is released in a few seconds (mostly absorbed by the envelope)
- This energy allows the core to expand and cool.
	- degeneracy is lifted
	- nuclear burning stabilizes
	- the reaction rate slows
	- this does not disrupt the star nor immediately changes its luminosity

Once the helium flash occurs, the star will peak on the [[#Red Giant Branch (RGB)|Red Giant Branch]] and transition to the [[#Horizontal Branch]] with stable helium burning in the core and [[Timescales#Thermal Timescale|KH contractions]].

#### Horizontal Branch

The **Horizontal Branch** occurs after the star begins stably fusing helium in the core and hydrogen in the shell. With the stable nuclear burning core, the star can virially adjust through  gravitational contractions and heating ([[Timescales#Thermal Timescale|thermal timescale]]) in the envelope. Any instabilities on the horizontal branch can lead to oscillations and [[Stellar Classes#Variable Stars|variable stars]].
- $R$ decreases
- $L\sim$ constant
- $T_{\rm eff}$ increases

![[HR_horizontalBranch.png|align:center|500]]

Throughout this branch, the star moves slightly down and to the left. The horizontal branch ends when all of the helium core-burning ends and an inert carbon-oxygen core is developed. (similar to the inert helium core).

#### Asymptotic Giant Branch (AGB)

The **Asymptotic Giant Branch** is similar to the [[#Subgiant Branch (SGB)|SGB]]+[[#Red Giant Branch (RGB)|RGB]] track, and occurs after the core helium is all burned to carbon and oxygen.

![[HR_AGB.gif|align:center|500]]

**For $M \lesssim 8 \; {\rm M_{\odot}}$ stars:**
- Inert carbon-oxygen core contracts and heats (on the [[Timescales#Thermal Timescale|thermal timescale]]) driving the helium burning shell out of equilibrium
	- Envelope expands and cools (similar to the [[#Subgiant Branch (SGB)|SGB]])
	- Once the star is unable to virially adjust to the helium shell-burning's excess energy by further cooling while remaining in [[Stellar Structure#Hydrostatic Equilibrium|hydrostatic equilibrium]]...
		- Hydrogen shell-burning becomes temporarily extinguished
		- Carbon-oxygen core becomes degenerate, slowing core-contraction
		- Convection in the envelope causes the *"second dredge-up"* of [[Carbon-Nitrogen-Oxygen Cycle|CNO]] products, alters surface composition.
- After the luminosity has increased and the star has traveled up the AGB track, the hydrogen shell will re-ignite leading to double shell burning and cyclic shell flashes called [[#Thermal Pulses (TP-AGB)|]] [[#^thermal-pulses-helium|"AGB thermal pulses"]].
	- These high temperature shell flashes lead to reaction chains that produce many neutrons, allowing the [[Neutron Capture#s-process]] to occur in the stellar envelope.
	- For $M \gtrsim 2 \; {\rm M_{\odot}}$ stars, convection in the envelope can cause a periodic *"third dredge-up"* of [[Carbon-Nitrogen-Oxygen Cycle|CNO]] products and [[Neutron Capture#s-process]] elements, once again altering surface composition.
		- This can produce carbon-rich stars

> [!note] Thermal Pulses (TP-AGB)
> 
> ![[HR_doubleShellBurning.png|align:center|500]]
> 
> Pulses are caused by...
> 1) The thick hydrogen burning shell re-ignites on top of the dormant helium layer.
> 2) Helium layer grows in mass, contracts, and heats up.
> 3) Helium burning ignites (non-degenerately) in a thin shell at the bottom of the helium layer (due to strong $T$ dependence).
> 	- Thermally unstable and explosive $\implies$ *"shell flash"*.
> 4) Energy absorbed by outer layers causing them to expand and cool, dousing hydrogen burning.
> 5) Helium burning front advance through helium layer until it reaches the hydrogen layer.
> 6) Proximity of helium burning re-ignites hydrogen burning. Helium burning runs out of fuel and stops.
> 7) Cycle repeats.
>
> Pulses have period of $P \sim 10^{3} - 10^{5} \; {\rm yr}$
^thermal-pulses-helium

Star moves up and to the right (decreasing $T_{\rm eff}$ and increasing $L$) until it reaches the [[#Hayashi Track|Hayashi Limit]]. Here, it "asymptotically" approaches the [[#Red Giant Branch (RGB)|RGB track]] (with a higher $R$ and $L$). At the late [[#Asymptotic Giant Branch (AGB)|AGB]] phase, the [[#Thermal Pulses (TP-AGB)|thermal pulses]] cause additional small peaks at the top of the [[#Asymptotic Giant Branch (AGB)|AGB]] track.

### Post-Asymptotic Giant Branch (Post-AGB)

[[#Asymptotic Giant Branch (AGB)|AGB]] stars have very strong stellar winds driving enormous mass loss. In late-[[#Asymptotic Giant Branch (AGB)|AGB]] phases, it can be as strong as $\sim 10^{-4} \; {\rm M_{\odot}/yr}$ (*"superwind"*). This mass loss strips away a lot of the envelope, extinguishing all shell burning.
- The star moves to the left on the HR diagram as the hot carbon-oxygen core is now exposed (classifying itself as a [[Stellar Classes#White Dwarf|C-O White Dwarf]])
- This core (still emitting high energy photons) ionizes the surrounding gas shells, creating a fluorescent [[Nebulae#Planetary Nebula|planetary nebula]].

This is the death of the star.

## Heavier-Element Burning

In  $M \gtrsim 8 \; {\rm M_{\odot}}$ stars, they can achieve higher thresholds for nuclear burning, fusing heavier elements than just helium. (carbon, oxygen, silicon, etc.)

![[HR_onionShellBurning.png|aling:center|400]]

- The inert carbon-oxygen core will ignite under non-degenerate conditions, and stably begin fusing carbon around $T_{\rm eff} \sim 6 \times 10^{8} \; {\rm K}$.
- Once the fuel is exhausted, the core will undergo normal gravitational contractions ( or degenerate core contractions) and heating around the new inert core.
	- The heating of the envelope will continue until the next nuclear burning threshold is reached, temporarily stabilizing the core (on the [[Timescales#Nuclear Timescale|nuclear timescale]]) through each nuclear reactions.
	- This allows the star to eventually cross each accessible nuclear burning threshold, creating an "onion skin" structure of burning and non-burning shells with an iron core
- Throughout this process, the luminosity is [[Luminosity#Eddington Limit|Edddington-Limited]], such that $L \sim$ constant across the entire evolution. $$L_{\rm Edd} = \frac{4 \pi c G M}{\kappa} \approx 3.2 \times 10^{4} \; \fpar{M}{M_{\odot}} \fpar{\kappa_{\odot}}{\kappa} \; L_{\odot}$$
- Eventually, the electron degeneracy pressure will not be able to provide sufficient support for the iron core ([[Chandrasekhar Limit]])
- Given that its [[Binding Energy#Nuclear Binding Energy|inefficient to fuse nuclei heavier than iron]] and the electron degeneracy pressure is too weak, the iron core will collapse causing a [[Core-Collapse|core collapse]] [[Stellar Explosions#Supernova|supernovae]] or [[Photodisintegration|photodisintegration]].

This collapse is the death of the star and birth of a compact object.


## Other Features of HR Diagram
### Instability Strip

A strip on the [[#Hertzsprung-Russel diagram|HR-diagram]] representing an instability of the radius and luminosity of stars due to density and pressure fluctuations. These fluctuations tend to often through the [[Pulsation#Kappa Opacity Mechanism]].

![[HR_instabilityStrip.jpg|align:center|500]]

Why doesn't this occur across all the HR diagram?
- On the low $T$ end (redder side), convection in the envelope can begin causing an increase in mixing and preventing the development of the [[Pulsation#Kappa Opacity Mechanism]]
- On the high $T$ end (bluer side), the $\ce{He}$ ionization zone is too far out in the stellar atmosphere to drive pulsations



### Lines of Constant Radius

If we assume that stars act as pure [[Blackbody Radiation|blackbodies]], then we can apply [[Blackbody Radiation#Stefan-Boltzmann Law]] such that...

$$
L = (4 \pi R^{2}) \; \sigma T^{4}
\hRightarrow
\log L = 4 \log T + \underbrace{\log(4\pi\sigma) + 2 \log R}_{\rm constant}
\hspace{1cm}
\textcolor{gray}{\left[ \; y = m x + b \; \right]}
$$

The lines of constant radius $(R)$ then appear as straight lines on the log-log space with a slope of 4. In linear space, this is a power law.

![[HR_constantRadius.png|align:center|350]]

> [!note] 
> Since $T$ increases to the left, the constant-radius line appears with a negative slope, with vertical offset scaling by $R$.

