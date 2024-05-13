### Question
---
Explain quantitatively why stimulated emission is important and spontaneous emission is usually ignored in the radio domain, whereas the reverse is true in the optical domain. Given a thermal spectrum at some temperature T, at what frequency would the two emission rates be equal?

### Answer
---
##### Explain quantitatively why stimulated emission is important and spontaneous emission is usually ignored in the radio domain, whereas the reverse is true in the optical domain.

If we compare the two emission process rates at some given temperature of a [[Blackbody Radiation|blackbody]], we find the ratio of rates is highly dependent on the frequency of the incident light. Once the photon energy ($h\nu$) is much higher or lower than the thermal energy ($k_{\rm B}T$), the efficiency of one of the emission processes will fall off, yielding a dominant mechanism for that given temperature.

**More explicit calculations...**

Here, we compare the rates of [[Einstein Coefficents#Stimulated Emission|stimulated emission]] and [[Einstein Coefficents#Spontaneous Emission|spontaneous emission]].

$$R = \left[ \frac{\text{stimulated rate (per volume)}}{\text{spontaneous rate (per volume)}} \right]= \frac{B_{21} n_{2} J_{\nu}}{A_{21} n_{2}} = \left(\frac{B_{21}}{A_{21}}\right) J_{\nu} = \left(\frac{c^{2}}{2 h \nu^{3}}\right) J_{\nu}$$

If we assume the source emits like a [[Blackbody Radiation|blackbody]], this ratio reduces to ...

$$R = \left(\frac{c^{2}}{2 h \nu^{3}}\right) B_{\nu} = \left( e^{h \nu / k_{\rm B} T} - 1 \right)^{-1}$$

For [[Electromagnetic Spectrum|radio emission]] at a given temperature ($T$), we find that $R \gg 1$ such that [[Einstein Coefficents#Stimulated Emission|stimulated emission]] dominates the radio domain.

$$\frac{h \nu}{k_{\rm B} T} \ll 1 \hspace{1cm} \Rightarrow \hspace{1cm} R = \left( e^{h \nu / k_{\rm B} T} - 1 \right)^{-1} \approx \frac{k_{\rm B} T}{h \nu} \gg 1$$

For [[Electromagnetic Spectrum|optical emission]] at a given temperature ($T$), we find that $R \ll 1$ such that [[Einstein Coefficents#Spontaneous Emission|spontaneous emission]] dominates the optical domain.

$$\frac{h \nu}{k_{\rm B} T} \gg 1 \hspace{1cm} \Rightarrow \hspace{1cm} R = \left( e^{h \nu / k_{\rm B} T} - 1 \right)^{-1} \approx e^{-h \nu / k_{\rm B} T} \ll 1$$

##### Given a thermal spectrum at some temperature T, at what frequency would the two emission rates be equal?

The emission rates for these two processes will be equal when the incident photon energy is comparable to the thermal energy of the system ($h \nu \sim k_{\rm B} T$).

For equal emission rates, $R=1$.

$$R = 1 \hspace{1cm} \Rightarrow \hspace{1cm} 
\begin{aligned}[t]
	R = 1 &= \left( e^{h \nu / k_{\rm B} T} - 1 \right)^{-1} \\
	1 &=  \left( e^{h \nu / k_{\rm B} T} - 1 \right)\\
	h \nu &= k_{\rm B} T \ln(2)
\end{aligned}$$
$$\boxed{ \; \nu = \frac{k_{\rm B} T}{h}\ln(2) \quad \approx 1.44 \times 10^{10} \; {\rm [Hz/K]} \; \times \; T \; {\rm [K]}\; } \hspace{1cm} \Rightarrow \hspace{1cm} h \nu \sim k_{\rm B} T$$