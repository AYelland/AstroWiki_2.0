### Question
---
In our Universe, at roughly what scale does perturbation theory break down and become non- perturbative?

### Answer
---
Linear structure growth (see [[Question 132]]) breaks down when overdensities become large ($\delta \gg 1$) and decouple from the [[Hubble#Hubble Law|Hubble flow]]. Structure in the universe forms hierarchically because there is more power on smaller scales, such that they go non-linear first. 


***At what length scale does this transition occur for a given redshift?*** 

From the [[Spherical Top Hat Model|spherical top-hat model]] at [[Spherical Top Hat Model#At turnaround...|turnaround]], we found the overdensity parameter of a perturbation to be...

$$\delta = \xi - 1 \hRightarrow \xi_{\rm ta} \equiv \frac{\rho_{\rm max}}{\bar{\rho}} = \frac{\rho_{\rm max}}{\rho_{\rm crit}(z)} = \fpar{r_{\rm crit}}{r_{\rm max}}^{3} = \fpar{3 \pi}{4}^{2} \simeq 5$$

...where $\rho_{\rm max} \equiv \rho(t_{max})$, $r_{\rm max} \equiv r(t_{max})$ and $t_{\rm max}$ is the time at which the overdensity decouples from the Hubble flow.

Thus, the transition to non-linearity occurs at approximately...

$$\rho \simeq 5 \bar{\rho} = 5 \bar{\rho_{0}} (1+z)^{3} = \fpar{15 \Omega_{M} H_{0}^{2}}{8 \pi G}(1+z)^{3}$$

We can convert this to a (mass-dependent) radius via $\rho = 3M/4\pi r^3$ and end up with a nonlinear scale that gives something like 10s of $\pu{Mpc}$. 

$$r_{\rm{nonlinear}} \lesssim \left(\frac{M}{10^{12}\,M_{\odot}}\right)^{1/3} \left(\frac{1}{1+z}\right) \,\pu{Mpc}$$

Basically, all of this means that the largest systems (like galaxies and [[Galaxy Cluster|galaxy clusters]]) will go through this non-perturbative phase in which they virialize.

*(Source: https://ned.ipac.caltech.edu/level5/March06/Padmanabhan/Nabhan3.html)*