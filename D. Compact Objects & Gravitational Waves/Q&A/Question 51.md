### Question
---
Describe the various stages of evolution of a supernova remnant. What are the relevant physical processes during each phase? Explain why in the Sedov-Taylor phase of a supernova remnant, the radius expands at $t^{2/5}$.

### Answer
---

![[SN_shock_composite.png|align:center|600]]

**(1) Free Expansion Phase**:  |  $R\propto t$  |  lasts $\sim 100-200$ years  |  $v$ constant 

- When [[Stellar Explosions#Supernova|SN]] first explodes, material ejected at [[Fluid Mechanics#Supersonic|supersonic]] speeds where the initial [[Stellar Explosions#Supernova|SN]] mass is much greater than the [[Interstellar Medium|ISM]] gas enclosed by the expanding sphere. $$M_{\rm S} \gg \left( \frac{4}{3} \pi R_{\rm S}^{3} \right) \, \rho_{0}$$
- This renders the [[Interstellar Medium|ISM]] pressure is negligible, such that the shock front has no deceleration and it expands with constant velocity. $$v = \text{constant} \hRightarrow R_{\rm S} = v_{\rm S} t \hRightarrow \boxed{\; r \propto t \;}$$
- Shock waves sweeps up and collects material from the [[Interstellar Medium|ISM]], eventually slowing down
- Ejected gas is [[Optical depth#Optical thickness|optically thick]] and kept hot by radioactive decay of isotopes created by the supernova. (powers the light curve)
- This expansion continues until the mass collected from ISM is about equal to the initial mass of the ejecta. \[ $M_{\rm S} \simeq \left( \frac{4}{3} \pi R_{\rm S}^{3} \right) \, \rho_{0}$ \] $\implies$ $t \sim 100 - 200 \; {\rm yr}$


**(2) Sedov-Taylor Phase**:  |  $R\propto t^{2/5}$  |  lasts $\sim 10^4$ years  |  $E$ constant

- Ejecta runs "out of steam" kinetically from the free expansion, and the swept of [[Interstellar Medium|ISM]] material dominates the expansion rate. $$M_{\rm S} \ll \left( \frac{4}{3} \pi R_{\rm S}^{3} \right) \, \rho_{0}$$
- Ejecta itself is heated by the [reverse shock](https://ned.ipac.caltech.edu/level5/March05/Dwek/Dwek3_3.html)
- Very hot ionized gas cannot efficiently radiate away energy (cooling time $\gg$ dynamical time)
	- Radiated heat gets absorbed (high opacity) and equilibrated into the system before it escapes
	- Leads to expansion with roughly a constant energy $\implies$ adiabatic
- Material continues adiabatic expansion, driven by thermal pressure of the hot gas, until $T \sim 10^{6} \; {\rm K}$ such that radiation losses becomes significant.

> [!math] Time-Dependence
> 
> Let's derive the time-dependence of the radius in terms of the parameters $E \equiv \text{const}$, $\rho_{0} = \text{const}$, $R \equiv R_{\rm S}$, $v_{\rm S} \equiv \dot{R}$, and  $t$. 
> 
> We can use the conservation of energy, looking at the swept up ISM energy ($E_{\rm kin}$) and the thermal energy ($E_{\rm th}$), where we use the momentum conservation equation of the [[Question 50|Rankine–Hugoniot Jump Conditions]] ($P \propto \rho v^{2}$).
> 
> $$E_{\rm kin} = \frac{1}{2} M_{\rm S} v_{\rm S}^{2} = \frac{1}{2} \left( \frac{4}{3} \pi R_{\rm S}^{3} \right) \rho_{0} v_{\rm S}^{2} = \frac{2}{3} \pi \rho_{0} R_{\rm S}^{3} v_{\rm S}^{2}$$
> 
> $$E_{\rm th} = \frac{3}{2} N k_{\rm B} T = \frac{3}{2} P V = \frac{3}{2} \left( \frac{3}{4} \rho_{0} v_{\rm S}^{2} \right) \left( \frac{4}{3} \pi R_{\rm S}^{3} \right) = \frac{3}{2} \pi \rho_{0} R_{\rm S}^{3} v_{\rm S}^{2}$$
> 
> Combining with the initial SN energy ($E_{\rm SN} \equiv constant$)
> 
> $$E_{\rm SN} = E_{\rm kin} + E_{\rm th} \hRightarrow R^{3} v^{2} = R^{3} \dot{R}^{2} \propto \text{constant}$$
> 
> Integrate the differential equation for how radius scales with time...
> 
> $$
> \left( \td{R}{t} \right)^{2} \, R^{3} \propto {\rm constant} \hRightarrow \int \rd t \propto \int R^{3/2} \; \rd R  \hRightarrow t \propto R^{5/2}
> $$
>
> Such that the time-dependence on the radius is:
> $$\boxed{ \; R \propto t^{2/5} \;}$$
> 
> \**Note: We could also use dimensional analysis, by using an ansatz of a "self-similar" solution (see Geoffrey Mo's notes).*


**(3) Snowplow phase**:  |  $R\propto t^{1/4}$  |  lasts $\sim 10^5$ years  |  $P$ (momentum) constant

- Once temperatures drop to $T \sim 10^{6} \; {\rm K}$, then the ejecta and swept up mass can efficiently cool as it expands 
	- Recombination can now occur between the electrons and protons to form molecular hydrogen
- Since the medium is less ionized and has a lower opacity (more transparent to light), energy is lost to radiation and the thermal pressure decreases, slowing the expansion
	- Energy is no longer conserved.
- Momentum is conserved (since no thermal expansion) and shock wave collects more material from ISM. The swept-up mass is pushed along "like a snowplow".
- Assuming the radius scales with a power-law ($R \propto t^{q}$)... $$p = M_{\rm S} v_{\rm S} = \left( \frac{4}{3} \pi R^{3} \right) \rho \dot{R} = \text{const} \hRightarrow R \propto t^{1/4}$$
- This phase last until $v_{\rm S} \simeq c_{\rm s}$ and the expanding gas becomes apart of the hot coronal phase of the [[Interstellar Medium|ISM]]


**(4) Merger phase**:  |  $R\propto \text{const}$  |  End-state |  $R$ constant

- Eventually enough ISM mass is swept up and instabilities in the gas lead to the ejecta breaking up and dissipating into the ISM. This is the stage of becoming indistinguishable from ISM material.
