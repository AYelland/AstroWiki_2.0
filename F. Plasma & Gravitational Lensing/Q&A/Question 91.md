### Question
---
What is "Faraday rotation"? How is it used in astronomy?

### Answer
---
##### What is "Faraday rotation"?

> [!note]
> This is the first of two measurements one can make in different bands to infer information about the line-of-sight (the second is the [[Question 92|dispersion measure]]).

![[faraday_rotation.png|align:center|500]]

**Faraday rotation** occurs when light propagates in the presence of a magnetic field (aligned with the direction of propagation) and the polarization vector rotates. The angle of rotation ($\beta$) of the polarization vector depends linearly on propagation length in the magnetic field ($d$) and the strength of the magnetic field ($B$). 

$$\beta = \mathcal{V} B d \hWhere \mathcal{V} \equiv \mathcal{V}(\lambda) = \underbrace{\fpar{e}{2 m_{\rm e} c} \lambda \td{n}{\lambda}}_{\rm constant}$$

The proportionality constant (known as *Verdet Constant*) is dependent in the light's wavelength ($\lambda$) and change in the medium's refractive index ($n$) with respect to the wavelength. It is usually is measured empirically for a given medium.

*How does it work?*
- When an external magnetic field surrounds a medium, it can provide an overall torque on the captured atomic electrons, directly affecting their motion around their respective atomic nuclei. This provides a bias in the overall electron motion in the medium in the direction of the magnetic field.
- Additionally, as light propagates through the medium, it can cause the electrons to induce their own magnetic field (since they are moving charges) that can either add or subtract from the overall external magnetic field, based on the light's circular polarization.
- With the bias from the external magnetic field, this causes the left (counter-clockwise) and right (clockwise) circularly polarized light waves to propagate at slightly different speeds.
	- This property is known as "circular birefringence". 
- This effect accumulates into an overall phase shift in the polarization, induced by the Faraday effect, is to rotate the orientation of a wave's linear polarization.

*(Helpful Youtube Video: https://youtu.be/tueywXYpVsk?si=xszmA5hJSYDno_CQ)*

> [!note] Circular Polarization
> Similar to how linear polarization (i.e. $+$ or $\times$) can compose a basis when analyzing light propagation, we can define another basis called "circular polarization".
> 
> "Circular polarization" is decomposed into left (counter-clockwise) and right (clockwise) states, defined by the polarization vector rotating at a constant rate perpendicular to the direction of the wave.
> 
> ![[circular_polarization.gif|align:center]]
> 
> We can express the states as a superposition of two circularly polarized components of opposite handedness and different phase. Using bra-ket notation, one could imagine light wave would look like...
> $$
> \begin{alignat}{2}
> 	&\text{Linear Polarization: } &\hspace{1cm} \ket{\Phi} &= A \ket{\updownarrow} + B \ket{\leftrightarrow} \\
> 	&\text{Circular Polarization: } &\hspace{1cm} \ket{\Phi} &= C \ket{L_{\rm ccw}} + D \ket{R_{\rm cw}} \\
> \end{alignat}
> $$
> For un-polarized light, the components would have equal amplitudes/coefficients ($A=B, C=D$).

##### How is it used in astronomy?

We use Faraday rotation to measure the strength of magnetic fields between an emitting astronomical source and the observer, given we have knowledge about the electron number density along the path of propagation.

To do this, we use the **rotation measure** ($\mathcal{R}$) defined in SI units as...

$$
\mathcal{R} = \underbrace{\frac{e^{3}}{8 \pi^{2} \epsilon_{0} m_{\rm e}^{2} c^{4}}}_{\simeq \; 2.62 \times 10^{-13} \; {\rm \left[ T^{-1} \right]}} \int_{0}^{d} n_{\rm e}(z) B_{\parallel}(z) \; \rd z
\hWhere
\begin{aligned}
	z &\equiv \text{path of propagation} \\
	n_{\rm e}(z) &\equiv {\rm e^{-}\ number\ density\ at\ } z \\
	B_{\parallel}(z) &\equiv {\rm B\ field\ strength\ along\ } \hat{z}\\
\end{aligned}
$$

...which is related to the Faraday rotation angle ($\beta$) by the squared-wavelength.

$$\beta = \beta_{\rm 0} + \mathcal{R} \lambda^{2} \hRightarrow \Delta \beta = \mathcal{R} \lambda^{2}$$

Meaning, the longer the wavelength, the greater the Faraday effect is. That said, if we can measure $\Delta \beta$ at different wavelengths, we can disentangle the Faraday rotation from the intrinsic polarization angle ($\beta_{0}$). This gives us a proxy for the magnetic field strength ($B$).

To note, with a measurement of both the [[Question 92|dispersion measure]] and the rotation measure, we can further constrain the weighted mean of the magnetic field along the line-of-sight.

Because the Faraday effect it so prominent at longer wavelengths, it is commonly studied in radio astronomy ([[Fast Radio Burst|FRBs]] and [[Neutron Star#Pulsar|Pulsars]]).