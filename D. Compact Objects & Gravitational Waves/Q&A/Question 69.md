### Question
---
How would you go about estimating the number of binary systems in the galaxy that contain a black hole? What observational constraints do we have on this number?

### Answer
---
##### How would you go about estimating the number of binary systems in the galaxy that contain a black hole?

Any star that has a mass higher than $\sim 20\,M_\odot$ will become a [[Black Hole|black hole]] (see [[Question 40]]). So, we just need to work out:
1. *How many stars will be above this mass?*
2. *How many stars will be in binaries?*

Here are some common initial mass functions for stars:

![[initial_mass_functions.svg.png|align:center|400]]

1. To answer the first question, we will need to assume some probability distribution for the number of stars as a function of mass. That probability distribution function is defined as the **initial mass function (IMF)**. 
	
	We will use the "Salpeter IMF" with its Kroupa 2001 modification... $$\frac{\mathrm{d} N}{\mathrm{d} M} \propto M^{-2.3}$$...which holds for stars above $0.5 \; M_{\odot}$ . *(We won't consider objects below this mass since there are alternative powers on $M$ for lower masses.)*
	
	If we want to find the number of stars above a specific mass ($M_{*}$), we would simply integrate... $$N(M>M_{*}) \propto \int_{M_{*}}^{\infty} M^{-2.3} \; \mathrm{d} M$$
	Thus, the ratio of number stars above $0.5\,M_\odot$ to the number of stars above $20\,M_\odot$ is given by... $$f \equiv \frac{N_{20}}{N_{5}} = \frac{\int_{20 \, M_{\odot}}^{\infty} M^{-2.3} \; \mathrm{d} M}{\int_{0.5 \, M_{\odot}}^{\infty} M^{-2.3} \; \mathrm{d} M} \simeq 10^{-3}$$...where we "round down" to reflect the fact we aren't covering the whole distribution in mass.
	
	This is the statement that **about 1 in 1000 stars can become a [[Black Hole|black hole]].** Therefore, in the Milky Way where we have $\sim 10^{11}$ stars, about $10^{8}$ can become black holes.

3. To answer the second question, we make the naive assumption that $\sim 50 \%$ of all stars are in a [[Binary Stars|binary]]. That means we have **about $\sim 5 \times 10^{7}$ BH binaries in the Milky Way.** 

If we want to do better, need to do much more detailed stellar population synthesis and/or simulations, which get numbers close to $10^6-10^7$, meaning we probably overestimated but we are near the same order of magnitude.

##### What observational constraints do we have on this number?

Though we predict $\sim 10^{6} - 10^{7}$ [[Black Hole|black holes]] in the Milky Way, it is hard to observationally find this BH population.

**[[Binary Stars#X-Ray Binary]] Population:**
- $\mathcal{O}(100)$ observed in the Milky Way ($\sim 60$ confirmed, $\sim 40$ candidates)
	- Observed population is so low because we need to have relatively consistent x-ray emission to be able to see them.
	- Without accretion from the donor companion star, we can't get good x-ray measurements
- We have observed in [[Binary Stars#Low Mass X-Ray Binary (LMXB)|LMXB]] and [[Binary Stars#High Mass X-Ray Binary (HMXB)|HMXB]], but no sources for [[Binary Stars#Intermediate Mass X-Ray Binary (IMXB)|IMXB]]
	- Stellar winds are not strong enough for x-ray emission with intermediate mass companions
	- [[Binary Stars#Roche Lobe|RLOF]] proceeds very quickly in intermediate systems, making this phase rare to observe

**[[Instruments#LIGO]] Observations of Binary [[Black Hole|BH]] Mergers:**
- We can only detect binaries for which both objects are compact and they underwent a merging event.