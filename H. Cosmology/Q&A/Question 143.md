### Question
---
What are the "flatness problem" and the "isotropy problem" in standard Big-Bang cosmology? How does the inflationary model resolve these problems?

### Answer
---
##### Flatness Problem

The fact that the total $\Omega = \rho/\rho_c$ of the [[Friedmann Equation]] is remarkably close to 1 today ($\Omega \simeq 1.00\pm 0.01$). That is, it is very *flat*. 

Why is this a problem? If you look at the Friedmann equations, a deviation from flatness will be blown up as the universe expands. A flatness of $\Omega \simeq 1.00\pm 0.01$ today would require
- $\Omega \simeq 1.00\pm 0.00004$ at [[Cosmological Timeline#Recombination]]
- $\Omega \simeq 1.00\pm 10^{-12}$ at [[Big Bang Nucleosynthesis|nucleosynthesis]]

This implies an incredibly fine tuning of the universe at early times to be incredibly flat.

> [!derivation]
> 
> Start with the [[Friedmann equation]] and ignore $\Lambda$ (since in early universe it was negligible) (or define $\rho_{\rm c}$ with $\Lambda$ in it as in I do [[Friedmann Equation#Critical Density|here]]). We can then rearrange such that...
> 
> $$H^{2} = \frac{8 \pi G \rho}{3} - \frac{k c^{2}}{a^{2}} +\frac{\Lambda c^{2}}{3} \hspace{2cm} \left(\frac{3 H^{2}}{8 \pi G} - \rho(z)\right)a^{2} = -\frac{3 k c^{2}}{8 \pi G} = \text{const}$$
> 
> Using that $\Omega(z) = \rho(z) / \rho_{\rm c}(z)$ and the definition of the [[Friedmann Equation#Critical Density|critical density]], this can be written (using $\rho(z)\propto a^{-3}$) as...
> 
> $$\begin{align}
> \rho(z) \left( \frac{\rho_{c}(z)}{\rho(z)} - 1 \right) a^{2} &= \text{const} \hspace{1cm} \Rightarrow \hspace{1cm} 
> \Omega^{-1} - 1 \propto a
> \end{align}$$
> 
> Today ($a=1$), we observe a flat universe with $\Omega \simeq 1$. 
> 
> Given that density perturbation in the universe become more prominent as it expands and evolves, for $\Omega$ to be approximately $1$ today, then it must have also been extremely close to $1$ throughout the age of the universe. The problem is with this is that $a$ has changed by a factor of $10^{60}$ since the Planck era ($a(t_{\rm planck}) \sim 10^{-60}$), such that it would have to be *very* fine-tuned before the Big Bang.
> 
> There is no known reason for the density of the Universe to be so close to the critical density, and this appears to be an unacceptably strange coincidence in the view of most astronomers. Hence the flatness ‘problem’.

A proposed theory that solves this is [[Cosmological Timeline#Cosmic Inflation|inflation]], in which the universe rapidly expanded by a large factor in an extremely short period of time, such that locally, the universe looks very flat.

![[flatness_problem.jpeg|align:center|400]]

##### Isotropy Problem

The light horizon size at [[Cosmological Timeline#Recombination|recombination]] is only $\sim 2^\circ$ on the sky today, but its almost a perfect [[Blackbody radiation#Blackbody radiation|blackbody]].

The blackbody spectrum infers that the universe was in thermal equilibrium, and further suggests that this scale should be the size of the entire sky. When was it in causal contact in order to reach such a thermal equilibrium?

> [!derivation]
> To calculate the size of the light horizon, see the calculation for the [[Cosmic Microwave Background#Sound Horizon|sound horizon size]]. In that derivation, we assumed sound speed was proportional to the speed of light by $c_{\rm s} = c/\sqrt{3}$. Therefore, using the results, we can just multiply that answer of about $1^{\circ}$ by $\sqrt{3}$.
> $$l \sim \frac{\pi}{\theta} \hspace{1cm} \Rightarrow \hspace{1cm} \theta \sim \theta_{\rm s} \sqrt{3} \sim \left(\frac{\pi}{l_{\rm s}}\right) \sqrt{3} \sim 2 \degree$$

Inflation solves this by whole universe being in causal contact close to Big Bang.

![[isotropy_problem.png|align:center|600]]

