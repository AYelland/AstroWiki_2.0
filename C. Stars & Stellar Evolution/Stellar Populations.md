---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
---

> [!key-idea]
> The stellar populations are defined by a decreasing metal content (and the correlated increasing age theorized by [[_Stellar Nucleosynthesis]])
> - [[#Population III (Pop. III)]] - Original stars (very low metal content)
> - [[#Population II (Pop. II)]] - Old stars (low metallicity)
> - [[#Population I (Pop. I)]] - Youngest stars (high metallicity)

## Population I (Pop. I)

- Bluer stars
- Metal-rich *(i.e. young stars)*
- Often found in spiral arms of a galaxy (since these are star-forming regions)
- Usually maintain elliptical orbits about the galactic center
- Thought to have formed recently from enriched ISM
- Planets?
	- Theoretically: 
		- Pop. I stars are more likely have planetary systems, given planets are formed by the accretion metals
	- Observationally: 
		- [[Planetary Classes#Rocky Planets|Rocky Planets]] are concentrated about stars with a larger range of metallicities.
		- [[Planetary Classes#Gas Giants|Gas Giants]] are concentrated around stars with relatively higher metallicity.

**Examples:** [[Sun]], stars in spiral arms and disk (star-forming regions)

## Population II (Pop. II)

- Yellow Stars
- Metal-poor *(i.e. old stars, stars formed in an unenriched medium with few metals)*
- Typically found near the central galactic bulge, within globular star clusters, and in the Milky Way halo
- Potentially higher ratio of "alpha elements" (elements produced by the [[alpha process]]) compared to [[#Population I (Pop. I)|Pop I stars]], due to type II supernova contributions to the ISM at time of formation
- Orbits undergo random motion
- Thought to have formed from more pristine gas (i.e. hydrogen & helium based) before being enriched with metals from supernovae

**Examples:** stars near/in the [[Anatomy of a Galaxy#Galactic Bulge|Galactic Bulge]], a [[Stellar Clusters#Globular Cluster|Globular Cluster]], or the [[Anatomy of a Galaxy#Stellar Halo|Stellar Halo]] 

> [!bonus]-
> **What is the approximate maximum/minimum $\ce{[Fe/H]}$ [[Metallicity|metallicity]] that a Population II star can have?**
> $$
> \begin{align}
> \log_{10} \left({\frac {N_{\mathrm {Fe}}}{N_{\mathrm {H}}}}\right) = \log_{10} \varepsilon ({\rm Fe}) - \underbrace{\log_{10} \varepsilon ({\rm H})}_{= \ 12} \hspace{1cm} \text{where} \hspace{1cm} 
> \begin{aligned}
> 	&N_{\rm Fe} = \ce{Fe} \text{ atoms per unit of volume} \\
> 	&N_{\rm H} = \ce{H} \text{ atoms per unit of volume}
> \end{aligned}
> \end{align}
> $$
> Take the mass of a typical star forming cloud to be $10^{5} \, M_{\odot}$ and made of pure hydrogen gas (Bromm et al. 2013). (Recall: $M_{\odot} \simeq 2 \times 10^{30} \, {\rm kg}$ and $m_{\rm H} = m_{\rm p} \simeq 1.674 \times 10^{-27} \, {\rm kg}$)
> $$
> N_{\ce H} = \frac{M_{\rm gas}}{m_{\rm H}} = \frac{10^{5} \, M_{\odot}}{m_{\rm p}} = \frac{10^{5} \times (2 \times 10^{30} \, {\rm kg})}{1.674 \times 10^{-27} \, {\rm kg}} = 1.19 \times 10^{62} \, {\rm kg}
> $$
> Take the canonical supernova iron yield to be $0.1 \, M_{\odot}$, and then calculate the amount of iron ($\ce{Fe}$) produced by a single supernova event. ($m_{\rm Fe} \simeq 9.273 \times 10^{-26} \, {\rm kg}$)
> $$
> N_{\rm Fe} = \frac{M_{\rm yield}}{m_{\rm Fe}} = \frac{10^{-1} \, M_{\odot}}{m_{\rm Fe}} = \frac{10^{-1} \times (2 \times 10^{30} \, {\rm kg})}{9.273 \times 10^{-26} \, {\rm kg}} = 2.14 \times 10^{54} \, {\rm kg}
> $$
> Now, apply the values to the above [[Metallicity|metallicity]] equation to get the metallicity of the gas that a new star would form in...
> $$
> \log_{10} \varepsilon(\ce{Fe})_{*} = \log_{10} \left({\frac {N_{\mathrm {Fe}}}{N_{\mathrm {H}}}}\right)_{*} + \underbrace{\log_{10} \varepsilon ({\rm H})}_{= \ 12} = \log_{10} \left( \frac{2.14 \times 10^{54}}{1.19 \times 10^{62}} \right)_{*} + 12 = 4.26
> $$
> Converting to a [[Metallicity#^31901d|abundance ratio]] of $\ce{[Fe/H]}$, using the metallicity of the Sun as the standard to measure against (Asplund et al. 2009, $\log_{10} \varepsilon (\ce Fe)_{\odot} = 7.46$).
> $$\left[\ce{Fe}/\ce{H}\right] = {\log_{10} \varepsilon ({\rm Fe})}_{*} - {\log_{10} \varepsilon ({\rm Fe})}_{\odot} = (4.26) - (7.46) = -3.2$$
> And thus, the minimum abundance of a second generation star is $\left[\ce{Fe}/\ce{H}\right] \simeq -3.2$. 
> 
> In actuality, we do find stars that are more iron-poor than this, with the record being at $\left[\ce{Fe}/\ce{H}\right] \lesssim -7.3$. This is because the above calculation is a rough approximation with many assumptions that don't account for the high variety of nature (such as fragmentation of the gas cloud or alternative supernova mechanics). However, the majority of 2nd generation stars are found to have metallicities around this $\left[\ce{Fe}/\ce{H}\right] \simeq -3.2$ value.

## Population III (Pop. III)

- Theorized population of very first stars which formed when there were no metals at all ($z\simeq 20$)
- Extremely massive and luminous
- Not yet observed. Why?
	- Too hard to image a star at such a high redshift (best change is lucky highly-magnified star via [[Gravitational Lensing]])
	- Initial mass function for stars would have been high-mass skewed (why?) and thus most of these stars would have died by now.
	- Observable ones could also have been enriched by metals from their environment at this point.

**Examples:** nowhere ($z \gtrsim 20$)