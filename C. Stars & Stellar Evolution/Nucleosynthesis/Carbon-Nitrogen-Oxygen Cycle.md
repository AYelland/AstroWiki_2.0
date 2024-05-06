---
banner: "![[particles.jpg]]"
banner_y: 0.55
aliases:
  - CNO cycle
---
The carbon-nitrogen-oxygen is one of two known sets of nuclear fusion reactions that converts hydrogen to helium in stars. Similar to the [[Proton-Proton Chain]], it effectively converts four protons into one helium-4 nuclei, but it uses $\ce{C}$, $\ce{N}$, $\ce{O}$, and $\ce{F}$ in a catalytic manner to do so.

> [!key-idea] Important Notes
> - The *rate limiting reaction* in the [[#CNO-I]] cycle is the $\ce{^{14}N}$ nuclei undergoing [[Proton Capture|proton capture]] to produce $\ce{^{15} O}$. $$\ce{^{14}N} + p \longrightarrow \ce{^{15}O} + \gamma$$
> - Similar to the [[Proton-Proton Chain|pp chain]], the net energy released is the same, ($E_{\rm gen} \sim 26 \; {\rm MeV}$), and some of that energy escapes through neutrinos. However, unlike the [[Proton-Proton Chain|pp chain]], the CNO cycle is catalytic such that it doesn't consume *all* of its constinuents.
> -  In stars a bit larger than the sun ($M \gtrsim 1.3 \; {\rm M_{\odot}}$) - and therefore hotter - the CNO cycle is dominant over the [[Proton-Proton Chain|pp chain]].
> - Cold vs. Hot CNO 
> 	- Dependent on [[Proton Capture|proton capture]] rate vs [[Beta Decay#Beta-Plus Decay|beta-plus decay]] rate (i.e. hotter allows heavier element formation since proton capture rate is faster than beta-plus decay rate)
> 	- Inside of stars, there are 4 [[#Cold CNO Cycles]] ([[#CNO-I]], [[Carbon-Nitrogen-Oxygen Cycle#CNO-II]], [[#CNO-III]], [[#CNO-IV]]) that can occur. The [[#CNO-III]] and [[#CNO-IV]] cycles are reserved for heavier stars.
> 	- Outside of stars, where the temperature and pressure are high enough, there are 3 [[#Hot CNO Cycles]] ([[#HCNO-I]], [[#HCNO-II]], [[#HCNO-III]]) that produce helium-4 through a different reaction chain.
> 	- HCNO Sites: [[Stellar Explosions#Supernova|supernovae]] and [[Binary Stars#X-Ray Binary|XRBs]]
^important-notes

> [!sun] In the Sun...
> About $\sim 1 \%$ of the energy produced in the sun is through the CNO cycle, almost entirely from [[#CNO-I]]. The other $99 \%$ comes from the [[Proton-Proton Chain|pp chain]].
> 
> *Note: [[#CNO-III]] and [[#CNO-IV]] only occur in more massive stars and in supernovae.*
^in-the-sun


## Cold CNO Cycles

![[CNOcycle_cold.png]]

With normal stellar conditions, the catalytic hydrogen burning is restricted by the timescales necessary for nuclear fusion through [[Proton Capture|proton captures]] with respect to [[Beta Decay#Beta-Plus Decay]]. Due to the lower temperature and pressure, the cold CNO cycles work on timescales long enough (many years) that the slow [[Proton Capture|proton capture]] processes can occur.

### CNO-I

$$\ce{^{12}C} \; \rightarrow \; \ce{^{13}N} \; \rightarrow \; \ce{^{13}C} \; \rightarrow \; \ce{^{14}N} \; \rightarrow \; \ce{^{15}O} \; \rightarrow \; \ce{^{15}N} \; \rightarrow \; \ce{^{12}C}$$
This is the main cycle of the larger CNO cycle. Using a present $\ce{^{12}C}$ nuclei, it can catalytically generate $\ce{^{4}He}$ nuclei through the following reactions.

$$
\begin{alignat}{2}
	\ce{^{12}C} + p &\longrightarrow \ce{^{13}N} + \gamma &\quad + 1.95 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{13}N} &\longrightarrow \ce{^{13}C} + e^{+} + \nu_{e} &\quad + 1.20 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 9.965 \; {\rm min}$)} \\
	\ce{^{13}C} + p &\longrightarrow \ce{^{14}N} + \gamma &\quad + 7.54 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{14}N} + p &\longrightarrow \ce{^{15}O} + \gamma &\quad + 7.35 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{15}O} &\longrightarrow \ce{^{15}N} + e^{+} + \nu_{e} &\quad + 1.73 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 122.24 \; {\rm s}$)} \\
	\ce{^{15}N} + p &\longrightarrow \ce{^{12}C} + \alpha &\quad + 4.96 \; {\rm MeV}\hspace{1cm} &\text{($p-\alpha$ reaction)} \\
\end{alignat}
$$

### CNO-II

$$\ce{^{15}N} \; \rightarrow \; \ce{^{16}O} \; \rightarrow \; \ce{^{17}F} \; \rightarrow \; \ce{^{17}O} \; \rightarrow \; \ce{^{14}N} \; \rightarrow \; \ce{^{15}O} \; \rightarrow \; \ce{^{15}N}$$
This is a minor branch CNO cycle, where $\ce{^{4}He}$ is produced through the following reactions. In this branch, it does utilize fluorine as an intermediate product in the reaction chain, but it does not accumulate in the star.

$$
\begin{alignat}{2}
	\ce{^{15}N} + p &\longrightarrow \ce{^{16}O} + \gamma &\quad + 12.13 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{16}O} + p &\longrightarrow \ce{^{17}F} + \gamma &\quad + 0.60 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{17}F} &\longrightarrow \ce{^{17}O} + e^{+} + \nu_{e} &\quad + 2.76 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay)} \\
	\ce{^{17}O} + p &\longrightarrow \ce{^{14}N} + \alpha &\quad + 1.19 \; {\rm MeV} \hspace{1cm} &\text{($p-\alpha$ reaction)} \\
	\ce{^{14}N} + p &\longrightarrow \ce{^{15}O} + \gamma &\quad + 7.35 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{15}O} &\longrightarrow \ce{^{15}N} + e^{+} + \nu_{e} &\quad + 2.75 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay)} \\

\end{alignat}
$$

### CNO-III

$$\ce{^{17}O} \; \rightarrow \; \ce{^{18}F} \; \rightarrow \; \ce{^{18}F} \; \rightarrow \; \ce{^{15}N} \; \rightarrow \; \ce{^{16}O} \; \rightarrow \; \ce{^{17}F} \; \rightarrow \; \ce{^{17}O}$$
This is a subdominant branch only significant for massive stars. This chain of reactions begins when the $\ce{^{17}O}$ produces a $\ce{^{18}F}$ nuclei (and a photon) instead of the $\ce{^{14}N}$ nuclei (and alpha particle) in the [[#CNO-II]] branch. $\ce{^{4}He}$ is then generated through the following reactions.

$$
\begin{alignat}{2}
	\ce{^{17}O} + p &\longrightarrow \ce{^{18}F} + \gamma &\quad + 5.61 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{18}F} &\longrightarrow \ce{^{18}O} + e^{+} + \nu_{e} &\quad + 1.66 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 109.771 \; {\rm min}$)} \\
	\ce{^{18}O} + p &\longrightarrow \ce{^{15}N} + \alpha &\quad + 3.98 \; {\rm MeV}\hspace{1cm} &\text{($p-\alpha$ decay)} \\
	\ce{^{15}N} + p &\longrightarrow \ce{^{16}O} + \gamma &\quad + 12.13 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{16}O} + p &\longrightarrow \ce{^{17}F} + \gamma &\quad + 0.60 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{17}F} &\longrightarrow \ce{^{17}O} + e^{+} + \nu_{e} &\quad + 2.76 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 64.49 \; {\rm s}$)}
\end{alignat}
$$

### CNO-IV

$$\ce{^{18}O} \; \rightarrow \; \ce{^{19}F} \; \rightarrow \; \ce{^{16}O} \; \rightarrow \; \ce{^{17}F} \; \rightarrow \; \ce{^{17}O} \; \rightarrow \; \ce{^{18}F} \; \rightarrow \; \ce{^{18}O}$$
This is a subdominant branch only significant for massive stars. This chain of reactions begins when the $\ce{^{18}O}$ produces a $\ce{^{19}F}$ nuclei (and a photon) instead of the $\ce{^{15}N}$ nuclei (and alpha particle) in the [[#CNO-III]] branch. $\ce{^{4}He}$ is then generated through the following reactions.

$$
\begin{alignat}{2}
	\ce{^{18}O} + p &\longrightarrow \ce{^{19}F} + \gamma &\quad + 7.994 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{19}F} + p &\longrightarrow \ce{^{16}O} + \alpha &\quad + 8.114 \; {\rm MeV}\hspace{1cm} &\text{($p-\alpha$ decay)} \\
	\ce{^{16}O} + p &\longrightarrow \ce{^{17}F} + \gamma &\quad + 0.60 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{17}F} &\longrightarrow \ce{^{17}O} + e^{+} + \nu_{e} &\quad + 2.76 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay)} \\
	\ce{^{17}O} + p &\longrightarrow \ce{^{18}F} + \gamma &\quad + 5.61 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{18}F} &\longrightarrow \ce{^{18}O} + e^{+} + \nu_{e} &\quad + 1.656 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay)}
\end{alignat}
$$

*Note: In some instances $\ce{^{18}F}$ can combine with a helium nucleus to start a sodium-neon cycle.*

## Hot CNO Cycles
*(Also known as **beta-limited CNO cycles**)*

*Showing similarity to [[#Cold CNO Cycles]]...*

![[CNOcycle_hot_basic.png|align:center]]

*Showing branching of the Hot CNO cycles...*

![[CNOcycle_hot.png|align:center|450]]

With conditions of higher temperature and pressure (in supernovae and x-ray burst) the rate of [[Proton Capture|proton captures]] exceeds the rate of [[Beta Decay#Beta-Plus Decay]], pushing the hydrogen burning process to the [[_Stellar Nucleosynthesis#Table of Nuclides|proton drip line]]. This allows a different chain of catalytic reactions to occur.

### HCNO-I

$$\ce{^{12}C} \; \rightarrow \; \ce{^{13}N} \; \rightarrow \; \ce{^{14}O} \; \rightarrow \; \ce{^{14}N} \; \rightarrow \; \ce{^{15}O} \; \rightarrow \; \ce{^{15}N} \; \rightarrow \; \ce{^{12}C}$$
The difference between the [[#CNO-I]] cycle and the HCNO-I cycle is that $\ce{^{13}N}$ captures a proton instead of decaying.

$$
\begin{alignat}{2}
	\ce{^{12}C} + p &\longrightarrow \ce{^{13}N} + \gamma &\quad + 1.95 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{13}N} + p&\longrightarrow \ce{^{14}O} + \gamma &\quad + 4.63 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{14}O} &\longrightarrow \ce{^{14}N} + e^{+} + \nu_{e} &\quad + 5.14 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 70.641 \; {\rm s}$)} \\
	\ce{^{14}N} + p &\longrightarrow \ce{^{15}O} + \gamma &\quad + 7.35 \; {\rm MeV}\hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{15}O} &\longrightarrow \ce{^{15}N} + e^{+} + \nu_{e} &\quad + 2.75 \; {\rm MeV}\hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 122.24 \; {\rm s}$)} \\
	\ce{^{15}N} + p &\longrightarrow \ce{^{12}C} + \alpha &\quad + 4.96 \; {\rm MeV}\hspace{1cm} &\text{($p-\alpha$ reaction)} \\
\end{alignat}
$$

### HCNO-II

$$\ce{^{15}N} \; \rightarrow \; \ce{^{16}O} \; \rightarrow \; \ce{^{17}F} \; \rightarrow \; \ce{^{17}O} \; \rightarrow \; \ce{^{14}N} \; \rightarrow \; \ce{^{15}O} \; \rightarrow \; \ce{^{15}N}$$
The difference between the [[#CNO-II]] cycle and the HCNO-II cycle is that $\ce{^{17}F}$ captures a proton instead of decaying, leading to the production of $\ce{^{18}Ne}$ and the output of $\ce{^{4}He}$ at a different step in the reaction chain.

$$
\begin{alignat}{2}
	\ce{^{15}N} + p &\longrightarrow \ce{^{16}O} + \gamma &\quad + 12.13 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{16}O} + p &\longrightarrow \ce{^{17}F} + \gamma &\quad + 0.60 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{17}F} + p &\longrightarrow \ce{^{18}Ne} + \gamma &\quad + 3.92 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{18}Ne} &\longrightarrow \ce{^{18}F} + e^{+} + \nu_{e} &\quad + 4.44 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 1.672 \; {\rm s}$)} \\
	\ce{^{18}F} + p &\longrightarrow \ce{^{15}O} + \alpha &\quad + 2.88 \; {\rm MeV} \hspace{1cm} &\text{($p-\alpha$ reaction)} \\
	\ce{^{15}O} &\longrightarrow \ce{^{15}N} + e^{+} + \nu_{e} &\quad + 2.75 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 122.24 \; {\rm s}$)} \\
\end{alignat}
$$

### HCNO-III

$$\ce{^{18}F} \; \rightarrow \; \ce{^{19}Ne} \; \rightarrow \; \ce{^{19}F} \; \rightarrow \; \ce{^{16}O} \; \rightarrow \; \ce{^{17}F} \; \rightarrow \; \ce{^{18}Ne} \; \rightarrow \; \ce{^{18}F}$$
The difference between the [[#HCNO-II]] cycle and the HCNO-III cycle is that $\ce{^{18}F}$ undergoes [[Proton Capture|proton capture]] to produce $\ce{^{19}Ne}$ instead of creating a helium nuclei. 

$$
\begin{alignat}{2}
	\ce{^{18}F} + p &\longrightarrow \ce{^{19}Ne} + \gamma &\quad + 6.41 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{19}Ne} &\longrightarrow \ce{^{19}F} + e^{+} + \nu_{e} &\quad + 3.32 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 17.22 \; {\rm s}$)} \\
	\ce{^{19}F} + p &\longrightarrow \ce{^{16}O} + \alpha &\quad + 8.11 \; {\rm MeV} \hspace{1cm} &\text{($p-\alpha$ reaction)} \\
	\ce{^{16}O} + p &\longrightarrow \ce{^{17}F} + \gamma &\quad + 0.60 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{17}F} + p &\longrightarrow \ce{^{18}Ne} + \gamma &\quad + 3.92 \; {\rm MeV} \hspace{1cm} &\text{($p$ capture)} \\
	\ce{^{18}Ne} &\longrightarrow \ce{^{18}F} + e^{+} + \nu_{e} &\quad + 4.44 \; {\rm MeV} \hspace{1cm} &\text{($\beta^{+}$ decay, $\; \tau_{1/2} = 1.672 \; {\rm s}$)} \\
\end{alignat}
$$

## Energy Generation

Linearizing the [[Nuclear Energy Generation Rate|energy generation rate (per volume)]]...

$$\epsilon_{\rm v} = \rho \, \epsilon_{\rm m} = Q_{\rm nuc} \,  n_{A} \, n_{B} \, \sigma v \left( \frac{1}{1 + \delta_{AB}} \right) \quad \propto \quad Q_{\rm nuc} \,  n_{A} \, n_{B} \, S(E_{0}) \; T_{6}^{-2/3} \, e^{-B T_{6}^{-1/3}}$$

...we find that $\epsilon \propto T^{20}$ such that it has a lot steeper dependence on temperature.