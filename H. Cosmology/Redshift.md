---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - redshift
  - redshifted
  - z-shifted
---
## Sources of Redshift/Blueshift

There are 3 sources of redshift/blueshift: 
- [[#Relativistic Doppler Effect]] - from the relative motion between the source and observer
- [[#Gravitational Redshift]] - due to light exiting a gravitational field
- [[#Cosmological Expansion]] - where space itself stretches

## Redshift

Redshift ($z$) is defined by the difference in observed wavelength and emitted wavelength of light:
$$
z \equiv \frac{\lambda_{\rm obs} - \lambda_{\rm em}}{\lambda_{\rm em}} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\lambda_{\rm obs}}{\lambda_{\rm em}} = 1 + \frac{\lambda_{\rm obs} - \lambda_{\rm em}}{\lambda_{\rm em}} = 1 + z
$$

## Relativistic Doppler Effect

The **relativistic Doppler effect** is the change in frequency, wavelength and amplitude of light, caused by the relative motion of the source and the observer (as in the classical Doppler effect), when taking into account effects described by the special theory of relativity.

$$
\boxed{1 + z = \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \sqrt{\frac{1 + \beta}{1 - \beta}} = \left( 1 + \beta \right) \gamma} \hspace{1cm} \text{where} \hspace{1cm}
\beta \equiv \frac{v}{c} \quad , \quad \gamma = \frac{1}{\sqrt{1 - \beta^{2}}}
$$

The relativistic Doppler effect is different from the non-relativistic Doppler effect as the equations include the time dilation effect of special relativity and do not involve the medium of propagation as a reference point. They describe the total difference in observed frequencies and possess the required Lorentz symmetry.

![[z_dopplerEffect.png|align:center|400]]

> [!note]
> This expression for redshift also implies that at first order correction...
> 
> $$
> \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \frac{f_{\rm emt}}{f_{\rm obs}} = 1 + \beta + \mathcal{O}(\beta^{2})
> \hspace{1cm} \Rightarrow \hspace{1cm}
> \begin{align}
> 	\Delta \lambda &= \lambda_{\rm obs} - \lambda_{\rm emt} = \beta \lambda_{\rm emt} \\
> 	\Delta f &= f_{\rm obs} - f_{\rm emt} = - \beta f_{\rm emt} \\
> \end{align}
> $$
> 
> ...meaning if the observer and source are getting closer together ($v>0$) we have that the frequency increases, and that the frequency decreases for moving away.

> [!derivation]
> Consider the problem in the reference frame of the source. Suppose one wavefront arrives at the receiver. The next wavefront is then at a distance...
> 
> $$\lambda_{\rm s} = \frac{c}{f_{\rm s}}
> \hspace{1cm} \text{where} \hspace{1cm} 
> \begin{aligned} 
> 	\lambda_{\rm s} &= \lambda_{\rm emt} \equiv \text{emission wavelength at source} \\
> 	f_{\rm s} &= \lambda_{\rm emt} \equiv \text{emission frequency at source}
> \end{aligned}
> $$
> 
> The wavefront moves at the speed of light ($c$), but at the same time, the receiver is moving at their own speed ($v$). We can connect the distance traveled by the the period of time it takes for wavefronts to reach the observer from the source (from the frame of the source) ($t_{\rm r,s}$).
> 
> $$
> \lambda_{\rm s}+ v \, t_{\rm r,s} = c \, t_{\rm r,s}
> \hspace{1cm} \Rightarrow \hspace{1cm}
> t_{\rm r,s} = \frac{\lambda_{\rm s}}{c \left( 1 - \frac{v}{c} \right)} = \frac{1}{f_{\rm s} ( 1 - \beta)}
> \hspace{1cm} \text{where} \hspace{1cm}
> \beta \equiv \frac{v}{c}
> $$ 
>
> Connecting the frequency of the emitted light to the observed light, we can find a ratio that correlates to the wavelength ratio. However, unlike the normal Doppler effect, we have to take into account relativistic effects where the clocks on the receiver are time dilated relative to clocks at the source: 
> 
> $$f_{\rm s} = \frac{1}{t_{\rm r,s} (1 - \beta)} = \frac{f_{\rm r,s}}{(1 - \beta)}$$
> 
> $$t_{\rm r} = \frac{t_{\rm r,s}}{\gamma} \hspace{1cm} \Rightarrow \hspace{1cm} f_{\rm r} = \gamma \; f_{\rm r,s} = \left(\frac{1}{\sqrt{1 - \beta^{2}}}\right) \left(1 + \beta \right) f_{\rm s} = \sqrt{\frac{1 + \beta}{1 - \beta}} \; f_{\rm s}$$
> 
> $$\frac{f_{\rm r}}{f_{\rm s}} = \frac{\lambda_{\rm s}}{\lambda_{\rm r}} = \quad \boxed{\frac{\lambda_{\rm emt}}{\lambda_{\rm obs}} = \sqrt{\frac{1 + \beta}{1 - \beta}} = 1 + z }$$

## Gravitational Redshift

The **gravitational redshift** (*or Einstein Shift*) originates from time dilation occurring in a gravitational well. As photons have to climb out of a deep potential, they lose energy and become redshifted. The following formula is for a gravitational field of an uncharged, non-rotating, spherically symmetric mass.

$$
\boxed{1 + z = \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \left( 1 - \frac{r_{\rm S}}{R_{\rm emt}} \right)^{-1/2}}
\hspace{1cm} \text{where} \hspace{1cm}
r_{\rm S} = \frac{2 G M}{c^{2}} \equiv \text{Schwarzschild Radius}
$$

This expression tells us that as as redshift increases, so does the observed radius of the source. Therefore, neutrons stars and black holes appear to be bigger than their true physical size.

> [!derivation]
> The derivation of this effect follows from the [[General Relativity#Schwarzschild Metric|Schwarzschild solution]] of the Einstein equations. 
> 
> Let us consider a spherically symmetric mass $M$ with some size $R$ to be non-rotating ($\mathrm{d} \theta = \mathrm{d} \varphi = 0$) and uncharged. We will only consider the photons emitted radially from the surface of our mass while our observer is at rest relative to the mass ($\mathrm{d} r = 0$).
> 
> For an object at a particular radius $r$, the spacing of clock ticks in proper time are determined by... *(abusing notation a little)*
> 
> $$\mathrm{d} \tau^{2} = \left( 1 - \frac{r_{\rm S}}{r} \right) \mathrm{d} t^{2} \hspace{1cm} \Rightarrow \hspace{1cm} \left. \frac{\mathrm{d} \tau}{\mathrm{d} t} \right|_{r} = \sqrt{1 - \frac{r_{\rm S}}{r}}$$
> 
> We will define the gravitational redshift between an observer at the surface ($r=R$) and an observer at $r = \infty$, such that they are outside of the well.
> 
> $$1 + z = \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \frac{\lambda_{\infty}}{\lambda_{\rm R}}$$
> 
> If we now compare the proper time observed by a timelike observer at both $r=R$ and $r=\infty$ in one unit of coordinate time (i.e. $\mathrm{d} \tau / \mathrm{d} t$), we can compare their wavelengths.
> 
> $$\lambda \sim \frac{1}{\nu} \sim \text{observers in proper time }\tau \hspace{1cm} \Rightarrow \hspace{1cm} \lambda = \frac{\mathrm{d} \tau}{\mathrm{d} t}$$
> $$1 + z = \frac{\lambda_{\infty}}{\lambda_{\rm R}} = \frac{\mathrm{d} \tau / \mathrm{d} t |_{\infty}}{\mathrm{d} \tau / \mathrm{d} t |_{R}} = \sqrt{\frac{1 - (r_{\rm S} / r_{\infty})}{1 - (r_{\rm S} / r_{\rm R})}} = \left( 1 - \frac{r_{\rm S}}{R} \right)^{-1/2} = \left( 1 - \frac{2 G M}{R c^{2}} \right)^{-1/2}$$
> 
> $$\boxed{1 + z = \frac{\lambda_{\rm obs}}{\lambda_{\rm emt}} = \left( 1 - \frac{r_{\rm S}}{R} \right)^{-1/2}} \hspace{1cm} \text{where} \hspace{1cm} r_{\rm S} = \frac{2 G M}{c^{2}} \equiv \text{Schwarzschild Radius}$$


## Cosmological Expansion

The **cosmological redshift** comes from stretching of the wavelengths of photons as they propagate through the expanding space.

$$
\boxed{1+z = \frac{\lambda_{\rm obs}}{\lambda_{\rm em}} = \frac{a_{\rm obs}}{a_{\rm em}}} \hspace{1cm} \text{where} \hspace{1cm} c \; \mathrm{d} t = a(t) \; \mathrm{d} \chi
$$

For observing today, we have $a_{0} = 1$, such that...

$$
\frac{a_{\rm obs}}{a_{\rm emt}} = \frac{a_{0}}{a} = \frac{1}{a} = 1+z \hspace{1cm} \Rightarrow \hspace{1cm} a = \frac{1}{1+z}
$$

> [!derivation]
> Let our photon travel from the source at $(t_{\rm em}, a_{\rm em}, z_{\rm em})$ to the observer at $(t_{\rm obs}, a_{\rm obs}, z_{\rm obs})$.
> 
> ![[z_cosmology_derivation.png|align:center|400]]
> 
> The spatial hyper-surface can shrink or expand depending on $a(t)$, so $\lambda_{\rm obs}$ is not necessarily equal to $\lambda_{\rm em}$. Photons always travel along the shortest path, so for light we have:
> $$\mathrm{d} s = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \mathrm{d} x = c \; \mathrm{d} t = a(t) \; \mathrm{d} \chi$$
> $$
> \begin{aligned}
> 	{\rm Pulse\ A}: \int_{\chi_{\rm em}}^{\chi_{\rm obs}} \mathrm{d} \chi &= \int_{t_{\rm em}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)} \\
> 	\\
> 	{\rm Pulse\ B}: \int_{\chi_{\rm em}}^{\chi_{\rm obs}} \mathrm{d} \chi &= \int_{t_{\rm em}+\delta t_{\rm em}}^{t_{\rm obs}+\delta t_{\rm obs}} \frac{c \mathrm{d} t}{a(t)} = \int_{t_{\rm em}}^{t_{\rm obs}}... + \int_{t_{\rm obs}}^{t_{\rm obs} \delta_{t_{\rm obs}}}...-\int_{t_{\rm em}}^{t_{\rm em} + \delta_{t_{\rm em}}} \\
>     &\approx \int_{t_{\rm em}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)} + \left( \frac{c \; \delta t_{\rm obs}}{a(t_{\rm obs})} - \frac{c \; \delta t_{\rm em}}{a(t_{\rm em})} \right)
> \end{aligned}
> $$
>   
>  Bringing the two back together...
>  $$\underbrace{\int_{t_{\rm em}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)}}_{\rm Pulse\ A} = \underbrace{\int_{t_{\rm em}}^{t_{\rm obs}} \frac{c \; \mathrm{d} t}{a(t)} + \left( \frac{c \; \delta t_{\rm obs}}{a(t_{\rm obs})} - \frac{c \; \delta t_{\rm em}}{a(t_{\rm em})} \right)}_{\rm Pulse\ B}$$
>  $$\frac{c \; \delta t_{\rm obs}}{a(t_{\rm obs})} = \frac{c \; \delta t_{\rm em}}{a(t_{\rm em})} \hspace{1cm} \Rightarrow \hspace{1cm} \frac{c \; \delta t_{\rm obs}}{c \; \delta t_{\rm em}} = \frac{\lambda_{\rm obs}}{\lambda_{\rm em}} = \frac{a_{\rm obs}}{a_{\rm em}}$$
>  $$\boxed{1+z = \frac{\lambda_{\rm obs}}{\lambda_{\rm em}} = \frac{a_{\rm obs}}{a_{\rm em}}}$$


> [!note] The Effect on the Luminosity
> The change of [[luminosity]] $L=\frac{\rm energy\ of\ photons}{\rm time}$ is affected "twice" by expansion since
> 
> $$
> \frac{\lambda_{\rm obs}}{\lambda_{\rm em}} = \frac{c \, \delta t_{\rm obs}}{c \, \delta t_{\rm em}} = \frac{a_{\rm obs}}{a_{\rm em}} \hspace{1cm} \Rightarrow \hspace{1cm} L_{\rm obs} = \frac{h f_{\rm obs}}{\delta t_{\rm obs}} = \frac{h f_{\rm em}}{\delta t_{\rm em}} \left(\frac{a_{\rm em}}{a_{\rm obs}}\right)^{2} = L_{\rm em}\left(\frac{a_{\rm em}}{a_{\rm obs}}\right)^{2}
> $$
> 
> If $a_{\rm obs}=1, z_{\rm obs} = 0$ and $a_{\rm em} = a, z_{\rm em} = z$, then we have
> 
> $$
> L_{\rm obs} = L_{\rm em} \left(\frac{1}{1+z}\right)^{2} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{L_{\rm obs} = \frac{L_{\rm em}}{(1+z)^{2}}}
> $$
