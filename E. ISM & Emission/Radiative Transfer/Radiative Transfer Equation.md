---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
  - RTE
  - radiative transfer equation
---
*(Helpful Resource: https://www.cv.nrao.edu/~sransom/web/Ch2.html)*

When light interacts with matter, one of two things can happen:

1) Light is created/emitted
2) Light is absorbed/scattered/removed

With this in mind, we can compose the **Radiative Transfer Equation (RTE)** from the change in the [[Intensity#Specific Intensity|specific intensity]] over the path the light traveled ($\mathrm{d} z$).
$$\frac{\mathrm{d} I_{\nu}}{\mathrm{d} z} = j_{\nu} - \alpha_{\nu} I_{\nu}$$
Here, $\alpha_{\nu}$ is the absorption coefficient and $j_{\nu}$ is the spontaneous emission coefficient where...
$$
\left[ j_{\nu} \right] \equiv \frac{\text{specific intensity}}{\text{length}}
\hspace{2cm}
\left[ \alpha_{\nu} \right] \equiv \frac{1}{\text{length}}
$$

> [!note]
> Having $\alpha_{\nu} \propto \frac{\mathrm{d} I_{\nu}}{\mathrm{d} z}$ is not always exact; however, it tends to be a pretty good estimate. Additionally, one could introduce an additional term for "simulated emission" that would also be proportional to the change in intensity, but its not necessary in more cases.

---
**NOT FINISHED:**

If we solve the RTE, then we can define the **source function** ($S_{\nu}$).

$$
\begin{align}
	\frac{\mathrm{d} I_{\nu}}{\mathrm{d} z} &= j_{\nu} - \alpha_{\nu} I_{\nu} \\
	\frac{1}{\alpha_{\nu}} \frac{\mathrm{d} I_{\nu}}{\mathrm{d} z} &= \frac{j_{\nu}}{\alpha_{\nu}} - I_{\nu} \\
	\frac{\mathrm{d} I_{\nu}}{\mathrm{d} \tau_{\nu}} &= S_{\nu} - I_{\nu} \hspace{1cm} \text{where} \hspace{1cm} \boxed{S_{\nu} \equiv \frac{j_{\nu}}{\alpha_{\nu}}} \\
	\frac{\mathrm{d} I_{\nu}}{\mathrm{d} \tau_{\nu}} e^{\tau_{\nu}} &= S_{\nu} e^{\tau_{\nu}} - I_{\nu} e^{\tau_{\nu}} \\
	\frac{\mathrm{d} }{\mathrm{d} \tau_{\nu}} \underbrace{\left( I_{\nu} e^{\tau_{\nu}} \right)}_{x} &= \underbrace{S_{\nu} e^{\tau_{\nu}}}_{y} \\
	x(\tau_{\nu}) - x(0) &= \int_{0}^{\tau_{\nu}} y(\tau_{\nu}') \; \mathrm{d} \tau_{\nu}' \\
		x(\tau_{\nu}) - x(0) &= \int_{0}^{\tau_{\nu}} y(\tau_{\nu}') \; \mathrm{d} \tau_{\nu}' \\
\end{align}
$$

With this definition, we can use the value of $\tau_{\nu}(z)$ to determine the visibility through the space in between a source and the observer.

- If $\tau_{\nu} \gg 1$: the medium is opaque *(optically thick)* $$I_{\nu} = S_{\nu} = B_{\nu(T)}$$
- If $\tau_{\nu} \ll 1$: the medium is transparent *(optically thin)* $$I_{\nu} = B_{\nu}(T) + \underbrace{\tau_{\nu} (S_{\nu} - B_{\nu}(T))}_{= 0 \; (S_{\nu} = B_{\nu}(T))} = B_{\nu}(T)$$
- If $\tau_{\nu} \simeq 1$: we can see intensity behaviors
