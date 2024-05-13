### Question
---
Explain how a radio interferometer manages to produce sub-arcsecond images when none of the constituent dishes has an angular resolution of better than 1 arcmin.

### Answer
---
See [[Methods#Long baseline interferometry|LBI/VBLI]].

In [[Question 156]], we calculated the diffraction limitation for a given telescope.

$$\theta  = \frac{1.22  \, \lambda}{D} \hspace{1cm} \text{where} \hspace{1cm} \begin{aligned}
	\theta &\equiv \text{angular resolution (radian)} \\
	\lambda &\equiv \text{wavelength} \\
	D &\equiv \text{telescope diameter}
\end{aligned}$$

Since $\lambda$ is relatively large in the [[Electromagnetic Spectrum|radio]] band, we would need a huge dish diameter to get decent angular resolution. For an [[Units & Conversions#Arcsecond ($''$)|arcsecond]] angular resolution ($\theta = 1' \simeq 5 \times 10^{-6}\,\pu{rad}$) of radio wavelengths ($\lambda \gtrsim 1\,\pu{m}$), we would need a dish about $250\,\pu{km}$ across, which is entirely unfeasible.

$$5 \times 10^{-6} \; {\rm rad} = \frac{1.22 \times 1 \; {\rm m}}{D} \hspace{1cm} \Rightarrow \hspace{1cm} D \simeq 250 \; {\rm km}$$

Thus, we can use multiple dishes to get better resolution, but with much less collecting area than a telescope that large. This effectively constructs a large interferometer that can constructively interfere to produce an effective diameter equal to the length of the baseline (how far apart the dishes are). To do this, it requires careful clock-synchronization and precise timing at each telescope due to the time-delay between different paths going to different telescopes.

[[Instruments#EHT]] has a baseline of $\sim 1000\,\pu{km}$; such that at $\lambda \sim 1\,\pu{mm}$, they have an angular resolution of about $\theta \sim 25\,\pu{\mu as}$. With this, they were able to image the first two black holes: [[EHT-images.jpg|M87 and Sag A*]]