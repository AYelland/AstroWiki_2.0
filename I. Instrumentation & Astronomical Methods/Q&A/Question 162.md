### Question
---
Derive the approximate (within a factor of a few) spectral resolution R required to detect a planet that perturbs its host star by a radial velocity amplitude of 10 cm/s. Describe some practical challenges with calibration and stability, and how they are addressed for such instruments. Why have we not yet achieved this precision in RV measurements of real stars?

### Answer
---
##### Derive the approximate (within a factor of a few) spectral resolution R required to detect a planet that perturbs its host star by a radial velocity amplitude of 10 cm/s.

> [!note] Defining Spectral Resolution
> 
> The **spectral resolution** of a spectrograph (or frequency spectrum more generally), is a measure of its ability to resolve features and distinguish between lines in the electromagnetic spectrum.. It is usually denoted by $\Delta \lambda$, and is closely related to the **resolving power** ($R$) of the spectrograph, defined as...
> 
> $$R = \frac{\lambda}{\Delta\lambda}$$
> 
> ...where $\Delta \lambda$ is the smallest difference in wavelengths that can be distinguished at a wavelength of $\lambda$. 
> 
> The spectral resolution can also be expressed in terms of physical quantities, such as velocity. Then, the resolution describes the difference between velocities $\Delta v$ that can be distinguished through the [[Redshift#Relativistic Doppler Effect|Doppler shifts]], such that the resolving power is...
> 
> $$R = \frac{\lambda}{\beta\lambda} = \frac{1}{\beta}= \frac{c}{\Delta v}$$

For a radial velocity measurement of $\Delta v \sim 10\,\pu{cm s^{-1}}$ (see [[Question 9]] to understand order of magnitude), we would need a resolving power of...

$$R \simeq \frac{c}{0.1 \; {\rm m/s}} \simeq 3 \times 10^{9}$$

This is much higher that the best that exists today ([[Instruments#HARPS]] has  $R \sim 10^{5}$ with  $\Delta v \sim 1 \; {\rm m/s}$,  [[Instruments#VLT]] with $\Delta v \sim 0.3 \; {\rm m/s}$)

**How can we achieve such a precision then?**

The resolution is the ability to distinguish between lines. This is *not* the same as measuring the central position of a line, which is needed to compare to the rest frame value to get a radial velocity. 

If we measure multiple lines rather than just one, we can measure shifts below the spectral resolution of the instrument. In general, if we have an observable $X$ and we can measure it to be $\mu_X$ with uncertainty for a single observation $\sigma_X$, then our uncertainty on the value of $\mu_X$ can be reduced by repeating observations (for a Gaussian process if we made the observation a billion times, we would get a beautiful Gaussian of well-measured width $\sigma_X$ and a very certain mean value $\mu_X$). The scaling on the uncertainty of the mean $\sigma_{\mu,X}$ for repeating the observation $N$ times is  

$$\sigma_{\mu,X} = \frac{\sigma_X}{\sqrt{N}}$$

In the case at hand, we want to measure the position of the center of a line $\mu$ which we do with some uncertainty $\sigma$ set by the spectral resolution, and if we measure several lines we can improve sensitivity roughly via the same math as above (since we are in principle measuring different things each time, but to get the same number) to get 

$$\sigma_\mu = \frac{\sigma}{\sqrt{N}}$$

where $N$ is the number of lines. 

> [!derivation] In terms of velocities...
> 
> We can define our uncertainty of central position of our spectral lines through the distribution of the data points.
> 
> $$\sigma_{v} \approx \frac{{\rm FWHM}}{{\rm SNR}} \hspace{1cm} \text{where} \hspace{1cm} {\rm SNR} \sim \sqrt{N} \text{ for photon noise}$$
> 
> For a single spectral line:
> 
> $$\sigma_{v} \approx \frac{\Delta v}{{\rm SNR}} = \frac{c}{R \cdot {\rm SNR}}$$
> 
> For a $n$ spectral line, we apply the reduction of $\sqrt{N}$.
> 
> $$\sigma_{v} \approx  \frac{c}{R \cdot {\rm SNR} \cdot \sqrt{N}}$$
> 
> Therefore, for a radial velocity measurement of $R \sim 3 \times 10^{9}$ for $N \sim 1000$ spectral lines to achieve the $\Delta v \sim 10 \; {\rm cm/s}$ precision...
> $$R \cdot {\rm SNR} \cdot \sqrt{N} \sim 3 \times 10^{9} \hspace{1cm} \Rightarrow \hspace{1cm} R \cdot {\rm SNR} \sim 10^{8} \hspace{1cm} \Rightarrow \hspace{1cm} SNR \sim 10^{3}$$
> ...we would need a signal-noise-ratio of about 1000 using today's technology (with $R\sim 10^{5}$).

##### Describe some practical challenges with calibration and stability, and how they are addressed for such instruments. Why have we not yet achieved this precision in RV measurements of real stars?

**Challenges:**
- We are looking at tiny changes in detector pixels $\implies$ the instrument has to be extremely stable. 
	- Vacuum to prevent pressure fluctuations
	- cooled to prevent thermal fluctuations
	- no moving parts ideally
	- continual calibration via known sources
- Sources also vary in that they are spinning and have intrinsic variability in their atmospheres etc, which is really hard to subtract from signal. 
- Has been proposed to observe in minima of solar cycles of stars strategically to minimize this effect.

Sources:
- https://www.youtube.com/watch?v=DmNwPTY47SA (start at 26 min)
- http://spiff.rit.edu/classes/resceu/lectures/radial_vel/radial_vel.html
