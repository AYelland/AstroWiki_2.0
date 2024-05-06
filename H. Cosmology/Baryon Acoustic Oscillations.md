---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - BAO
  - baryon acoustic oscillations
---
> [!note] Sources
> - Images and Descriptions: [acoustics](http://background.uchicago.edu/~whu/intermediate/acoustic.html)
> - Overview Picture: [stackexchange](https://physics.stackexchange.com/questions/104010/connection-between-bao-und-cmb-spectrum)
> - Visualization of Freese-In: https://w.astro.berkeley.edu/~mwhite/bao/

**Baryon Acoustic Oscillations (BAO)** are fluctuations in the density of the visible baryonic matter (normal matter) of the universe, caused by acoustic density waves in the primordial plasma of the early universe.

The oscillations occur due to the coupling (i.e. interactions) of photons and baryons. With gravity being the driving force and radiation/photon pressure (from electron scattering) being the restoring force, the oscillations create density waves that propagate through the universe, like sound waves.

The speed in the baryon-photon fluid can be expressed as $c_{s} = c / \sqrt{3}$ , such that we can use the [[Distances#Angular Diameter Distance|angular diameter distance]] to find the sound horizon.

$$d_{A} = \frac{\ell_{s}}{\theta_{s}}$$

The BAO serve as the scale of the first [[Cosmic Microwave Background#CMB Power Spectrum]] peak as we'd measure it today. Shows up in galaxy-galaxy correlation function. $\sim 150\,\pu{Mpc}$ in today's universe.

![[BAO.jpg|align:center|500]]

## The Mechanism

Consider a system that starts in a rarefaction (diminution of baryon density)...
- Gravity acts on the baryons and pulls them in towards over densities, making then denser and compressing the fluid in potential wells set by [[dark matter]].
- Photon radiation pressure resists the compression and pushes the fluid back out, making the regions less dense and causing another rarefaction.
- This created conditions for "acoustic" oscillations (sound/pressure waves) of the photon-baryon fluid.

The maximum wavelength of these pressure waves at any given point in time was set by the distance a photon could have travelled since the big bang (as that effectively sets the maximum distance of causal connection).

![[BAO_wells.gif|align:center|300]]

This creates a system equivalent to a mass on a spring falling under gravity. In the image above, we think of the two balls as representing mass for springs, and analogously, the energy density for the early universe fluid. 

Looking at a bigger picture with multiple wells (seeded by quantum fluctuations during inflation), we find...

![[BAO_wells_multiple.gif|align:center|600]]

For different length scales, we have different modes of oscillation. For example, it takes half as long for the fluid to compress into a potential of half the length scale, leading to oscillations twice as fast (bottom mode below).

![[BAO_wells_mode.gif|align:center|600]]

---
## Relation to the CMB

The [[Cosmic Microwave Background|CMB]] power spectrum peaks originate from these acoustic oscillations. These oscillations are frozen in at [[Cosmological Timeline#Recombination]], when the photon-baryon fluid is decoupled.
- The acoustic modes (and therefore length scales) caught at extrema of their oscillation represent the peaks - characteristic scales with enhanced temperature fluctuations
- The wavenumbers (or spatial frequency) of the peaks are harmonically related to the fundamental scale - the distance sound can travel by recombination.

The fundamental scale (mode) reaches it maximum compression exactly when recombination occurs, such that it is the scale at which we see large temperature fluctuations. This length scale is the **sound horizon** and its angular size sets the position of the first peak of the CMB power spectrum. (see [[Cosmic Microwave Background#Sound Horizon]])

Because a scale half the size oscillates twice as fast, if the sound horizon scale $l_H$ reaches exactly first compression in the time it takes to reach recombination, then $2 l_H$ will reach exactly its first rarefaction by recombination (it will reach first compression in half the time to recombination). 

The harmonics of $l_H$ continue in this manner, leading to the following scales observed as being those with greatest temperature fluctuation relative to the mean:

![[cmb_compress_rarefact.png|align:center|500]]


A nice way to think about this is as resonant frequencies/wavelengths in a cavity/pipe. The scale of the effective cavity $L$ is set by the time to recombination and the sound speed as $L = t_{\rm rec} \, c_{\rm s}$, and the size admits a fundamental frequency/wavelength $\lambda_0 = 2L$  and harmonics of that frequency (unclear the exact nature of factors of 2 here).

![[BAO_sound_cavity_harmonics.png|align:center|400]]

### A more visual description...
*(Source: [stackexchange](https://physics.stackexchange.com/questions/104010/connection-between-bao-und-cmb-spectrum))*

Let us think about the universe as an open pipe, with a length set by the horizon (i.e. how far a photon has had time to travel up till that point in history) and grows with time as the universe expands and cools.

The fundamental mode of these acoustic oscillations in the pipe (i.e. the wavelength that can fit one half wavelength into the universe-pipe) will be the wavelength corresponding to one full compression (i.e. gravity, operating at light speed, has just had time to pull matter in, but the photon pressure hasn't had time to push it back out yet). 

The second harmonic/mode will be one full wavelength (i.e. gravity had time to pull matter in, the photon pressure pushed it out, and there hasn't been time enough for anything else yet). 

Of course, every wavelength shorter than the fundamental will exist, but at *any given snapshot in time*, only the integer multiples of the fundamental mode will constructively interfere to dominate the distribution of clumpiness of matter at that moment. All the rest will destructively interfere and average out to zero.

Eventually the universe cools enough for [[Cosmological Timeline#Recombination|recombination]]. All the electrons and protons get together, decoupling from the photons (due to the giant $13.6 \; {\rm eV}$ energy gap in Hydrogen) as they all just zip off in whatever direction they were going. Without the photon pressure to counteract the gravity, the oscillations stop.

- The baryons and dark matter are now free to succumb to gravity, and the current universe results. 
- The photons, which are now free-streaming, carry with them a distribution that exactly mirrors the state of the universe at recombination. This means that the photons will contain a picture of a universe, that has a specific fundamental frequency $\implies$ [[Cosmic Microwave Background|CMB]]

Since the fundamental tone (and all its integer multiples) define the clumpiness, a power spectrum made of the [[Cosmic Microwave Background|CMB]] will have a peak at each length scale that fits neatly into the pipe (i.e. the compression modes, the rarification modes, etc.). Thus, the power spectrum of the [[Cosmic Microwave Background|CMB]] should have an infinite number of peaks correlated to the infinite number of ever-shorter wavelengths that could perfectly fit into the universe pipe at recombination.

There two things tend to damp out the small scale fluctuations.
1. The first is that the last scattering surface (i.e. the CMB) is actually a shell. Recombination happened over a number of years, and so the thickness of that shell sets the minimum wavelength that we can see in the CMB today, as correlation information was lost as photons had to random walk out of that shell to freedom and they tended to walk from hot areas to cool areas because of diffusion. 
2. The second is basically every other thing (i.e. gravity) that effects photons on their 13 billion year journey to our telescopes. (see [[Cosmic Microwave Background#Anisotropies|CMB anisotropies]])

Fast forward to today, we can attempt to quantify the structure of the universe with respect to the early universe. One way to do this is by using the galaxy or cluster [[Question 122|correlation function]] to determine the spatial layout of baryons in our present day and see if any preferred length scales; however, its important to note that this is not an accurate tracer of mass (see [[Question 120]]).

The really useful thing here, is that by measuring the same thing at [[Cosmic Microwave Background|CMB]] times and now, we get a kind of cosmic ruler that helps us understand how the universe has expanded over the intervening billions of years. Ideally, we would make this same measurement somewhere in the middle (which is what the 21cm radio observatories are working on) to help put another tick mark on our ruler. Since the details of expansion are driven by dark energy, this helps us put some constraints on our understanding of what, exactly, it is (or at least maybe what it isn't).