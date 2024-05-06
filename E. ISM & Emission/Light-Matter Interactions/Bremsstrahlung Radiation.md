---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - free-free emission
  - bremsstrahlung
  - bremsstrahlung emission
  - bremsstrahlung radiation
  - braking radiation
---
 Sources:
 - https://www.astro.utu.fi/~cflynn/astroII/l3.html
 - https://casper.astro.berkeley.edu/astrobaki/index.php/Thermal_Bremsstrahlung
 
 **Bremsstrahlung Emission** (also known as **Free-Free Emission** or **Braking Radiation**) is when electromagnetic radiation produced by the deceleration of a charged particle when deflected by another charged particle. (mediated by the Coulomb Force)

 Typically, this is done by an electron and an atomic nucleus, such that as an electron passes close to an ion, it *feels* an acceleration, and an accelerating charge produces radiation.

![[scattering_bremsstrahlung.png|align:center|300]]

Given that both charged particles are unbound before and after interaction, it is also considered **free-free emission**. At higher temperatures where much of the material is highly ionized (i.e. plasmas), this type of radiation becomes very important.

By [[Larmor Formula]], we can determine that this type of radiation is more prominent from electrons (and lighter particles) than other species since the power scales inversely with mass.

### Spectrum

**Thermal Bremsstrahlung Radiation** is bremsstrahlung emission from a distribution of thermalized electrons following the [[Statistical Mechanics#Maxwell-Boltzmann]] distribution. 

The spectrum is divided into three regimes:
- **Optically thick** (low-frequency) - self-absorption becomes important as the radiation acts more like a [[Blackbody Radiation|blackbody]] (blackbody = perfect emitter/absorber = most efficient radiator). The emission is then blackbody limited by the [[Blackbody Radiation#Rayleigh-Jeans Law]]. ( $F_{\nu} \propto \nu^{2}$ ).
- **Constant Emission Rate** (mid-frequencies) - constant emissivity. (Why?) $$\text{Emissivity:} \hspace{1cm} \varepsilon \sim Z^{2} \, n_{e} n_{i} \,T^{-1/2} \hRightarrow \varepsilon_{\nu} \propto g(\nu, T) \varepsilon \, e^{-h\nu / k_{\rm B} T}$$
- **Optically thin** (high-frequency) - photons escape before the electrons can re-absorb them, but there is a thermal cut-off where you can't emit photon with much higher energy than $\nu \sim k_{\rm B} T / h$. (see [[Blackbody Radiation#Blackbody Specific Intensity|blackbody spectrum]])

![[scattering_bremsstrahlung_spectrum.png|align:center]]
