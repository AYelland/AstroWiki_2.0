---
banner: "![[particles.jpg]]"
banner_y: 0.55
aliases:
---

$$
\ce{^{A}_{Z}X} + n \longrightarrow \ce{^{(A+1)}_{Z}X}
$$

Neutron capture is a process in which an atomic nucleus ($\ce{^{A}_{Z}X}$) and one or more neutrons ($n$) collide and merge to form an isotope with one higher atomic mass ($A+1$). If the new isotope is stable, a series of increases in mass can occur, but if it is unstable, then [[Beta Decay#Beta-Minus Decay]] will occur, producing an element of the next higher atomic number ($A-1, Z+1$).

Neutron capture can proceed in two ways depending on the neutron flux: as a rapid process ([[#r-process]]) or a slow process ([[#s-process]]).


> [!note] 
> Since neutrons have no electric charge, they can enter a nucleus more easily than a charged particle, which has to overcome or tunnel through the high Coulomb Barrier. This allows neutron capture to play a significant role in the cosmic nucleosynthesis of elements heavier than iron ($A=56$), whereas elements with $A>56$ cannot be formed through thermonuclear reactions. 

### s-process

![[s-process.png|align:center]]

$$
\ce{^{A}_{Z}X} + n \longrightarrow \ce{^{(A+1)}_{Z}X} 
\hspace{1cm} 
\underbrace{\textcolor{gray}{\left[ \ce{^{A}_{Z}X} \longrightarrow \ce{^{A}_{(Z+1)}X'} + e^{-} + \bar{\nu}_{e} \right]}}_{\rm \beta^{-} \ decay}
\hspace{1cm} \longrightarrow \hspace{1cm}
\ce{^{(A+N)}_{Z'}X'}
$$

The s-process (slow neutron-capture process) occurs when an atomic nucleus ($\ce{^{A}_{Z}X}$) undergoes successive [[#Neutron Capture|neutron captures]], but the neutron flux is low enough that [[Beta Decay#Beta-Minus Decay|beta-minus decay]] **can** occur between captures. *(hence, a "slow" process)*

**Important Notes:**
- Accounts for approximately half the atomic nuclei heavier than iron.
- Each branch of the s-process reaction chain terminates at a cycle involving... 
	- Bismuth *(heaviest "stable" element -- technically, radioactive with half-life $\approx 10^{19} \; {\rm yr}$)*
	- Polonium *(first non-primordial element after bismuth -- half-life $\approx 138 \; {\rm day}$)*
	- Lead *(decay remanent from Polonium)*
- Timescale: $\sim \mathcal{O}(10 \; {\rm yr})$ between successive neutron captures, such that the full process in the reaction chain can take $\sim \mathcal{O}(1000 \; {\rm yr})$

**S-Process Sites:**
- The [[Hertzsprung-Russell Diagram#Asymptotic Giant Branch]] 

### r-process

![[r-process.png|align:center|500]]

$$
\ce{^{A}_{Z}X} + Nn \longrightarrow \ce{^{(A+N)}_{Z}X} 
\hspace{1cm} 
\underbrace{\textcolor{gray}{\left[ \ce{^{A}_{Z}X} \longrightarrow \ce{^{A}_{Z+1}X'} + e^{-} + \bar{\nu}_{e} \right]}}_{\rm \beta^{-} \ decay}
\hspace{1cm} \longrightarrow \hspace{1cm}
\ce{^{(A+N)}_{Z'}X'}
$$

The r-process (rapid neutron-capture process) occurs when an atomic nucleus ($\ce{^{A}_{Z}X}$) undergoes successive [[Neutron Capture|neutron captures]], but the neutron flux is high enough that [[Beta Decay#Beta-Minus Decay|beta-minus decay]] **cannot** occur between captures. *(hence, a "fast"/"rapid" process)* 

This allows the nuclei to become neutron-rich and highly unstable. This process can continue until the nuclei becomes neutron-saturated (i.e. neutron drip line), and then it will undergo many [[Beta Decay#Beta-Minus Decay|beta-minus decay]] in quick succession until it enters the valley of stability.

> [!note] Seed Nuclei
> The r-process creates their own seed nuclei, such that they might proceed in massive stars that contain no heavy seed nuclei. This is unlike the [[#s-process]] which needs a seed nuclei of iron-56 or heavier.

**Important Notes:**
- Accounts for approximately half the atomic nuclei heavier than iron.
- Creates the most neutron-rich stable isotopes of each heavy element
	- Typically, the heaviest four isotopes of every heavy element; heaviest two come only from the r-process
- Restricted by the limit of stability (i.e. neutron drip line) where a nuclei is physically unable to retain neutrons, due to the short range nuclear force. 
- Timescale: $\sim \mathcal{O}(0.01 \; {\rm s})$ between successive neutron captures *(100 captures per second)*

**R-Process Sites:**
- Center of a core-collapse supernova
- Kilonova (binary neutron star merger)
- Thermonuclear weapon explosions
- *Maybe in collapsars (massive star collapse)*

Need locations with a high density of free neutrons. The necessary neutron density is estimated to be $\sim \mathcal{O}(1000 \; {\rm /cm^{3}})$ at $T \approx 2 \; {\rm GK}$ by matching neutron drip line peaks with mass number abundance peaks on the nuclide table.
