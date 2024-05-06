---
banner: "![[instrumentation.png]]"
banner_y: 0.79
aliases:
---
## Telemetry

The recording and communication of information from the instrument to us. In the context of space-based observatories, refers to return of data to Earth via a retrieval mechanism like the [[Instruments#Deep Space Network]].


## Long Baseline Interferometry
*(Abbrev. as **LBI** or **VLBI** for Very LBI)*

*Good Sources:*
- https://www.astro.princeton.edu/~gk/AST542/xuening.pdf
- https://www.eso.org/public/teles-instr/technology/interferometry/

By using long baseline interferometry (LBI), one can deploy multiple detectors to increase the effective resolution to an instrument of the same size as the separation between detectors (but with less light collection area). (See [[Question 153]])

Very-long-baseline interferometry (VLBI) is a type of astronomical interferometry that uses multiple radio telescopes on Earth or in space to detect a signal from a source. The distance between the radio telescopes is calculated using the difference between the arrival times of the radio signal at different telescopes. This allows simutaneous observations by many radio telescopes to be combined, emulating a telescope with a size equal to the maximum separation between the telescopes.

**Usage:**
- imaging distant cosmic radio sources (first image of [[Black Hole#Supermassive Black Hole|SMBHs]] wth [[Instruments#EHT]])
- spacecraft tracking
- measures the time differences between the arrival of radio waves at separate antennas
- Earth rotation studies
- map movements of tectonic plates very precisely (within millimeters)

**Simple Example**
The image below shows that detectors aligned colinearly improve the resolution along that axis (variation in that dimension of the image happens more quickly than orthogonal direction). Need to use at least a triangle if you want details in both dimensions

![[interferometry.png|align:center|500]]


## Strell Ratio

ratio of power in wings of psf versus in sharp bit in middle

## Reflection Spectroscopy
*(same mechanism as [[#Reverberation Mapping]])*

![[reflection_bh.png|align:center|500]]

As high-energy radiation is emitted from the corona, some of it can be reflected off the accretion disk. By measuring the shape of spectral lines (narrow or broad) emitted from the [corona](app://obsidian.md/Active%20Galactic%20Nuclei#Corona) and reflected off the accretion disk, we can constrain how fast the disk is moving. 

This gives a good estimation of where the $R_{\rm ISCO}$ is of a [[Black Hole|black hole]], given that it limits how closes of a radius the accretion disk can have. By using the [[Black Hole#^parameter-constraint|parameter constraints]] on the black hole, we can get a proxy for the spin.

## Reverberation Mapping

![[AGN_reverberationMapping.png|aling:center|500]]
![[AGN_reverberationMapping_regions.jpg|aling:center|500]]


As high-energy radiation is emitted from the corona, some of it can be reflected off the accretion disk. By measuring the temporal difference between the light received from the corona and the light reflected by the accretion disk, we can use the time lags to infer information about the environment very close to a black hole. *(See [this page](https://ned.ipac.caltech.edu/level5/March10/Peterson/frames.html) for a reverberation mapping overview.)*

**Optical/broad line region (BLR):**
Light-travel time induces a delay ($\tau_{\rm LT}$) that allows us that allows us to measure between optical broad lines (with respect to the continuum) and estimate location of the broad line region.

$$\tau_{\rm LT} \sim \frac{R_{\rm BLR}}{c}$$

We can further relate the mass of the black hole ($M_{\rm BH}$) to the location of the broad line region (BLR) through the velocity dispersion of the spectral lines.

$$M_{\rm BH} = \frac{f \, R_{\rm BLR} \, (\Delta v)^{2}}{G}$$where $f$ is a scale factor related to geometry and kinematics of the broad line region. It is usually $f \sim 5$.

Requirements:
- High time resolution ($\lesssim 1$ day)
- Long duration monitoring (~ months)
- Moderate spectral resolution ($\sim 600\,\pu{km\,s^{-1}}$)
- High signal-to-noise (SNR)

**X-ray**
Probe time delays between corona and disk in reflection features ($\tau_{LT, Xray} \ll \tau_{LT,opt}$). Can fit lag enegry spectrum to measure the mass, as the lag depends on the mass since we are probing $R_{\rm{ISCO}}$ 

## Photometry

See [[Photometry]].