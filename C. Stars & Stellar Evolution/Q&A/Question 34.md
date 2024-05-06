### Question
---
Describe the prominent neutrino producing reactions in the sun, and the experiments designed to detect them. What was the solar neutrino problem and how was it solved?

### Answer
---
##### Describe the prominent neutrino producing reactions in the sun...

> [!atom]- What are neutrinos?
>
> ![[SMparticles_neutrinos.png|align:center|500]]
> Neutrinos are...
> - Leptons (fermions) within the Standard Model of Particles
> 	- Charge: neutral
> 	- Mass: $m_{\nu} \le 0.8 \; {\rm eV/c^{2} \ (90\%\ CL)}$ 
> 	- Spin: $\hbar/2$
> - They have three generations (also known as flavors) associated with the other leptons (electron, muon, tau)
> - They only interact by the nuclear weak force (and are the only elementary particles that do), meaning they don't interact easily with matter and are hard to detect.

In the [[Sun]], they are produced in large quantities through the nuclear fusion reactions and lepton conservation. With a mean free path of $\sim 10\,\pu{pc}$, they are able to easily escape the [[Sun|sun]] after their production, such that if we can detect and measure them, we can directly probe the physics in the core of the Sun itself.

The primary production mechanism for solar neutrinos is through the [[Proton-Proton Chain|pp chain]]. In the associated neutrino-producing reactions, we expect them all to be electron neutrinos (initially).
- [[Proton-Proton Chain#PP I]] generates $\sim 90 \%$ of solar neutrinos in first step of the reaction chain. $$p + p \longrightarrow D + + e^{+} + \nu_{\rm e}$$
- [[Proton-Proton Chain#PP II]] generates $\sim 7 \%$ of solar neutrinos in first step of the reaction chain. $$\ce{^{7}Be} + e^{-} \longrightarrow \ce{^{7}Li} + \nu_{e}$$
- [[Proton-Proton Chain#PP III]] generates $\lesssim 1 \%$ of solar neutrinos in the boron decay. $$\ce{^{8}B} \longrightarrow \ce{^{8}Be + e^{+} + \nu_{e}} $$

##### ...and the experiments designed to detect them. 

- **Homestake Experiment** (1970) - a detector placed ~1 mile underground with the goal of detecting and measuring neutrino flux using a chlorine-based detector (100,000 gallon tank of perchloroethylene). 
	- When a electron neutrino ($\nu_{e}$) interacts with chlorine ($\ce{^{37}Cl}$), the atom transforms into a radioactive argon isotope ($\ce{^{37}Ar^{+}}$) that can be measured and counted. $$\ce{^{37}Cl} + \nu_{e} \longrightarrow \ce{^{37}Ar^{+}} + e^{-}$$
	- It was placed underground to avoid cosmic ray pollution in their measurements.
	- After running the experiment for 24 years, they were only able to measure (consistently) *one third* of the neutrino flux they expected to detect. 

- Other like **Super-Kamiokande** (Cherenkov detector using $e^{-}$ - $\nu_{e}$ scattering), **SAGE**, **GALLEX** confirmed the deficit.

##### What was the solar neutrino problem and how was it solved?

This discrepancy between experiment and theory became known as the "solar neutrino problem" where neither could account for the lacking/excess neutrinos.

The resolution is either:
1. There are problems with the fundamental physics in the solar models (i.e. we don't understand the Sun)
2. Something happens to the neutrinos on their way from the Sun to us

Turns out, neutrinos oscillate between mass states (known as generations or flavours) as they propagate! Detectors are only sensitive to electron neutrinos, and so if they oscillated between the different flavours (to the tau or muon neutrino state) after their emission, then we would only see about *one third* of the electron neutrino flux emitted by the Sun. 

This was proven true by the **Super-Kamiokande** experiment when they measured atmospheric neutrinos ($\nu_{e}$ and $\nu_{\mu}$ but not $\nu_{\tau}$) through cosmic ray spallation, and the discovery resulted in 2002 Nobel prize. 

Later, this was confirmed by Solar Neutrino Observatory that detected all 3 flavors and found about 1/3 of each, matching oscillation theory. 