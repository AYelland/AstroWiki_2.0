### Question
---
From a physics perspective, how does the quantity (B-V) help to determine a star's effective (surface) temperature?

### Answer
---
By [[Blackbody Radiation#Wien's Displacement Law]], we know that the [[Flux|flux]]/[[Intensity|intensity]] emitted by blackbodies with higher temperature peak at smaller wavelengths. 

![[wiens_displacementLaw.png|aling:center|500]]

$$
B_{\nu}(\nu,T) = \frac{2 h \nu^{3}}{c^{2}} \left(\frac{1}{\exp \left[ \frac{h \nu}{k_{\rm B} T} \right] - 1}\right) \hspace{1cm} \Rightarrow \hspace{1cm} \lambda_{\rm peak} \simeq \frac{b}{T_{\rm eff}}
$$

By assuming the stellar surface emits as a [[Blackbody Radiation|blackbody]], we can measure the flux output of a star in the [[Photometry#UBVRI Filters|B and V bands]] , take their difference, and find the [[Hertzsprung-Russell Diagram#Color Index|color index (B-V)]]. 

$$
\begin{align}
	\lambda_{\rm short} - \lambda_{\rm long} \quad \equiv \quad m_{\rm short \lambda} &- m_{\rm long \lambda} = -2.5\log_{10} \left(\frac{F_{\rm short \lambda}}{F_{\rm long \lambda}}\right) \\
	&\Downarrow \\
	B-V \quad \equiv \quad m_{\rm B} &- m_{\rm V} = -2.5\log_{10} \left(\frac{F_{\rm B}}{F_{\rm V}}\right)
\end{align}
$$

![[wiens_stars.jpeg|align:center|500]]

This color index represents a crude estimate of the slope of the distribution between the two bands. This slope is inversely related to the effective temperature ($T_{\rm eff}$) of the star. 

- If $m_{\rm short \lambda} - m_{\rm long \lambda} < 0$ :
	- The shorter-wavelength filter is transmitting more light than the longer-wavelength filter, and we will see more of the shorter-wavelength radiation.
	- This correlates to seeing **hotter** and **bluer** stars.
- If $m_{\rm short \lambda} - m_{\rm long \lambda} = 0$ :
	- The filters transmit light equally.
- If $m_{\rm short \lambda} - m_{\rm long \lambda} > 0$ :
	- The longer-wavelength filter is transmitting more light than the shorter-wavelength filter, and we will see more of the longer-wavelength radiation.
	- This correlates to seeing **cooler** and **whiter** stars.




