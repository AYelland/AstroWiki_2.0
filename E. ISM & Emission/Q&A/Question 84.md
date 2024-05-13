---
aliases:
  - cooling function
  - heating function
  - Cooling Function
  - Heating Function
---
### Question
---
Sketch a typical cooling function $\Lambda(T)$ for diffuse interstellar gas and identify its prominent features, spanning from IR to X-ray. Overplot a hypothetical heating curve and show how to identify points of thermal equilibrium and their stability.

### Answer
---
##### Cooling Function
*(See [Good Slide Deck here](http://www.astro.yale.edu/vdbosch/astro610_lecture15.pdf))*

The **cooling function** $\Lambda (T)$ is the functional dependence on temperature for the "cooling rate" ($\mathcal{C}$) of the [[Interstellar Medium|interstellar medium]], where the cooling rate represents by a power (radiation) density of the energy released by the gas. 

$$\mathcal{C} = n^{2} \Lambda(T) \hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}
	\mathcal{C} &\equiv \text{cooling rate} \; {\rm \left[ erg \, cm^{-3} \, s^{-1} \right]} \\
	n &\equiv \text{number density} \; {\rm \left[ cm^{-3} \right]} \\
	\Lambda(T) &\equiv \text{cooling function} \; {\rm \left[ erg \, cm^{3} \, s^{-1} \right]} 
\end{aligned}$$

The energy loss by cooling can be caused a variety of processes, most importantly...
- Free-Bound: Recombination
- [[Bremsstrahlung Radiation|Free-Free Emission]]: Thermal Bremsstrahlung Radiation
- [[Bound-Free Absorption]]: Collisional-ionization *(line emission)*
- [[Bound-Bound Absorption]]: Collisionally-excitation *(line emission)*

![[cooling_processes_diagrams.png|align:center|550]]

![[cooling_processes_plot.png|align:center|550]]


As inferred in the emission processes in the plot above, the cooling function is dependent on the composition of the gas itself. In fact, many different elements contribute to the overall cooling function across a range temperature depending on their ionization and transition energies.


![[cooling_elements.png|align:center|450]]

> [!note] Primordial Gas and First Stars
> 
> When the [[Stellar Populations#Population III (Pop. III)|first stars]] were forming (end of [[Cosmological Timeline#Dark Ages]]), the cooling function was not able to rely on metal line cooling. It was only able to only able to use atomic and molecular cooling mechanism (such as the 4 mentioned above) with hydrogen and helium. As more metals are introduced to the system, more cooling mechanisms become available, and the cooling power increases as seen above.
> 
> ![[cooling_processes_primordial.png|align:center|450]]
> 
> - https://ned.ipac.caltech.edu/level5/Sept15/Johnson/Johnson2.html
> - https://ned.ipac.caltech.edu/level5/Sept12/Glover/Glover1.html


To summarize what processes and features are dominant in the cooling function at different temperature ranges, we use the diagram form Megan's notes. (units: $\left[ \pu{erg cm^{3} s^{-1}} \right]$)

![[cooling_megan.png|align:center]]

*(See [this link](https://www.astro.umd.edu/~richard/ASTRO620/A620_2015_Gas_lec2.pdf) for some more details on where this curvature comes from.)*


##### Heating Function

Similar to the cooling function, there is a **heating function** $\Gamma(T)$ responsible for temperature dependence of "heating rate" ($\mathcal{H}$), where the heating rate represents power density of the energy injected into the gas.

$$\mathcal{H} = n^{2} \, \Gamma(T) \hspace{1cm} \text{where} \hspace{1cm} 
\begin{aligned}
	\mathcal{H} &\equiv \text{heating rate} \; {\rm \left[ erg \, cm^{-3} \, s^{-1} \right]} \\
	n &\equiv \text{number density} \; {\rm \left[ cm^{-3} \right]} \\
	\Gamma(T) &\equiv \text{heating function} \; {\rm \left[ erg \, cm^{3} \, s^{-1} \right]} 
\end{aligned}$$

*(Note: Megan's notes have a typo that was carried into Cian's notes, $\mathcal{H} \ne n \, \Gamma$)*

The energy gain from heating can be caused a variety of processes, including...
- [[Interstellar Medium#Cosmic Rays]] spallation
- Photoionization
- Photoelectric heating from [[Interstellar Medium#Dust|dust grains]]

##### Thermal Equilibrium

Thermal equilibrium is found by balancing of the cooling and heating processes. If we define a **Generalized Loss Function** based on the heating and cooling rates...

$$\mathcal{L}(T) =  n^{2} \, \Lambda(T) - n^{2} \, \Gamma(T)$$

...then we know when there is no energy loss when $\mathcal{L}(T')=0$, and the interstellar gas will be in thermal equilibrium. (Thus, thermal equilibrium is dependent on the function's zeros.)

However, we are interested in the *stability* of these thermal equilibrium points. This is dependent on the derivative (turning points) of the loss function.

$$\begin{align}
	&\left. \frac{\partial \mathcal{L}}{\partial T} \right|_{T'} > 0 \hspace{1cm} \Rightarrow \hspace{1cm} \text{stable equilibrium} \\ 
	&\left. \frac{\partial \mathcal{L}}{\partial T} \right|_{T'} <0 \hspace{1cm} \Rightarrow \hspace{1cm} \text{unstable equilibrium}
\end{align}$$

![[ISM_stability.png|align:center|600]]

- At the **stable** equilibrium points (blue dots), if we perturb the temperature to the left/right, then we will get net heating/cooling in response, returning the gas to equilibrium.
- At the **unstable** equilibrium point (red dot), if we perturb the temperature to the left/right, then we will get net cooling/heating in response, driving the gas further away from equilibrium.

Plotting the heating function over the cooling function, we can now color the regions of instability. From Megan's notes...

![[heating_megan.png|align:center]]

---
Sources:
- https://www.astronomy.ohio-state.edu/pogge.1/Ast871/Notes/Intro.pdf
- https://www.astro.yale.edu/vdbosch/astro610_lecture15.pdf