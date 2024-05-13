### Question
---
What is the physical significance of the plasma frequency?

### Answer
---
The **plasma frequency** ($\omega_{\rm p}$) is a parameter of how fast plasma waves propagate, but even more so, it is the most fundamental time-scale in plasma physics. It sets the timescale for charges in a plasma to relax. 

To identify the effects of light trying to propagate through a plasma, we can compare the plasma frequency to the frequency of the light ($\omega$). *(This is motivated by the dispersion relationship and the group velocity derived in [[Question 92]].)*

$$
\textcolor{gray}{ \left[ \; 
\text{Dispersion Relation:} \hspace{1cm} \omega^{2} = \omega_{\rm p}^{2} + c^{2} k^{2}
\hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}
	\omega &\equiv \text{wave ang. frequency} \\
	\omega_{\rm p} &\equiv \text{plasma ang. frequency} \\
	k &\equiv \text{wave number}
\end{aligned}
\; \right]}
$$

$$v_{\rm g} = c \; \sqrt{1 - \left(\frac{\omega_{\rm p}}{\omega}\right)^{2}} \quad \simeq \begin{cases}
	\; c &\quad {\rm for} \quad \omega_{\rm p} \gg \omega \\
	\; c \sqrt{1 - (\omega_{\rm p}/\omega)^{2}} &\quad {\rm for} \quad \omega_{\rm p} \gt \omega \\
	\; \text{imaginary} &\quad {\rm for} \quad \omega_{\rm p} \lt \omega \\
\end{cases}$$

- For $\omega \gg \omega_{\rm p}$ , the plasma has little effect on the light and it passes unattenuated.
- For $\omega \gt \omega_{\rm p}$ , the plasma introduces a time delay on the propagating light. 
- For $\omega \lt \omega_{\rm p}$ , the plasma has enough time to react and the light wave will be dampened and reflected through oscillations in the plasma.

There is a different plasma frequency for each particle species. However, the relatively fast electron frequency is the most important, and references to "the plasma frequency'' typically mean the electron plasma frequency.

$$\omega_{\rm p} = \sqrt{\frac{n_{\rm e} e^{2}}{\epsilon_{0} m_{\rm e}}} \hspace{1cm} \text{(SI units)} \hspace{2cm} \textcolor{gray}{\left[ \;\omega_{\rm p} = \sqrt{\frac{4 \pi \, n_{\rm e} e^{2}}{m_{\rm e}}} \hspace{1cm} \text{(CGS units)} \right]}$$

> [!derivation]
> 
> The electron plasma frequency can be derived from *Maxwell's Equations*, or by considering the restoring force of a displaced charge species in a plasma. I show the latter. *([Source](https://farside.ph.utexas.edu/teaching/plasma/lectures1/node6.html))*
> 
> Let us imagine a box (with equal-area sides) consisting of particle species with positive and negative charges ($\pm q$), each with an equal number density ($n$). If we then displace one particle species in the box by some distance $\delta x$ in the $\hat{x}$-direction, then we will create a charge imbalance forcing one side of the box have a net negative charge and the other side an equal and opposite net positive charge...
> 
> $$Q = \left(\frac{\text{charge}}{\text{particle}}\right) \times \left(\frac{\text{particles}}{\text{volume}}\right) \times \text{volume} = q\,n\, (A\delta x)$$
> 
> ...and thus, each has a surface charge density of...
> 
> $$\sigma = \frac{Q}{A} = q \, n \, \delta x$$
> 
> This effectively is the classic "two charged parallel plates" of electromagnetism, of which has an electric field strength ($E$) in between the two sides.
> 
> $$E = -\frac{\sigma}{\epsilon_0}$$
> 
> Applying [[Newton's Laws of Motion#Newton's 2nd Law]] to a test particle in the box, we can define the *plasma frequency* ($\omega_{\rm p}$).
> 
> $$m \frac{\mathrm{d}^{2} (\delta x)}{\mathrm{d} t^{2}} = q E = - m \left(\frac{q^{2} n}{\epsilon_{0} m}\right) \, \delta x = - m \, \omega_{\rm p}^{2} \, \delta x \hspace{1cm} \Rightarrow \hspace{1cm} \omega_{\rm p} \equiv \sqrt{\frac{q^{2} n}{\epsilon_{0} m}}$$
> 
> This is just a simple harmonic oscillation for the displacement of charges from quasi-neutrality at a frequency ($\omega_{\rm p}$). We can thus think of this frequency as the (inverse) timescale over which charges in a perturbed quasi-neutral plasma return themselves to quasi-neutrality.


> [!note] Usage on Earth
> 
> We use the fact that EM waves cannot penetrate a plasma if they are below the plasma frequency to send radio signals around the Earth. They are bounced off of the bottom of the atmosphere, and received after the reflection. Higher frequencies than radio can pass straight through.
