---
banner: "![[galaxies.jpg]]"
banner_y: 0.35
aliases:
---
## Press-Schechter Theory

The **Press-Schechter theory** correlates the probability of a halo with a mass greater than a certain threshold mass ($M$) to the probability of the early universe having an overdensity greater than some critical density value ($\delta > \delta_{\rm crit}$). This directly connects the early universe fluctuations visible on the [[Cosmic Microwave Background|CMB]] to the [[#Press-Schechter Halo Mass Function|mass function]] of low [[Redshift|redshift]] galaxies.

![[press-schechter-theory.png]]

In the Press-Schechter (PS) formalism, we smooth the mass overdensity field by applying a [[Spherical Top Hat Model|spherical top-hat filter]]. Assuming the perturbations in this smoothed field follow a Gaussian distribution, this correlation is expressed by the equality:

$$P( \,> M) = P \left( \delta(M) > \delta_{\rm crit} \right)$$

Here, $\delta(M)$ represents the linearly extrapolated overdensity at the mass scale $M$, and $\delta_{\rm crit} \simeq 1.69$ is the [[Friedmann Equation#Critical Density|critical overdensity]] that determines collapse. 

This theoretical formalism effectively models the growth and collapse of small density fluctuations in the universe and connects them to the formation of structures through gravitational processes.

## Press-Schechter Halo Mass Function

The mass function describes the number of structures per unit volume with some mass in between $M$ and $M + \rd M$ at a given [[Redshift|redshift]].

If we consider a mass density fluctuation field ($\delta(x)$) throughout the universe, we can smooth it out and filter the field, omitting details on scales smaller than a characteristic length scale ($R$) by applying the [[Spherical Top Hat Model|spherical top-hat]] window function.

$$\delta_{M}(x) = \int \rd^{3} x' \; \delta(x') W_{R}(x - x') \hWhere W(x - x') = \begin{cases}
	1 &\text{for } |x - x'| < R \\
	0 &\text{otherwise}
\end{cases}$$

Given a uniform background density ($\rho_{0}$), set by the cosmological critical density $(\rho_{c})$ and the density parameters $(\Omega_{i})$, we can define a region of mass ($M$) within the characteristic radius ($R$) by:

$$M = \rho_{0} V = \left( \rho_{c} \Omega_{m} \right) \left( \frac{4 \pi R^{3}}{3} \right) \hWhere \rho_{c} \equiv \frac{3 H^{2}(z)}{8 \pi G}$$

If we assume that the mass density field has a Gaussian probability distribution, then the probability for some point in the field $(\delta_{M})$ to be greater than some critical density $(\delta_{c})$ is:

$$P(\delta_{M}) \; \rd \delta_{M} = \fpar{1}{\sqrt{2 \pi \sigma_{M}^{2}}} \exp \left[ - \frac{\delta_{M}^{2}}{2 \sigma_{M}^{2}} \right] \; \rd \delta_{M} \hRightarrow P_{> \delta_{c}}(M) = \int_{\delta_{c}}^{\infty} P(\delta_{M}) \; \rd \delta_{M}$$

where the variance on the mass probability distribution is related to the mass filter and the redshift. Below, $P_{m}(k,z)$ is the matter power spectrum and $\widetilde{W}_{R}^{2}(k)$ is the Fourier transform of the top hat filter function.

$$\sigma_{M}^{2} = \sigma_{R}^{2} = \frac{1}{2 \pi^{2}} \int_{0}^{\infty} \rd k \; k^{2} P_{M}(k, z) \widetilde{W}_{R}^{2}(k)$$

To then set up the expression for the mass function $N(M)$. We begin by taking the difference of the probabilities for the given mass range: $[ M, \; M + \rd M]$. This represents a total number distribution for the masses in this volume.

$$\begin{align}
    N(M) \rd M &= \left[ P_{>\delta_{c}}(M) - P_{>\delta_{c}}(M + \rd M) \right] \\
        &= \td{P_{>\delta_{c}}}{M} \; \rd M \\
        &= \td{P_{>\delta_{c}}}{\sigma_{M}} \;\td{\sigma_{M}}{M} \; \rd M \\
        & \nonumber \\
    &\left[ \begin{aligned}
        \td{P_{>\delta_{c}}}{\sigma_{M}} &= \td{}{\sigma_{M}} \left[ \int_{\delta_{c}}^{\infty} \fpar{1}{\sqrt{2 \pi \sigma_{M}^{2}}} \exp \left[ - \frac{\delta_{M}^{2}}{2 \sigma_{M}^{2}} \right] \; \rd \delta_{M} \right] \\
            &= \frac{1}{\sqrt{\pi}} \int_{x \sqrt{2} \sigma_{M}}^{\infty} e^{-x^{2}} \; \rd {x}
                \hspace{4cm} {\color{gray} \left( x = \frac{\delta_{M}}{\sqrt{2} \sigma_{M}} \right) } \\
            &= - \frac{1}{\sqrt{\pi}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \left( \td{}{\sigma_{M}} \fpar{\delta_{c}}{\sqrt{2} \sigma_{M}} \right) \\
            &= - \frac{1}{\sqrt{\pi}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \left( - \frac{\delta_{c}}{\sqrt{2} \sigma_{M}^{2}} \right) \\
            &= \fpar{\delta_{c}}{\sqrt{2 \pi} \sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right]
    \end{aligned} \right] \\
        & \nonumber \\
        &= \left( \fpar{\delta_{c}}{\sqrt{2 \pi} \sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \right) \; \td{\sigma_{M}}{M} \; \rd M  \\
        &= \frac{1}{\sqrt{2 \pi}} \; \fpar{\delta_{c}}{\sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \; \td{\sigma_{M}}{M} \; \rd M
\end{align}$$

By dividing the number distribution the mean volume $[ M / \rho_{0} ]$, this converts it to a comoving number density for halos of mass $M$.

$$n(M) \; \rd M = \frac{1}{\sqrt{2 \pi}} \; \fpar{\rho_{0} \delta_{c}}{M \sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \; \td{\sigma_{M}}{M} \; \rd M$$

If we a step further, we can assume the variance evolves linearly, and we can re-express it with a growth factor $(D(z))$: $\sigma_{M}(z) = \sigma_{M} D(z)$, where $\sigma_{M} \equiv \sigma_{R}$ for the Einstein-de Sitter model.

$$n(M) \rd M = \frac{1}{\sqrt{2 \pi}} \; \fpar{\rho_{0} \delta_{c}}{M D^{2} \sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 D^{2} \sigma_{M}^{2}} \right] \; \td{\sigma_{M}}{M} \; \rd M $$

$$n(M) \rd M = \frac{1}{\sqrt{2 \pi}} \; \fpar{\rho_{0} \delta_{c}}{M D^{2} \sigma_{R}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 D^{2} \sigma_{R}^{2}} \right] \; \td{\sigma_{R}}{M} \; \rd M$$

### Normalization

To normalize the mass function, we can integrate the volume fraction on the range $M \in [0, \; 1]$. *(Here, I have re-absorbed the growth factor $D$ back into the variance.)*

$$\begin{align}
    \mathcal{N} &= \int_{0}^{1} N(M) \; \rd M \\
        &= \int_{0}^{1} \frac{1}{\sqrt{2 \pi}} \; \fpar{\delta_{c}}{\sigma_{R}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{R}} \right] \; \td{\ln (\sigma_{R})}{M} \; \rd M \\
        &= \int_{0}^{1} \frac{1}{\sqrt{2 \pi}} \; \fpar{\delta_{c}}{\sigma_{R}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{R}^{2}} \right] \; \td{\sigma_{R}}{M} \; \rd M \\
        &= \frac{1}{\sqrt{2 \pi}} \; \int_{0}^{\infty} \fpar{\delta_{c}}{\sigma_{R}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{R}^{2}} \right] \; \rd \sigma_{R} 
            \hspace{1cm} {\color{gray} 
            \left[ \begin{aligned}
                x &= \frac{\delta_{c}}{\sqrt{2} \sigma_{R}} \\
                \rd x &= - \tfpar{\delta_{c}}{\sqrt{2} \sigma_{R}^{2}} \rd \sigma_{R} \\
                &\quad = - \tfpar{x^{2} \sqrt{2}}{\delta_{c}} \rd \sigma_{R}
            \end{aligned} \right]} \\
        &= \frac{1}{\sqrt{2 \pi}} \; \int_{\infty}^{0} \fpar{2 x^{2}}{\delta_{c}} \exp \left[ - x^{2} \right] \left( - \frac{\delta_{c}}{x^{2} \sqrt{2}} \right) \; \rd x \\
        &= \frac{1}{\sqrt{\pi}} \int_{0}^{\infty} \exp \left[ - x^{2} \right] \; \rd x \\
        &= \frac{1}{\sqrt{\pi}} \left[ \frac{\sqrt{\pi}}{2} \right] \\
        &= \frac{1}{2}
\end{align}$$

$$\boxed{\mathcal{N} = \int_{0}^{1} n(M) \; \rd M = \frac{1}{2} \ne 1}$$

As seen above, the Press-Schechter mass function is not normalized to $1$, but instead to $1/2$. This is where the necessity of the fudge factor comes from.

## Extended Press-Schechter Theory

The Extended Press-Schechter (EPS) formalism is very similar, but differs in a few very crucial ways.

Within the PS formalism, only $1/2$ of the mass in the universe is accounted for. To account for the other half of the mass, the EPS formalism incorporates for nonlinear and more complex cosmological scenarios (i.e. the cloud-in-cloud problem). These enhancements include:

- A time-varying critical overdensity ($\delta_{\rm crit}(z)$), allowing the collapse threshold change over cosmological time.
- A non-Gaussian density fluctuation distribution, that may be more accurate for the complexity of the cosmic density field.
- Nonlinear, stochastic contributions from that various effects that can occur during collapse. In other words, the evolution of the density field changes by a “random walk” versus a linear extrapolation in order to describe the unpredictability of small-scale perturbations.
- The mass accretion rate of collapsing objects (mass of a collapsing region is not a fixed quantity and changes as more mass accretes onto it).

The statement of probabilities in EPS formalism is then:

$$P (> M, z) = P (\delta(M, z) > \delta_{\rm crit}(z))$$

where $\delta(M, z)$ represents the linearly extrapolated overdensity at the mass scale $M$ and [[Redshift|redshift]] $z$, and the collapse threshold ($\delta_{\rm crit}(z)$) evolves with time. 

Recognition of these additional effects allows the EPS formalism to be more applicable to a broader range of cosmological scenarios, enhances its ability to describe/predict the evolution of cosmic structures, and gives justification to the fudge factor in the PS formalism.