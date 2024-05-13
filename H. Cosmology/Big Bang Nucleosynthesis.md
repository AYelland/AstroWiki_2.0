---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
  - BBN
---

## General Information

**Big Bang Nucleosynthesis** is the creation of the light elements and nuclei in the early universe approximately minutes after the Big Bang, after the formation and freeze-out of nucleons. *(see [[Question 145]] of the timeline of creation)*

**Characteristics of BBN:**
- The initial conditions ([[#The Neutron-Proton Ratio|neutron-proton ratio]]) were set at the neutron "freeze-out" within the first second after the Big Bang. This ratio is the key parameter determining the abundances of light elements after nucleosynthesis ends.
- The universe was very close to homogeneous at this time, and strongly radiation-dominated.
- The fusion of nuclei occurred between roughly 10 seconds to 20 minutes after the Big Bang; this corresponds to the temperature range when the universe was cool enough for deuteron to survive, but hot and dense enough for fusion reactions to occur at a significant rate

> [!note] "Freeze-Out"
> In general a "freeze out" is when the conditions (like temperature or density) change such that a certain particle/nuclear interaction becomes very unlikely to happen.

## The Neutron-Proton Ratio

After the nucleon ($n$, $p$) production from gluon/quark plasma ($\sim 1 \; {\rm s}$ of the Big Bang), neutrons can use [[Beta Decay|beta decay]] and [[Electron Capture|electron capture]] through positron/electron and electron neutrinos interactions to create protons and vise versa.

$$\begin{align}
\mathrm{n}+\mathrm{e}^{+} &\rightleftharpoons \bar{\nu}_{\mathrm{e}}+\mathrm{p} \\
\mathrm{n}+\nu_{\mathrm{e}} &\rightleftharpoons \mathrm{p}+\mathrm{e}^{-}
\end{align}$$

At times much earlier than 1 sec, these reactions were fast and maintained the $n/p$ ratio close to 1:1. As the temperature dropped, the equilibrium shifted in favor of protons due to their slightly lower mass. The $n/p$ ratio smoothly decreased. These reactions continued until the decreasing temperature and density caused the reactions to become too slow, which occurred at about $T = 0.8 \,\pu{MeV}$ (time around 1 second). This is called the "freeze out" temperature.

At freeze out, the neutron–proton ratio was about $1/5$. 

> [!derivation] 
> 
> We can estimate this ratio by the simplified [[Saha Equation]], as a function of $T$.
> 
> $$\frac{n_{\rm n}}{n_{\rm p}} \simeq \left(\frac{m_{\rm n}}{m_{\rm p}}\right)^{3/2} \exp \left[ -\frac{\left(m_{\rm n}-m_{\rm p}\right)c^{2}}{k_{\rm B} T} \right] \simeq \exp \left[-\frac{1.3\,\pu{MeV}}{0.8\,\pu{MeV}} \right] \simeq \frac{1}{5}$$
> 
> ...where we use the difference between the neutron and proton masses as $1.3\,\pu{MeV}$ (about 2.6 electron masses), and that the freeze-out temperature for this decay has been measured in the lab to be about $k_{\rm B} T\sim 0.8\,\pu{MeV}$. 
> 
> This ratio sets the amount of helium which can possibly be made during BBN.

However, free neutrons are unstable with a mean life of $\sim 890\,\pu{s}$; therefore, some neutrons decayed in the next few minutes before fusing into any nucleus. So, the ratio of total neutrons to protons after nucleosynthesis ends is about $0.15$ (see [[#Deuterium Bottleneck]] below).

## Deuterium Bottleneck

> [!note]- Deuteron vs Deuterium
> 
> In astrophysics and astronomy, these words are often found being used interchangeably; however, they are distinct. **Deuteron** is the *nuclei* of a **Deuterium** *atom*. Meaning, deuteron consist of a ($p + n$), whereas, deuterium consist of a ($p + n + e^{-}$).
> 
> Therefore, when we are talking about nuclear reactions where the temperatures are extremely high (such that the fusion reaction can occur), the electron is no longer bound to the nuclei, and we are talking about *deuteron* (a charged ion).

In hopes for nucleons to settle into energetically favorable helium configurations (more favorable than free neutrons that can [[Beta Decay#Beta-Minus Decay|beta-minus decay]], $\tau \sim 890 \; {\rm s}$), they must first undergo [[Deuteron Fusion|deuteron fusion]]. 

$$H + n \leftrightharpoons D + \gamma$$

At the time of neutron freeze-out, the temperature of the universe was already smaller than $2.22 \; {\rm MeV}$ (the binding energy of deuteron); therefore, we would think that deuterium production could take place.

However, because there are so many more photons than baryons, the high energy tail of photons energy spectrum increased the *mean energy per particle* enough to immediately destroy any deuterium that was created. Once the temperature (and the associated mean energy per particle) of the universe was $k_{\rm B} T \ll 2.22 \; {\rm MeV}$, then  could efficiently form deuteron.

This is the **Deuteron Bottleneck**, in which helium production is restricted in the early universe.

The fusion reactions are as follows, where deuteron is represented by $\ce{D} \equiv \ce{^{2}H}$...

$$\begin{align}
	\ce{p} + \ce{n} &\longrightarrow \ce{D} + \gamma \\
	\ce{p} + \ce{D} &\longrightarrow \ce{^{3}He} + \gamma \\
	\ce{D} + \ce{D} &\longrightarrow \ce{^{3}He} + \ce{n} \\
	\ce{D} + \ce{D} &\longrightarrow \ce{^{3}He} + \ce{p} \\
	\ce{^{3}He} + \ce{D} &\longrightarrow \ce{^{4}He} + \ce{n} \\
	\ce{^{3}He} + \ce{D} &\longrightarrow \ce{^{4}He} + \ce{p} \\
\end{align}$$

It takes universe $\sim 200 \; {\rm s}$ to finally became cool enough for [[Deuteron Fusion|deuteron fusion]] to efficiently take place, and then there was an immediate burst of nucleosynthesis as the new deuteron is immediately fused to create helium.

> [!derivation]- The Time Delay before Deuteron Fusion
> The time delay needed for the temperature to drop below $2.22\;{\rm MeV}$ causes neutrons to [[Beta Decay|beta decay]] before they can fuse to deuteron. *(Note, without the fusion to deuteron, all neutrons would be gone!)*
> 
> To calculate this time delay, we can use the [[Deuteron Fusion|deuteron fusion]] reaction ($\ce{p + n \leftrightharpoons D + \gamma}$) since it never freezes out, and only stops once all neutrons are used up. From the [[Saha Equation]]...
> 
> $$\frac{n_{\rm D}}{n_{\rm p} n_{\rm n}} = \frac{g_{\rm D}}{g_{\rm p} g_{\rm n}} \left(\frac{m_{\rm D}}{m_{\rm p} m_{\rm n}}\right)^{3/2} \left(\frac{k_{\rm B} T}{2 \pi \hbar^{2}}\right)^{-3/2} \exp \left[ \frac{2.22 \; {\rm MeV}}{k_{\rm B} T} \right]$$
> 
> ...where $g_{\rm p}=g_{\rm n}=2$ *(2 spin configurations)*, $g_{\rm D}=3$ *(3 spin configurations: $\uparrow\uparrow, \downarrow\downarrow, \uparrow\downarrow$)*, and $m_{\rm p}=m_{\rm n}=m_{\rm D}/2$. Simplifying...
> 
> $$\frac{n_{D}}{n_{p} n_{n}} = 6 \; \left(\frac{m_{n} k_{\rm B} T}{\pi \hbar^2}\right)^{-3/2} \exp \left[ \frac{2.22 \; {\rm MeV}}{k_{\rm B} T} \right]$$
> 
> The protons will always outnumber the neutrons, so let us define the time of [[Deuteron Fusion|deuteron fusion]] as the time when half the neutrons have fused into deuteron ($n_{\rm D}=n_{\rm n}$).
> 
> $$\frac{n_{D}}{n_{n}} = 1 = 6 \, n_{p} \, \left(\frac{m_{n} k_{\rm B} T}{\pi \hbar^{2}} \right)^{-3/2} \exp \left[ \frac{2.22 \; {\rm MeV}}{k_{\rm B} T} \right]$$
> 
> We now want to know when this happens. We can relate $n_{p}$ to the temperature to calculate the corresponding temperature and time. Additionally, we can relate $n_{p}$ to the baryon density ($n_{b}$) and photon density ($n_{\gamma}$) through the fixed [[Question 145|baryon-to-photon ratio]] ($\eta \simeq 5 \times 10^{-10}$) and the [[#The Neutron-Proton Ratio|neutron-proton ratio]] ($n_{\rm n}/n_{\rm p} \simeq 1/5$).
> 
> $$n_{\rm b} = n_{\rm p} + n_{\rm n} = \frac{6}{5} \, n_{\rm p} \hspace{1cm} \Rightarrow \hspace{1cm} n_{\rm p} = \frac{5}{6} \, \eta \, n_{\gamma} = \frac{5}{6} \, \eta \left( 0.24 \left(\frac{k_{\rm B} T}{\hbar c} \right)^{3} \right)$$
> 
> This yields a temperature and time delay of...
> 
> $$\begin{aligned}
> 	1 &= 6 \left( \frac{5}{6} \eta \cdot 0.24 \left(\frac{k_{\rm B} T}{\hbar c}\right)^{3} \right) \left(\frac{m_n kT}{\pi\hbar^2}\right)^{-3/2} \exp \left[ \frac{2.22 \; {\rm MeV}}{k_{\rm B} T} \right] \\
> 	\\
> 	1 &\approx 3.4\times10^{-9} \left(\frac{kT}{m_n c^2}\right)^{3/2} \exp \left[ \frac{2.22 \; {\rm MeV}}{k_{\rm B} T} \right]
> \end{aligned}$$
> $$T \approx 8 \times 10^{8} \; {\rm K} \hspace{1cm} \Rightarrow \hspace{1cm} t \approx 200 \; {\rm s}$$

During the duration of this time delay, we lose neutrons some quantity of neutrons through [[Beta Decay|beta decay]], with a lifetime of $\tau \sim 890 \; {\rm s}$. Therefore, after $t \sim 200 \; {\rm s}$ , our [[#The Neutron-Proton Ratio|neutron-proton ratio]] is actually closer to...

$$\frac{n_{\rm n}}{n_{\rm p}} \approx \frac{e^{-t/\tau}}{(n_{\rm p}/n_{\rm n}) + (1 - e^{-t/\tau})} \approx 0.15 \quad (< 0.2)$$

We can now make an estimate how much helium we expect to make in BBN relative to other elements (i.e. hydrogen) by analyzing our helium-to-baryon ratio ($Y$).

Using the [[#The Neutron-Proton Ratio|neutron-proton ratio]] that includes the neutron beta decay ($n_{\rm n}/n_{\rm p} \simeq 0.15$) yields a much closer estimate relative to our observational measurements.

$$Y = \frac{4 n_{\rm He}}{4 n_{\rm He} + n_{\rm H}} = \frac{2 n_{n}}{2 n_{n} + (n_{p}-n_{n})} = \frac{2 n_{n}}{n_{p}+n_{n}} = \frac{2 (n_{n}/n_{p})}{1 + (n_{n}/n_{p})} \approx 0.25$$

...where $n_{\rm He}=n_n/2$ (every $\ce{^{4}He}$ nucleus has $2n$) and $n_{\rm H}=n_p-n_n$ (a $\ce{^{4}He}$ nucleus has equal number of protons and neutrons).

Alternatively, we could do this calculation with the mass fraction. To make $\ce{^{4}He}$, we need 2 neutrons. If $n_{\rm n}/n_{\rm p} = 0.15$, then we can use a simple multiple of the ratio and consider 30 neutrons and 200 protons to make 15 heliums. Once all of the helium is formed, the mass fraction of the newly formed helium relative to total number of nucleons is...

$$f_{\rm He} \simeq \frac{15 \,m_{\rm He}}{200 \, m_{\rm p} + 30 \, m_{\rm n}} \simeq \frac{60}{230} \simeq 0.25$$

> [!note] Notes
> - Large $\Omega_b$ leads to larger $\eta$.
> 	- This means deuteron can form earlier and there is less neutron decay.
> 	- This leads to a larger $n_n/n_p$, such that $Y$ also increases with $\Omega_b$.
> - Measurements of $\ce{^{4}He}$ and $\ce{D}$ allow us to determine $\eta$ and $\Omega_b$.
> 	- Deuteron abundance is a sensitive measure for $\Omega_b$.
> 	- Found with the [[Lyman-Alpha Forest]] by relating line strength of $\ce{H}$ and $\ce{D}$.
