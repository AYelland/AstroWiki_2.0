---
banner: "![[stars.png]]"
banner_y: 0.5
aliases:
  - metallicity
  - metallicities
---
**Metallicity** measures the abundance of the elements heavier than hydrogen and helium (such as carbon, oxygen, iron, …). In stellar astrophysics, metallicity usually refers to the abundance of iron and is defined as the iron-to-hydrogen ratio $\ce{[Fe/H]}$.

> [!note] "Metals" in Astronomy
> Astronomers use the term "metals" to refer to element that is not hydrogen or helium. *(See [[_Stellar Nucleosynthesis#Periodic Table]])*

This concept is very important when classifying stellar bodies by their age, and thus sorting them into [[Stellar Populations|stellar populations]]. This comes from the underlying assumption that old stars formed with the universe had very little metals (given they form from stellar fusion reactions) and young stars form in environments that are metal-rich.

Generally, we consider the iron content of the universe to linearly increasing in time because it has the highest [[Binding Energy#Nuclear Binding Energy|nuclear binding energy]]. Hence, it can be used as a chronological indicator of nucleosynthesis. Iron is relatively easy to measure with spectral observations due to the large number of lines in the spectra. 

**Absolute Abundance, $\log_{10} \varepsilon(\ce{A})$**

The absolute abundance represents the number of atoms (per unit of volume) of a specific element in a given star, relative to the abundance hydrogen. The hydrogen abundance value below is set to $12$ by definition.

$$\log_{10} \left({\frac {N_{\mathrm {A}}}{N_{\mathrm {H}}}}\right) = \log_{10} \varepsilon ({\rm A}) - \underbrace{\log_{10} \varepsilon ({\rm H})}_{= \ 12} \hspace{1cm} \text{where} \hspace{1cm}
\begin{align}
	&N_{\rm A} = \ce{A} \text{ atoms per unit of volume} \\
	&N_{\rm H} = \ce{H} \text{ atoms per unit of volume}
\end{align}$$

**Abundance Ratio, $\left[ \ce{A/B} \right]$** ^31901d

The abundance ratio is the ratio of two chemical abundances in a subject star, relative to the solar chemical abundance.

$$\left[\ce{A}/\ce{B}\right] = {\log_{10} \varepsilon ({\rm A})}_{*} - {\log_{10} \varepsilon ({\rm A})}_{\odot} = \log _{10}{\left({\frac {N_{\ce{A}}}{N_{\ce{B}}}}\right)_{\star}} - \log _{10}{\left({\frac{N_{\ce{A}}}{N_{\ce{B}}}}\right)_{\odot}} \hspace{1cm} \text{where} \hspace{1cm} \varepsilon(\ce{A}) = \frac{N_{\ce{A}}}{N_{\ce{B}}}$$

> [!example] For the iron-hydrogen ratio ($[\ce{Fe/H}]$) ...
> $$\left[\ce{Fe}/\ce{H}\right] = {\log_{10} \varepsilon ({\rm Fe})}_{*} - {\log_{10} \varepsilon ({\rm Fe})}_{\odot} \hspace{1cm} = \log _{10}{\left({\frac {N_{\ce{Fe}}}{N_{\ce{H}}}}\right)_{\star}} - \log _{10}{\left({\frac {N_{\ce{Fe}}}{N_{\ce{H}}}}\right)_{\odot}}$$
> 
> The solar metallicity of $\log_{10} \varepsilon (\ce{Fe})_{\odot} = 7.46 \pm 0.04$.
> - [Asplund et al. 2009](https://arxiv.org/pdf/0909.0948)
> - [Asplund et al. 2021](https://arxiv.org/pdf/2105.01661)

> [!example] For the magnesium-iron ratio ($[\ce{Mg/Fe}]$) ...
> $$
> \begin{align}
> \left[\ce{Mg}/\ce{Fe}\right] = \left[\ce{Mg}/\ce{H}\right] - \left[\ce{Fe}/\ce{H}\right] &= \left[ \log_{10} \varepsilon(\ce{Mg})_* - \log_{10} \varepsilon(\ce{Mg})_\odot \right] - \left[ \log_{10} \varepsilon(\ce{Fe})_* - \log_{10} \varepsilon(\ce{Fe})_\odot \right] \\
> &\\
> &= \left[ \log_{10} \left( \frac{N_\ce{Mg}}{N_\ce{H}} \right)_* - \log_{10} \left( \frac{N_\ce{Mg}}{N_\ce{H}} \right)_\odot \right] - \left[ \log_{10} \left( \frac{N_\ce{Fe}}{N_\ce{H}} \right)_* - \log_{10} \left( \frac{N_\ce{Fe}}{N_\ce{H}} \right)_\odot \right] \\
> &= \log_{10} \left( \frac{N_\ce{Mg}}{N_\ce{Fe}} \right)_* - \log_{10} \left( \frac{N_\ce{Mg}}{N_\ce{Fe}} \right)_\odot
> \end{align}
> $$
> 
> The solar metallicity of $\log_{10} \varepsilon (\ce{Fe}) = 7.46 \pm 0.04$ (*see https://arxiv.org/pdf/2105.01661*).

Therefore, stars with a higher metallicity than the Sun have a positive common logarithm, whereas those more dominated by hydrogen have a corresponding negative value. 

$$\left[ \frac{\rm Fe}{\rm H} \right]_{\star} \quad = \quad\begin{cases}
	& &\quad \dots \\
	+2 &\rightarrow \quad 10^{+2} &\text{times the metallicity of the Sun} \\
	+1 &\rightarrow \quad 10^{+1} &\text{times the metallicity of the Sun} \\
	~~~0 &\rightarrow \quad 10^{0} &\text{same metallicity as the Sun} \\
	-1 &\rightarrow \quad10^{-1} &\text{times the metallicity of the Sun} \\
	-2 &\rightarrow \quad10^{-2} &\text{times the metallicity of the Sun} \\
	& &\quad \dots \\
\end{cases}$$
 
> [!note] The unit often used for metallicity is the ${\rm dex}$ (contraction of "decimal exponent"). 

The complication with this system of measurements is that the Sun's metallicity is not set in stone. As time goes on, the solar metallicities increase, and the individual solar chemical abundance values have to be revised. Thus, when quoting a stellar abundance value, we must also reference what solar metallicity data we are using.

## Metallicity Classifications

In addition to the [[Spectral Classes|spectral classifications]] or the [[Stellar Populations|population classifications]], stars can be classified through their overall metallicity. With the assumption that the iron (Fe) metallicity directly correlates to a star's overall metallicity, then we can use it as a proxy for with generation the star belongs to. 

For example, the first stars ([[Stellar Populations#Population III (Pop. III)|Pop. III]] stars) would be considered the first generation. The stars formed from the remnants after the first generation dies would then be considered the second generation, and so on.... Gradually, the metallicity increases in each respective generation as nuclear fusion creates heavier and heavier elements.

| Description          | Definition           | Abbreviation |
| -------------------- | -------------------- | ------------ |
| Super-metal-rich     | $\ce{[Fe/H] > 0.0}$  | MR           |
| Solar                | $\ce{[Fe/H] = 0.0}$  | ---          |
| Metal-poor           | $\ce{[Fe/H] < -1.0}$ | NP           |
| Very-metal-poor      | $\ce{[Fe/H] < -2.0}$ | VMP          |
| Extremely-metal-poor | $\ce{[Fe/H] < -3.0}$ | EMP          |
| Ultra-metal-poor     | $\ce{[Fe/H] < -4.0}$ | UMP          |
| Hyper-metal-poor     | $\ce{[Fe/H] < -5.0}$ | HMP          |
| Mega-metal-poor      | $\ce{[Fe/H] < -6.0}$ | MMP          |
| Septa-metal-poor     | $\ce{[Fe/H] < -7.0}$ | SMP          |
| Octa-metal-poor      | $\ce{[Fe/H] < -8.0}$ | OMP          |

## Other Notes...

- [[Stellar Populations#Population III (Pop. III)|Pop. III stars]] are estimated to have metallicities close to $\ce{[Fe/H]} \lesssim -6$, a millionth of the abundance of iron in the Sun.
- [[Stellar Populations#Population II (Pop. II)|Pop. II stars]] have metallicities typically closer to $\ce{[Fe/H]} \sim (-3.0, -1.0)$ range.
- The metallicity of a star influences the mass and lifetime of the star, and the overall end state of how the star dies.