---
banner: "![[particles.jpg]]"
banner_y: 0.55
aliases:
  - pp chain
---
The proton–proton chain is one of two known sets of nuclear fusion reactions that converts hydrogen to helium in stars. It dominates in stars with $M \lesssim 1.3 \, {\rm M_{\odot}}$

![[ppchain.png|align:center]]

$$
\textbf{The Net Reaction:} \hspace{1cm} 4 \, p + 2 \,e^{-} \longrightarrow \ce{^{4}He} + 2 \, \nu_{e} \hspace{1cm} \left( 26.4 \, {\rm MeV} \right)
$$

> [!key-idea] Important Notes
> - The *rate limiting reaction* is the proton fusion (p-p reaction) to form deuteron ($D$), due to being mediated by the weak nuclear force.
> - In all branches, the net energy released is the same: $E_{\rm gen} = 26.731 \; {\rm MeV}$. However, some of that energy escapes through neutrinos: $E_{\nu} \approx 0.262 \; {\rm MeV}$.
> 	- This is because the overall net reaction is the same (i.e. same initial reactants and final products) for all three branches. $$E_{\rm nuc} = \left(m_{\rm reactants} - m_{\rm products} \right) c^{2}$$
> - For the production of one $\ce{^{4}He}$ nuclei...
> 	- The [[#PP I]] branch requires **two*** *p-p reactions*
> 	- In the [[#PP II]]/[[#PP III]] branches requires **one** *p-p reactions*
> 
> - In the [[#PP II]]/[[#PP III]] branches, the initial $\ce{^{4}He}$ nuclei acts as a catalyst, allowing the $\ce{^{3}He} + p \longrightarrow \ce{^{4}He} + \nu_{e}$ net reaction to occur
> - If a significant $\ce{^{4}He}$ is present in the system, then all three branches will operate simultaneously.
> - Neutrinos from the [[#PP III]] branch (from the $\ce{^{8}B}$ decay) are emitted on the energy continuum up to $15 \; {\rm MeV}$ and are easily detectable. *(This is important for the [[Sun#Solar Neutrino Problem]])*
^important-notes

> [!sun] In the Sun...
> - In the [[Sun|Sun]], the [[#PP I]] branch dominates ([[#PP I]] : $\sim 69 \%$ , [[#PP II]] : $\sim 30.9 \%$ , [[#PP III]] : $\sim 0.1 \%$)
> - Reaction Timescales:
> 	- The average proton in the core of the Sun waits $\sim 10^{9} \; {\rm year}$ before it fuses with another proton.
> 	- Each newly created deuterium ($D$) nucleus exists for only $\sim 1 \, {\rm s}$ before it is converted into helium-3 ($\ce{^{3}He}$). 
> 	- The $\ce{^{3}He}$ isotope then only exists for $\sim 400 \, {\rm yr}$ before it is converted into helium-4 ($\ce{^{4}He}$).
> - $99\%$ of the energy output of the sun comes from the p–p chains, with the other $1\%$ coming from the [[Carbon-Nitrogen-Oxygen Cycle|CNO cycle]].
^in-the-sun
## Steps of Reaction

1) Two protons ($p$) fuse together to produce deuteron ($D$, stable). *(This is known as the p-p reaction)*
	- As the protons fuse, one of them undergoes [[Beta Decay#Beta-Plus Decay]], converting into a neutron by emitting a positron and an electron neutrino.
	- The positron will annihilate with an electron from the environment into two gamma rays. 
	- The energy produced in this reaction is emitted through the photons ($\sim 1.18 \; {\rm MeV}$) and the neutrino ($\sim 0.262 \; {\rm MeV}$).
	- This *p-p reaction* is the rate-limiting reaction for the p-p chain due to being mediated by the weak nuclear force (therefore, it is extremely slow)
	$$
	p + p \longrightarrow D + e^{+} + \nu_{e} 
	\hspace{1.5cm} 
	\textcolor{gray}{\left[ e^{+} + e^{-} \longrightarrow 2 \gamma \right]} 
	\hspace{1.5cm}
	\left( 1.442 \, {\rm MeV} \right) 
	$$
	
> [!atom] PEP Reaction
> This net reaction produces the same amount of energy as the rare *proton-electron-proton (p-e-p) reaction* (electron capture).
> $$p + e^{-} + p \longrightarrow D + \nu_{e} \hspace{1cm} \left( 1.442 \, {\rm MeV} \right)$$
> The frequency ratio of the *p-e-p reaction* vs. the *p–p reaction* is 1:400. However, the neutrinos released by the *p-e-p reaction* are far more energetic.
> - Neutrinos produced in the *p–p reaction* range in energy up to $0.42 \, {\rm MeV}$
> - Neutrinos produced in the *p-e-p reaction* creates sharp-energy-line neutrinos at $1.442 \, {\rm MeV}$


2) A deuteron ($D$) fuses with another proton to produce the helium-3 isotope ($\ce{^{3}He}$, stable) *(also see [[Deuteron Fusion]])*
	$$p + D \longrightarrow \ce{^{3}He} + \gamma$$
	This process is extremely faster than the proton fusion in step 1, due to being mediated by the strong nuclear force. 


3) For the production of helium-4 ($\ce{^{4}He}$), the fusion reaction chain splits into **three branches** ([[#PP I]], [[#PP II]], [[#PP III]])
	- In [[#PP I]], the production of $\ce{^{4}He}$ requires two *p-p reactions*
	- In [[#PP II]] and [[#PP III]], the production of $\ce{^{4}He}$ requires only one *p-p reaction*. 
		- The $\ce{^{4}He}$ nucleus is a catalyst, allowing the net reaction to occur 
			$$
			\ce{^{3}He} + p \longrightarrow \ce{^{4}He} + e^{+} + \nu_{e}
			\hspace{1.5cm} 
			\textcolor{gray}{\left[ e^{+} + e^{-} \longrightarrow 2 \gamma \right]}
			$$
	
	- If there is a significant $\ce{^{4}He}$ already present, then all branches will operate simultaneously.

### PP I

4) Using two $\ce{^{3}He}$ produced through the previous reactions, they can immediately form a $\ce{^{4}He}$ nuclei $$\ce{^{3}He} + \ce{^{3}He} \longrightarrow \ce{^{4}He} + 2 p$$
> [!note]
> This branch is dominant at temperatures $T \in \left[ 10 \, , \; 18 \right] \; \times 10^{6} \; {\rm K}$ .

### PP II

4) Using an already present $\ce{^{4}He}$ nuclei, a $\ce{^{3}He}$ nuclei and $\ce{^{4}He}$ nuclei will fuse with produce a $\ce{^{7}Be}$ nuclei. *(same reaction in both the [[#PP II]] and [[#PP III]] branches)*
	$$
	\ce{^{3}He} + \ce{^{4}He} \longrightarrow \ce{^{7}Be + \gamma}
	$$

5) The $\ce{^{7}Be}$ nuclei then uses [[Electron Capture]] to convert a proton ($p$) into a neutron ($n$) to generate a $\ce{^{7}Li}$ nuclei.
	$$
	\ce{^{7}Be} + e^{-} \longrightarrow \ce{^{7}Li + \nu_{e}}
	$$

6) The $\ce{^{7}Li}$ nuclei then uses a proton to generate initiate a quick [[Alpha Decay|alpha decay]] into two $\ce{^{4}He}$ nuclei. *($\ce{^{8}Be}$ has a half-life $\sim 10^{-17} \; {\rm s}$)*
	$$
	\ce{^{7}Li} + p \longrightarrow 2 \, \ce{^{4}He}
	$$

> [!note]
> This branch is dominant at temperatures $T \in \left[ 18 \, , \; 25 \right] \; \times 10^{6} \; {\rm K}$ .

### PP III

4) Using an already present $\ce{^{4}He}$ nuclei, a $\ce{^{3}He}$ nuclei and $\ce{^{4}He}$ nuclei will fuse with produce a $\ce{^{7}Be}$ nuclei. *(same reaction in both the [[#PP II]] and [[#PP III]] branches)*
	$$
	\ce{^{3}He} + \ce{^{4}He} \longrightarrow \ce{^{7}Be + \gamma}
	$$

5) The $\ce{^{7}Be}$ nuclei then uses [[Proton Capture]] to generate a $\ce{^{8}B}$ nuclei.
	$$
	\ce{^{7}Be} + p \longrightarrow \ce{^{8}B + \gamma}
	$$
	
6) The $\ce{^{8}B}$ isotope (being highly unstable) quickly [[Beta Decay#Beta-Plus Decay]] into a $\ce{^{8}Be}$ isotope.
	$$
	\ce{^{8}B} \longrightarrow \ce{^{8}Be} + e^{+} + \nu_{e}
	$$
	
7) With a half-life $\sim 10^{-17} \; {\rm s}$, the $\ce{^{8}Be}$ nuclei very quickly undergoes [[Alpha Decay]] to generate two $\ce{^{4}He}$ nuclei.
	$$
	\ce{^{8}Be} \longrightarrow 2 \, \ce{^{4}He}
	$$

> [!note]
> This branch is dominant at temperatures $T > 25 \times 10^{6} \; {\rm K}$ .

## Energy Generation Rate

Using the [[Nuclear Energy Generation Rate|energy generation rate (per volume)]]...

$$\epsilon_{\rm v} = \rho \, \epsilon_{m} = Q_{\rm nuc} \,  n_{A} \, n_{B} \, \sigma v \left( \frac{1}{1 + \delta_{AB}} \right) \quad \propto \quad Q_{\rm nuc} \,  n_{A} \, n_{B} \, S(E_{0}) \; T_{6}^{-2/3} \, e^{-B T_{6}^{-1/3}}$$
...where $T_{6} = 10^{6} \; {\rm K}$.

We can linearize the relationship around the dominate temperature for [[#PP I]] branch ($T_{6} \approx 15$) such that $\epsilon \propto T^{4}$.