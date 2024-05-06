### Question
---
Explain, from a statistical mechanics point of view, why the Balmer lines are most prominent in A stars with an effective temperature of $\gg 10^{4} \; {\rm K}$.

### Answer
---
> [!key-idea] Big Picture
> The [[Spectral Features#Balmer Series]] (transitions to first excited ($n=2$) state of [[Interstellar Medium#Atomic Hydrogen|atomic hydrogen]]) is most strongly seen in [[Spectral Classes#A]] stars ($T \sim 7500-10000 \; {\rm K}$) because:
> 
> - Using the [[Saha Equation]], we can determine the relative abundances of ionized-to-neutral atoms as a function of temperature ($T$)
> 	- Hydrogen completely ionizes around $T \sim 10^{4} \; {\rm K}$
> - Using the [[Boltzmann Equation]], we can determine the relative abundances of atoms in the $n=1,2,3,\dots$ energy states as a function of temperature ($T$).
> 	- It turns out that the fractional occupancy of the $n=2$ energy level spikes at $10^{4} \; {\rm K}$, meaning at this temperature we see the most transitions to this level.
> 
> Intuitively, above this temperature, the hydrogen is mostly ionized (since ionization energy is just above the $n=2$ energy level), and below this temperature, most electrons are in the ground state ($n=1$), yielding the [[Spectral Features#Lyman Series]], not the [[Spectral Features#Balmer Series]].
> 
> So basically...
> $$\text{Balmer lines} \propto \fpar{n_{\text{un-ionized, } 2}}{n_{\text{tot}}} = \underbrace{\fpar{n_{\text{un-ionized, } 2}}{n_{\text{un-ionized, tot}}}}_{\text{Boltzmann factor}} \; \underbrace{\fpar{n_{\text{un-ionized, tot}}}{n_{\text{tot}}}}_{\text{Saha}} $$

Hydrogen only has a single ionized level (since it only has one electron to "give"). Therefore, the total number density can be represented by: $n_{\rm tot} = n_{\rm I} + n_{\rm II}$ where the roman subscripts refer to $\rm{HI}$ and $\rm{HII}$, the neutral (un-ionized) and singly-ionized states of Hydrogen, respectively. 

**Saha Equation:**
Using the [[Saha Equation]]...

$$\frac{n_{r+1}}{n_{r}} = \fpar{g_{e}\,g_{r+1}}{g_{r}} \fpar{1}{\lambda^{3} \, n_{e}} \,e^{-\chi_{r} / k_{\rm B} T} \hWhere \lambda \equiv \fpar{h^{2}}{2 \pi m_{e} k_{\rm B} T}^{1/2}$$

...where we can identify that ($n_{r+1} = n_{\rm II}$) and ($n_{r} = n_{\rm I}$). Additionally using the [[Saha Equation#^degeneracies|linked degeneracies]], this simplifies to...

$$\frac{n_{\rm II}}{n_{\rm I}} = \fpar{1}{\lambda^{3} \, n_{e}} \, \exp \left[ - \frac{13.6 \; {\rm eV}}{k_{\rm B} T} \right]$$

This allows us to define the fraction of $\ce{H}$ atoms in an netural state.

$$\frac{n_{\rm I}}{n_{\rm tot}} = \frac{n_{\rm I}}{n_{\rm I}+n_{\rm II}} = \left[ 1 + \frac{n_{\rm II}}{n_{\rm I}} \right]^{-1} = \left[ 1 + \fpar{1}{\lambda^{3} \, n_{e}} \, \exp \left[ - \frac{13.6 \; {\rm eV}}{k_{\rm B} T} \right] \right]^{-1}$$

**Boltzmann Equation:**
The neutral hydrogen population ($n_{\rm I}$) can be broken down into a sum of the energy level states ($n_{\rm I} = n_{1} + n_{2} + \dots$), where the subscript refers to the $n^{th}$ energy level. 

Using the [[Boltzmann Equation]] for the relative population of $n=2$ to the $n=m$ energy states of atomic hydrogen...

$$\frac{n_{2}}{n_{m}} = \frac{g_{2}}{g_{m}} \, \exp \left[ \frac{-(E_{2} - E_{m})}{k_{\rm B} T} \right] \quad \textcolor{gray}{= \frac{8}{2 m^{2}} \, \exp \left[ \frac{13.6 \; {\rm eV}}{k_{\rm B} T} \, \left( \frac{1}{4} - \frac{1}{m^{2}} \right) \right]}$$

where...
- $E_{m} = E_{0} / m^{2} = (-13.6 \; {\rm eV}) / m^{2}$
- $g_{m} = S \times m^{2}$
	- Spin Degeneracy: $S = 2s+1$
	- Energy Level Degeneracy: $m^{2}$

Sum over the $m$ energy states, we can define the fraction of $\ce{H}$ atoms in an $n=2$ energy state relative to the total population of neutral hydrogen ($n_{\rm I} = n_{1} + n_{2} + \dots$).

$$\frac{n_{2}}{n_{\rm I}} = \sum_{m=1}^{\infty} \frac{g_{2}}{g_{m}} \; \exp \left[ \frac{-(E_{2} - E_{m})}{k_{\rm B} T} \right]$$

**Combining the Saha and Boltzmann Relations:**
Putting these together, we can define the fraction of $\ce{H}$ atoms in an $n=2$ state relative to all hydrogen (neutral or ionized) as a function of temperature, which ends up looking like this:

$$\frac{n_{2}}{n_{\rm tot}} = \underbrace{\fpar{n_{2}}{n_{m, \, {\rm I}}}}_{\rm Boltzmann} \; \underbrace{\left( \frac{n_{\rm I}}{n_{\rm tot}} \right)}_{\rm Saha}$$
  
![[balmer_fraction.png|align:center|600]]

We can see here that the fraction of $n=2$ states peaks at $T \sim 10^{4} \; {\rm k}$, and hence, the [[Spectral Features#Balmer Series]] is prominent.