---
banner: "![[instrumentation.png]]"
banner_y: 0.79
aliases:
---
## Effects

### Read Noise

A CCD can make accurate, but not perfect, measurements of the charge accumulated in each CCD pixel.  One important limitation is the noise associated with the electronics that amplifies and digitizes the charge signal in the CCD readout. Read-out noise is generated in the amplifier on the [[#CCD]] chip that converts the stored charge of each photodiode (i.e., pixel) into an analog voltage to be quantified by A/D conversion. Read-out noise may be viewed as a "toll" that must be paid for reading the stored charge. Similar to Poisson noise it scales with the number of "counts" but linearly rather than the square root: $$\sigma_r = N_r$$Measured by taking zero-count images i think(?) Unclear.

### Aberration

In optics, aberration is a property of optical systems, such as lenses, that causes light to be spread out over some region of space rather than focused to a point. This cause the image formed by a lens to be blurred or distorted.

![[aberration.png|align:center|400]]
## CCD
*(**Charge Coupled Device**)*

![[CCD.png|align:center|450]]

- An integrated (coupled) circuit of linked capacitors, whose response is proportional to the intensity of incoming radiation
	- Pixels are represented by individual capacitors covered by a photoactive material (silicon)
	- Each capacitor in the array can exchange charge with neighboring capacitors, which allows the signal in one pixel to travel to a charge amplifier, converting the signal from a pixel into a voltage. (i.e. number of electrons $\propto$ amount of light)
	- The thickness of the semi-conductor corresponds to the wavelength desired to be studied
- 2009 Nobel Prize
- The quality advantage of CCDs over [[#CMOS]] sensors has diminished in recent years. Both are based on metal oxide semiconductor (MOS) technology (CCDs on MOS capacitors, and [[#CMOS]] on [[#MOSFET]] amplifiers).
- Complications:
	- When a pixel gets oversaturated, it can cause the whole row of pixels to be oversaturated $\implies$ leaves lines in the output images
		- Counteracted by having the x-ray telescope move around when looking at a source ("dither") to avoid saturation, and use star tracker to reconstruct image
	- When a CCD is outputting data (i.e. emptying the capacitors), it cannot take any more data.

![[ccd-conveyorBelt.png|align:center|400]]
## MOSFET
*(**Metal-Oxide Semiconductor Field Effect Transistor**)*

Voltage across gate determines conductivity, effectively forming a non-mechanical switch which is controlled electronically.

## CMOS 
*(**Complementary Metal–Oxide–Semiconductor**)*

"Active pixel sensor / complementary [[#MOSFET|MOS(FET)]]". 


## Schmidt Camera

![[Schmidt_Camera.jpg|align:center|450]]

- Optical telescope with large FOV and limited [[#aberration]].
- Designed and first used in the 1930s
- Examples:
	- [[Instruments#Kepler]]
	- Hipparcos

## Cassegrain Telescope

![[Cassegrain_Telescope.svg|align:center|450]]

- A combination of a parabolic primary mirror and a hyperbolic secondary mirror
- Often used in optical telescopes and radio antennas
- Optical path folds back onto itself, relative to the optical system's primary mirror entrance aperture
	- Places the focal point at a convenient location behind the primary mirror
	- The convex secondary creates much longer focal length in a mechanically short system

## Ritchy-Chretien Telescope

![[RitcheyChretien.jpeg|align:center|450]]

- A specialized [[#Cassegrain Telescope]] with two hyperbolic mirrors (instead of a parabolic primary mirror) to eliminate off-axis optical errors
	- A "classic" Cassegrain has parabolic primary mirror and hyperbolic secondary mirror (Similar to Shmidt but replace plate with mirror)
- Examples:
	- [[Instruments#HST|HST]]
	- [[Instruments#VLT|VLT]]
	- [[Instruments#KECK|Keck]]

## Multi-Object Spectrograph

![[Multi-Object_Spectroscopy.png|align:center|300]]

- Spectrograph that can get a spectrum for multiple different targets/points on the sky at a given time. 
- Employed on almost all ground based telescopes these days.
- Many different types:
	- multi fiber ([[Catalogs#SDSS|SDSS]])
	- multi slit ([[Instruments#GMT|GMT]])
	- slitless (Nirspec on [[Instruments#JWST|JWST]])
	- integral field unit (IFU, e.g [[Instruments#Gemini|Gemini]])

## Echelle Spectrograph

![[echelle-spectragraph.jpg|align:center|400]]

- Diffraction grating that is optimized for high incident angles + high diffraction orders which gives better spectral resolution.
- Uses two gratings (one $\perp$ to the other) to cross disperse the light + separate the overlapping high orders
- Examples:
	- HARPS

![[echelle_spect.jpg|align:center|500]]
## Coronograph

![[coronagraph.jpg|align:center|400]]

- Instrument on a telescope used to block out the direct light from a star to see other dimmer features (e.g. the solar corona or exoplanets when [[Detection Methods#Direct Imaging Method|direct imaging]])
- Moon acts roughly like a coronagraph during solar eclipse
- Examples: 
	- [[Instruments#JWST|JWST]] has Nircam+MIRI
	- [[Instruments#HST|HST]] has NIMCOS
	- SOHO

> [!image] April 8, 2024 Solar Eclipse
> ![[2024_solar-ecllipse.png|align:center]]

## Laser Interferometer

![[interferometer.png|align:center|400]]

- Measures the change in proper distance due to [[Gravitational Waves|GW]] by looking at the interference of light (relative phases) that has traveled  in along two separate paths
- Example:
	- [[Instruments#LIGO]]

## Adaptive Optics

- Technology used to compensate for the blurring of ground-based astronomical images by the atmospheric turbulence
- Measure time-dependent deflection of bright source and correct that deflection. 
- Use deformable mirrors for calibration to 
	- Very bright guide sources/stars on the sky as "guides" for very fast timescale corrections. 
	- Sometimes shoot lasers into the atmosphere to create small, well-understood false "stars" to use for corrections instead.
- Examples: 
	- [[Instruments#VLT|VLT]]
	- [[Instruments#KECK|Keck]]
