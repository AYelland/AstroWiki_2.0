---
aliases: Schechter Luminosity Function
---
### Question
---
What is the "Schechter luminosity function"? What is the luminosity of a typical bright galaxy? How does the luminosity function of galaxies compare to the mass function of halos from simulations?

### Answer
---
##### What is the "Schechter luminosity function"?

The **Schechter luminosity function** is the empirical relationship that describes the observed galaxy [[Luminosity|luminosity]] function (i.e. the distribution of number of galaxies with different luminosities). 

$$\Phi(L) = \frac{\Phi_{*}}{L_{*}} \left( \frac{L}{L_{*}} \right)^{\alpha} e^{-L/L_{*}} \hWhere 
\begin{aligned}
	\Phi_{*} &\simeq 0.02 \, h^{3} \; {\rm Mpc^{-3}} \\
	\alpha &\simeq -1.09 \\
	L_{*} &\simeq 10^{10} \; L_{\odot} \, h^{-2} \sim \text{MW luminosity}
\end{aligned}$$

...where $\Phi(L)$ has dimensions "galaxies per volume per luminosity", such that $\Phi(L) \, \rd L$ is the number of galaxies with luminosity between $L$ and $L+dL$ per unit volume.
-  $\Phi_{*} \equiv$ normalization factor
- $\alpha \equiv$  faint-end slope 
- $L_{*} \equiv$ characteristic $L$ at normalization point

The function has the following shape (from Megan's notes):

![[schechter_luminosity_function.png|align:center|400]]


##### What is the luminosity of a typical bright galaxy?

A typical galaxy has a luminosity similar to the [[Galaxies - General#The Milky Way|Milky Way]] ($L_{*} \sim L_{\rm MW} \sim 2 \times 10^{10} L_{\odot}$ ). 
- We don't see many galaxies far above this luminosity because they are associated with more rare, massive galaxies. 
- We don't see many far below because they're very faint.

##### How does the luminosity function of galaxies compare to the mass function of halos from simulations?

In simulations, we adjust the AGN feedback and the baryonic physics models in order to align our expectations with observations. This is because the luminosity of a galaxy directly stems from the galactic star formation, and the internal feedback mechanisms drives the gas out of smaller potentials, disrupting the star formation process.

- Smaller galaxies struggle to form stars due to [[Stellar Explosions#Supernova|SNe]] feedback.
- Larger galaxies struggle grow larger (and form more stars) due to the [[Active Galactic Nuclei|AGN]] feedback

![[schechter_luminosity_function_comparison.png|align:center]]
