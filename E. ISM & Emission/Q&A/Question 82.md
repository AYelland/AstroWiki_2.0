### Question
---
What kinds of sources are detected at TeV energies? What is the “cosmic gamma ray horizon”?

### Answer
---
##### What kinds of sources are detected at TeV energies?

- [[Active Galactic Nuclei|AGN]] and [[Active Galactic Nuclei#Blazar|Blazars]]
	- In jets electrons are accelerated and can spiral around internal magnetic field lines
	- This creates [[Synchrotron Radiation|synchrotron radiation]], which is then [[Inverse-Compton Scattering|inverse-compton scattered]] to higher and higher energies.
	- Similar mechanism in [[Binary Stars#X-Ray Binary|XRBs]].
- [[Gamma Ray Burst|GRBs]]
	- Same synchrotron-compton up-scattering mechanism as the jets mentioned above.
	- Fireball Model details in [[Question 67]]
- [[Stellar Explosions#Supernova]] Remnants
	- Shock fronts in SN explosions are efficient particle accelerators (thought to be main source of [[Interstellar Medium#Cosmic Rays|cosmic rays]]). 
	- If there is [[Synchrotron Radiation|synchrotron radiation]], the cosmic rays can produce TeV gamma rays via [[Inverse-Compton Scattering|inverse-compton scattering]].
	- Similar mechanisms in [[Nebulae#Pulsar Wind Nebula]], like the Crab Nebula 
		- See [[Question 62]], some of that energy accelerates particles in the nebula.
- [[Galaxy Classification#Starburst Galaxy (SBG)]]
	- Stars in these galaxies have relatively short lifetimes, lots of supernovae, ideal environment for [[Interstellar Medium#Cosmic Rays|cosmic ray]] production

##### What is the “cosmic gamma ray horizon”?

The **“cosmic gamma ray horizon”** is the energy and redshift-dependent [[Optical depth#Mean free path|mean free path]] for cosmic rays due to background light in the universe. (It is about $2\,\pu{Gpc}$ away from us.)

> [!important] Extragalactic Background Light (EBL)
> 
> ![[EBL.png|align:center|500]]
> 
> The light emitted by stars and [[Active Galactic Nuclei]] that permeates the Universe constitutes the **Extragalactic Background Light (EBL)**. It is a sea of photons that were emitted by these sources and reprocessed by the [[interstellar medium]] (gas and dust) of the host galaxy.  
^EBL

***How is this horizon formed?***

When a high energy photon coming from a source far away traverses the EBL, there is some probability that it will interact with EBL photons through a process called *[[#^pair-production|electron-positron (two-photon) pair-production]]*.

This means that some of those energetic photons will not arrive at our telescopes, and thus, the high-energy photon flux from distant sources is attenuated by the EBL. Additionally, because the density of EBL photons depends on [[redshift|redshift]] (the average rate of star formation is different at different epochs in the Universe), the probability of pair-production also depends on redshift. 

Given the probability of interaction, there will be a maximum effective distance that a high-energy photon can travel before before it encounters an EBL photon. That is, the universe will have some [[Optical Depth|optical depth]] for these high-energy photons due to the EBL. 

From the [[Optical Depth#^lambert-beer-law|Lambert-Beer law]]...

$$I_{\rm out} = I_{\rm in} \; e^{-\tau}$$

The **cosmic $\gamma$-ray horizon (CGRH)** is the energy/distance at which the [[Optical Depth#Optical Depth|optical depth]] is equal to unity ($\tau \sim 1$) as a function of redshift and energy. So, repeating the initial definition, the CGRH is the energy and redshift-dependent [[Optical Depth#Mean Free Path|mean free path]] for cosmic $\gamma$-rays due to background light in the universe.
 
 Current measurements place it at $z\simeq 0.5$ away from us ($\sim 2\,\pu{Gpc}$).

> [!note] Electron-Positron (two-photon) Pair-Production
> 
> ![[pair_production.png|align:center|200]]
> 
> **Two-Photon Pair Production** is the annihilation of the two photons and subsequent production of a particle-antiparticle pair.
> 
> For this to occur, the total energy of the two photons must surpass the rest energy of the particles created. (hence, this reaction is energy limited)
> 
> The easiest barrier to surpass is the rest mass of an electron-positron pair, since these have tiny masses. Because photons in the EBL typically have lower energies than the electron-positron rest mass, you need a very high energy photon to interact with a low-energy photon from the EBL to produce one such pair.
> ^pair-production