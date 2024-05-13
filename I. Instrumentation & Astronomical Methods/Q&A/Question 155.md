### Question
---
How would you calculate the “signal-to-noise ratio” for a standard ground-based telescope performing CCD imaging? What terms dominate at optical versus infrared wavelengths? Why, when observing objects that are fainter than physical foregrounds like the night sky, does SNR increase as sqrt(time)?

### Answer
---
##### How would you calculate the “signal-to-noise ratio” for a standard ground-based telescope performing CCD imaging?

In the photon counting regime, we can quantify the total number of photons observed ($N$) and the various contributions to noise in those counts, without making explicit any frequency dependence.

**Signal:**
- $N$ = number of photons from the source + sky background + anything else
- $N_{\rm s}$ = number of photons after we calibrate and quantify the other sources ($N_b, N_{\rm d}, N_{\rm r}$ below), and subtract their counts, leaving an estimate of the **total** source counts.

**Noise contributions:**
- $\sigma_{\rm s} = \sqrt{N_{\rm s}}$ = poisson noise from source 
- $\sigma_{\rm b} = \sqrt{N_{\rm b}}$ = poisson noise from background 
- $\sigma_{\rm d} = \sqrt{N_{\rm d}}$ = poisson noise from dark current (thermal noise in electrons, decreases if we lower temperature)
- $\sigma_{\rm r} = N_{\rm r}$ = [[Tools#Read noise|read noise]]

The total magnitude of the noise is then the following, assuming all the above are independent 

$$\sigma = \sqrt{\sigma_{\rm s}^{2} + \sigma_{\rm b}^{2} + \sigma_{\rm d}^{2} + \sigma_{\rm r}^{2}} = \sqrt{N_{\rm s} + N_{\rm b} + N_{\rm d} + N_{\rm r}^{2}}$$

Thus the signal to noise ratio (${\rm SNR}$) is:

$${\rm SNR} \equiv \frac{\rm{Signal}}{\rm{Noise}}= \frac{N_{\rm s}}{\sigma}$$

##### What terms dominate at optical versus infrared wavelengths? 

At [[Electromagnetic Spectrum|optical]] wavelengths, we are usually object-limited, meaning the dominant source of noise is the large number of source counts $\sigma \simeq \sqrt{N_s}$ . 
- Though the percentage error decreases with number of counts for poisson processes, the magnitude of the error itself still increases. 
- Since this is assumed independent of the other sources, it will eventually dominate.

At [[Electromagnetic Spectrum|IR]] wavelengths, the dark current is significant so $\sigma \simeq \sqrt{N_d}$ .
- Why? not sure, but may be due to thermal motion of particles within material of telescope itself, hence cooling of [[Instruments#JWST]] for example.

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

