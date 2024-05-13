### Question
---
What is a neutron star? What assumptions and inputs go into determining the upper mass limit for a neutron star? What is the approximate ratio of neutrons to protons (and electrons) in the interior of a neutron star?

### Answer
---
##### What is a neutron star?

See [[Neutron Star|Neutron Stars]].

##### What assumptions and inputs go into determining the upper mass limit for a neutron star? 

![[Tolman–Oppenheimer–Volkoff Limit]]

##### What is the approximate ratio of neutrons to protons (and electrons) in the interior of a neutron star?

Though there are many addition factors that need to be accounted (i.e. density and equation of state), we can approximate the nucleon ratio ($\bar{n}_{\rm n}/\bar{n}_{\rm p}$) as a function of temperature ($T$).

The composition of the interior will dictated by the [[Beta Decay#Beta-Minus Decay]] and [[Electron Capture]] rates.

$$
\begin{alignat}{4}
	&\beta^{\ -} \text{ Decay:} &\hspace{2cm} n &\longrightarrow p + e^{-} + \bar{\nu}_{e} \\
	&e^{-} \text{ Capture:} &\hspace{2cm} p + e^{-} &\longrightarrow n + \nu_{e}
\end{alignat}
$$

Assuming that the number densities of the neutrons and protons ($\bar{n}_{\rm n}$ , $\bar{n}_{\rm p}$) can be roughly represented by the [[Statistical Mechanics#Maxwell-Boltzmann]] distribution, we can use a ratio of their Boltzmann factors.

$$\bar{n}_{\rm s} = g_{\rm s} \left(\frac{m_{\rm s} k_{\rm B} T}{2 \pi \hbar^{2}}\right)^{3/2} \exp \left( - \frac{m_{\rm s} c^{2}}{k_{\rm B} T} \right) \hspace{1cm} \text{where} \hspace{1cm} s \equiv \text{particle species}$$
$$\frac{\bar{n}_{\rm n}}{\bar{n}_{\rm p}} \sim \exp \left( - \frac{(m_{\rm n} - (m_{\rm p} + m_{\rm e})) c^{2}}{k_{\rm B} T} \right) \sim \exp \left( - \frac{ 0.8 \; {\rm MeV}}{k_{\rm B} T} \right) \sim \exp \left( - \frac{10^{10} \; [{\rm K}]}{T}\right)$$

From this, we see that at temperatures $\sim 10^{10} \; {\rm K}$, we have $e \sim 3$ times more protons than neutrons; however, the ratio maximizes at a 8:1?

The final ratio should be $(\bar{n}_{\rm n}:\bar{n}_{\rm p}:\bar{n}_{\rm e} \longrightarrow 8:1:1)$ .

> [!cian] Comment from Cian
> Really, this argument is flawed, and it should include [[Degeneracy Pressure|Fermi levels]] such as that for the $e+p$ state: $(m_p + m_e)c^2 - E_F(T)$. With this, as we increase the density, the electron Fermi level rises until it is no longer energetically favorable to make an electron.
> 
> *(Somewhat better argument using the Fermi momenta/energies as in [this stackexchange post](https://astronomy.stackexchange.com/questions/45420/does-the-average-proton-electron-density-in-a-neutron-star-change-with-mass#:~:text=The%20ratio%20of%20neutrons%20to,the%20density%20becomes%20very%20large).)*

Another Source: http://windhorst322.asu.edu/notes/ryden_ch9_notes.pdf