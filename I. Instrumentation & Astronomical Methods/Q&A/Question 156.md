### Question
---
What is the diffraction limit for a telescope? Why does the signal-to-noise ratio scale like $D^{4}$ for diffraction limited imaging on ground-based telescopes with diameter $D$ at IR wavelengths?

### Answer
---
##### What is the diffraction limit for a telescope?

The **diffraction limit** is the minimum angular separation that can be resolved by a telescope, set by the observing wavelength and diameter of the telescope.

$$\theta_{\rm min} = \frac{1.22 \, \lambda}{D}$$

This arises from to the width of the central peak in an Airy disk (the diffraction pattern for light passing through a circular aperture - 2D analog of single slit experiment, [source](http://electron9.phys.utk.edu/optics421/modules/m5/Diffraction.htm)).

![[airy.png|align:center|400]]

> [!instrumentation]- Diffraction Spikes
> 
> **Diffraction spikes** are lines radiating from bright light sources, causing what is known as the starburst effect or sunstars in photographs and in vision. They are artifacts caused by light diffracting around the support vanes of the secondary mirror in reflecting telescopes or edges of non-circular camera apertures. (we can also see them around from the eyelashes and eyelids of the human eye.)
> 
> ![[diffraction-spikes.png|align:center|550]]

##### Why does the signal-to-noise ratio scale like $D^4$ for diffraction limited imaging on ground-based telescopes with diameter $D$ at IR wavelengths?

In [[Question 155]], we calculated the signal-to-noise ratio (${\rm SNR}$) in the photon counting regime in terms of photon rates for the source and the noise.

$${\rm SNR} = \frac{R_{\rm s} \sqrt{t}}{\sqrt{R_{\rm s} + n (R_{\rm b} + R_{\rm d} + R_{\rm r}^{2}/t)}}$$

For ground-based observations of a *faint* source in the [[Electromagnetic Spectrum|IR]], we will be in the counting regime (making this calculation valid) and [[Question 155#^9367ad|sky limited]], such that the SNR will scale with $\sqrt{t}$ (see [[Question 158]]). 

$${\rm SNR} = \fpar{R_{\rm s}}{\sqrt{n R_{\rm b}}}\sqrt{t}$$

We can now look at how the source photon rate ($R_{\rm s}$), the background photon rate ($R_{\rm b}$), and the number of pixels covered by our source and background ($n$) scales with the diameter of the aperture.

- **Source Photon Rate ($R_{\rm s}$):** defined similar to a power/luminosity, but using the source photon *number* flux ($F_{\rm s}$, counts per area per time) and $f$ is the optical throughput (unitless). $$R_{\rm s} = \fpar{\text{\# of source photons}}{\rm exposure\ time} = \td{N_{\rm s}}{t} = f F_{\rm s} \left( \pi \tfpar{D}{2}^{2} \right) \quad \propto D^{2}$$
- **Background Photon Rate ($R_{\rm b}$):** defined similar to the source photon rate, but uses the background photon *number* flux ($F_{\rm b}$, counts per area per time) and $f$ is the optical throughput (unitless). $$R_{\rm b} = \fpar{\text{\# of background photons}}{\rm exposure\ time} = \td{N_{\rm b}}{t} = f F_{\rm b} \left( \pi \tfpar{D}{2}^{2} \right) \quad \propto D^{2}$$
- **Pixel Coverage ($n$):** if our seeing is diffraction-limited, then the point=spread function (PSF) and the associated number of pixels covered the by the background and source drops off with respect to $\theta^{2} \implies n \propto D^{-2}$.  ![[snr_skynoise.png|align:center|200]] $$\theta_{1} \to \theta_{2} \hRightarrow n \propto \frac{1}{D^{2}}$$

Bring these three contributions together, we see that the diffraction limitation cancels with the $D^{2}$ scaling of background photon rate ($R_{\rm b}$), such that our ${\rm SNR}$ scales with...

$${\rm SNR} = \fpar{R_{\rm s}}{\sqrt{n R_{\rm b}}}\sqrt{t} \propto \fpar{D^{2}}{\sqrt{D^{2} \cdot D^{-2}}} \sqrt{t}\hRightarrow \boxed{{\rm SNR} \propto D^{2} \sqrt{t}}$$

Therefore, if we are trying to achieve some specific ${\rm SNR}$, then exposure time required scales inversely with the diameter.

$$\boxed{\; t \propto \frac{({\rm SNR})^{2}}{D^{4}} \;}$$

> [!note] A confusing question...
> 
> The question is confusingly worded and seems to imply that the ${\rm SNR}$ itself should scale with $D^{4}$, but this is not true-as we have seen, it scales like $D^{2}$. 
> 
> **Sources:** Chris Layden and Kevin Burdge both agree, as well as [this source](https://www.astro.princeton.edu/%7Ejgreene/ast303/Homework_4_soln.pdf) *(see the solution to problem 2b)*.


