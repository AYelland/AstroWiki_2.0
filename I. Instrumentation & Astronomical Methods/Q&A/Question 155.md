### Question
---
How would you calculate the “signal-to-noise ratio” for a standard ground-based telescope performing CCD imaging? What terms dominate at optical versus infrared wavelengths? Why, when observing objects that are fainter than physical foregrounds like the night sky, does SNR increase as sqrt(time)?

### Answer
---
##### How would you calculate the “signal-to-noise ratio” for a standard ground-based telescope performing CCD imaging?

In the photon counting regime, we can quantify the total number of photons observed ($N$) and the various contributions to noise in those counts, without making explicit any frequency dependence.

**Signal:**
- $N$ = number of photons from the source + sky background + anything else
- $N_{\rm s} =$ **total number of photons from the star/source**, after calibrate and quantify the other sources ($N_b, N_{\rm d}, N_{\rm r}$ below), and subtract their counts, leaving an estimate of the total source counts.

**Noise contributions**:
- $n_{\rm pix} =$ **number of pixels**
- $\sigma_{\rm s} = \sqrt{N_{\rm s}} \hspace{1.3cm} \Rightarrow N_{\rm s} =$ Poisson noise from the **star/source**
- $\sigma_{\rm b} = \sqrt{n_{\rm pix} N_{\rm b}} \hspace{0.5cm} \Rightarrow N_{\rm b} =$ per-pixel Poisson noise from the **sky background**
- $\sigma_{\rm d} = \sqrt{n_{\rm pix} N_{\rm d}} \hspace{0.5cm} \Rightarrow N_{\rm d} =$ per-pixel Poisson noise from the **dark current** (thermal noise in electrons, decreases if we lower temperature)
- $\sigma_{\rm r} = \sqrt{n_{\rm pix} N_{\rm r}^{2}} \hspace{0.5cm} \Rightarrow N_{\rm r} =$ per-pixel noise from the **[[Tools#Read noise|read noise]]**

Assuming each the above contributions are independent, we can add them in quadrature such that the total magnitude of the noise is then...

$$\sigma = \sqrt{\sigma_{\rm s}^{2} + \sigma_{\rm b}^{2} + \sigma_{\rm d}^{2} + \sigma_{\rm r}^{2}} = \sqrt{N_{\rm s} + n_{\rm pix} \left( N_{\rm b} + N_{\rm d} + N_{\rm r}^{2} \right)}$$

Thus, the **signal to noise ratio (${\rm SNR}$) equation** (also known as the *"CCD Equation"*) is defined as:

$${\rm SNR} \equiv \frac{\rm signal}{\rm noise} = \frac{N_{\rm s}}{\sigma} = \frac{N_{\rm s}}{\sqrt{\sigma_{\rm s}^{2} + \sigma_{\rm b}^{2} + \sigma_{\rm d}^{2} + \sigma_{\rm r}^{2}}} = \frac{N_{\rm s}}{\sqrt{N_{\rm s} + n_{\rm pix} \left( N_{\rm b} + N_{\rm d} + N_{\rm r}^{2} \right)}}$$

> [!important] To note, the $\sigma$ values do **not** represent the *"standard deviation"*, but instead the *"uncertainty"* of measurement.

> [!note]- In practice using photometry...
> Assuming you know what your contribution to the dark current and read noise is known, you can set the following variables to the counts of pixels, times the gain of your telescope, to calculate the signal-to-noise.
> 
> - $g =$ gain of the telescope, allowing the conversion of counts (ADU) to number of photons
> - $n_{\rm pix} =$ number of pixels in the aperture
> - $N_{\rm s} =$ sum of counts in source aperture, minus the median of the collection of counts in the background aperture
> - $N_{\rm b} =$ median/mean of the collection of counts in the background aperture (representing the the number of counts per pixel) -- the choice can be dependent on use case
> 
> $${\rm SNR} = \frac{g N_{\rm s}}{\sqrt{g N_{\rm s} + n_{\rm pix} \left( g N_{\rm b} + g N_{\rm d} + g N_{\rm r}^{2} \right)}}$$ 

*(Useful [source](https://burro.case.edu/Academics/Astr306/Lectures/Lecture_20240205.pdf))*

##### What terms dominate at optical versus infrared wavelengths? 

At [[Electromagnetic Spectrum|optical]] wavelengths, we are usually object-limited, meaning the dominant source of noise is the large number of source counts $\sigma \simeq \sqrt{N_s}$ . 
- Though the percentage error decreases with number of counts for poisson processes, the magnitude of the error itself still increases. 
- Since this is assumed independent of the other sources, it will eventually dominate.

At [[Electromagnetic Spectrum|IR]] wavelengths, the dark current is significant so $\sigma \simeq \sqrt{N_d}$ .
- Why? not sure, but may be due to thermal motion of particles within material of telescope itself, hence cooling of [[Instruments#JWST|JWST]] for example.

##### Why, when observing objects that are fainter than physical foregrounds like the night sky, does SNR increase as sqrt(time)?

Look at the observation in terms of intrinsic rates multiplied by exposure times... $$N_{\rm s} = R_{\rm s} t \hspace{1cm} N_{\rm b} = n R_{\rm b} t \hspace{1cm} N_{\rm d} = n R_{\rm d} t \hspace{1cm} N_{\rm r} = n R_{\rm r}$$...where $n$ is the number of pixels, $R_{\rm s}$ has units $\left[ \text{photons per second} \right]$ and the other rates ($R$) have units $\left[ \text{photons per second per pixel} \right]$, noting that the read-out is time-independent. 

We can the rewrite the signal to noise (${\rm SNR}$) as:

$${\rm SNR} \equiv \frac{\rm{Signal}}{\rm{Noise}}= \frac{R_{\rm s} t}{\sqrt{R_{\rm s} t + n (R_{\rm b} t + R_{\rm d} t + R_{\rm r}^{2})}} = \frac{R_{\rm s} \sqrt{t}}{\sqrt{R_{\rm s} + n (R_{\rm b} + R_{\rm d} + R_{\rm r}^{2}/t)}}$$

Such that everything except readout noise-dominated, it scales as $\sqrt{t}$. 

> [!derivation] Limiting Cases
> 1) Bright Source/Object Limited: $${\rm SNR} \sim \left(\frac{R_{\rm s}}{\sqrt{R_{\rm s}}}\right) \sqrt{t}\quad \propto \sqrt{t}$$
> 2) Background/Sky Source Limited: $${\rm SNR} \sim \left(\frac{R_{\rm s}}{\sqrt{n R_{\rm b}}}\right) \sqrt{t} \quad\propto \sqrt{t}$$
> 3) Dark Noise Limited: $${\rm SNR} \sim \left(\frac{R_{\rm s}}{\sqrt{n R_{\rm d}}}\right) \sqrt{t} \quad\propto \sqrt{t}$$
> 4) Read-Out Noise Limited: $${\rm SNR} \sim \left(\frac{R_{\rm s}}{\sqrt{n R_{\rm r}^{2}/t}}\right) \sqrt{t} \quad\propto t$$
^9367ad

