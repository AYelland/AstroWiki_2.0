### Question
---
What is the meaning and purpose of a log N – log S curve? Explain the current interpretation of this curve for gamma-ray bursts.

### Answer
---
![[logN_logS.gif|align:center|450]]

The **log N – log S curve** is used to measure deviation of a population of sources from being homogeneous and isotropic in the universe (e.g. uniform on the sky and at all redshifts).

- $N \equiv$ number of [[Gamma Ray Burst|GRBs]]
- $S \equiv$ total energy released ("[[Fluence|fluence]]", the time-integrated [[Flux|flux]] often measured in total number of counts observed.)

For the [[Flux|flux]] ($F$) of a source with [[Luminosity|luminosity]] ($L$) at distance ($D$), the [[Fluence|fluence]] ($S$) is defined with the total energy output ($E$).

$$F = \frac{L}{4 \pi D^{2}} \hspace{1cm} \xRightarrow{\text{time integrate}} \hspace{1cm} S = \frac{E}{4\pi D^2}$$

For some minimum detectable [[Fluence|fluence]] ($S_{\rm min}$) for our instrument, the maximum distance at which we can observe an object of energy ($E$) is...

$$D_{\rm max} = \sqrt{\frac{E}{4 \pi S_{\rm min}}}$$

Meaning, we expect to be able to see sources in a volume of space (centered on us) of size...

$$V = \frac{4}{3} \pi D_{\rm max}^{3} \hspace{2cm} \underbrace{N(F) \; \mathrm{d} F = n \cdot \left( 4 \pi r^{2} \right) \cdot \mathrm{d} r}_{\text{\# of events with flux }\in\;[ F, F+\mathrm{d} F]}  \quad \propto D_{\rm max}^{3}$$

...such that if the spatial density of sources is uniform, we should see $N \propto D_{\rm max}^{3} \propto S_{\rm min}^{-3/2}$ events, (i.e. a line on a log-log plot of slope $-3/2$).

The fact we are seeing deviations at low energy (i.e. far away form us) implies we are seeing out to [[Redshift|redshifts]] at which [[Gamma Ray Burst|GRBs]] had not yet formed. This could be due to:
- Finite age of universe, not enough time for [[Stellar Explosions#Supernova|supernovae]], binary [[Neutron Star|NS]] mergers, etc.
- Evolving [[Gamma Ray Burst|GRB]] rate or intrinsic luminosity over cosmic time, perhaps scaling with star formation rate or metallicity