### Question
---
Write down the fluid equations for conservation of mass and momentum that would describe a spherically symmetric, expanding supernova remnant. How would you derive the "jump conditions" for a strong adiabatic shock.

### Answer
---
##### Write down the fluid equations for conservation of mass and momentum that would describe a spherically symmetric, expanding supernova remnant. 

![[Fluid Mechanics#Conservation Laws]]

##### How would you derive the "jump conditions" for a strong adiabatic shock.

The "jump conditions" describe the relationship between the states on both sides of a shock wave when the (one-dimensional) fluid flow undergoes a rapid change.

![[SN_shockfront.png|align:center|500]]


In a simplified picture of a shock front above, we see a rise in density up to a particular point before it "jumps" in a discontinuity. This is due to the shock overdensity moving faster than the medium can respond.

If we work in the *shock front reference frame* where $v_{\rm shock} \equiv v_{\rm s}$ , the we can simply the system by assuming:
- The dynamics are steady-state in this frame: $\partial/\partial t = 0$
- The radial derivatives simplify to 1D Cartesian derivatives: $\frac{1}{r^{2}}\frac{\partial}{\partial r}(r^2\,\cdot) \rightarrow \frac{d}{d x}(\cdot)$ 
- Gravity and other external forces are negligible: $f = 0$
- The unshocked medium is at rest in the lab reference fra,e, so in the shock front frame it moves with speed $v_{s}$ 

With this, we obtain the "[**Rankine–Hugoniot Jump Conditions**](https://en.wikipedia.org/wiki/Rankine%E2%80%93Hugoniot_conditions)" through the conservation laws...

$$
\begin{alignat}{3}
	&\require{enclose}\enclose{circle}{1} \; \text{Mass:} &\hspace{0.1cm} \frac{\mathrm{d} }{\mathrm{d} x} \left( \rho v \right) &= 0 &&\hspace{1cm} \Rightarrow \hspace{1cm}& \rho v &= \rho_{0} v_{\rm S} \\
	\\
	&\require{enclose}\enclose{circle}{2} \; \text{Momentum:} &\hspace{0.1cm} \rho v \frac{\mathrm{d} v}{\mathrm{d} x} + \frac{\mathrm{d} P}{\mathrm{d} x} &= 0 &&\hspace{1cm} \Rightarrow \hspace{1cm}& P + \rho v^{2} &= \rho_{0} v_{\rm S}^{2} \quad \textcolor{gray}{\left[ P_{0} = 0 \right]} \\
	\\
	&\require{enclose}\enclose{circle}{3} \; \text{Energy:} &\hspace{0.1cm} \frac{\mathrm{d} }{\mathrm{d} x} \left( \frac{1}{2} \rho v^{2} + \frac{3}{2} n k_{\rm B} T + P \right) &= 0 &&\hspace{1cm} \Rightarrow \hspace{1cm}& \frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} &= \frac{1}{2} v_{\rm S}^{2} \quad \textcolor{gray}{\left[ P_{0} = 0 \right]}
\end{alignat}
$$

...where the right-hand-side are constants, based on the initial medium and the shock front's energy.

> [!derivation]- Mass Conservation Derivation
> 
> $$
> \begin{align}
> 	\frac{\partial \rho}{\partial t} + \frac{1}{r^{2}} \frac{\partial }{\partial r} (r^{2} \rho v) = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\mathrm{d} }{\mathrm{d} x} (\rho v) &= 0 \\
> 	\int \mathrm{d} (\rho v) &= 0 \\
> 	\rho v - \rho_{0} v_{\rm S} &= 0
> \end{align}
> $$
> $$\rho v = \underbrace{\rho_{0} v_{\rm S}}_{\text{constant}}$$

> [!derivation]- Momentum Conservation Derivation
> 
> $$
> \begin{align}
> 	\frac{\partial v}{\partial t} + v \frac{\partial v}{\partial r} + \frac{1}{\rho} \frac{\partial P}{\partial r} = \frac{1}{\rho} f_{\rm r} \hspace{1cm} \Rightarrow \hspace{1cm} \rho v \frac{\mathrm{d} v}{\mathrm{d} x} + \frac{\mathrm{d} P}{\mathrm{d} x} &= 0 \\
> 	\left( 2 \rho v \frac{\mathrm{d} v}{\mathrm{d} x} - \rho v \frac{\mathrm{d} v}{\mathrm{d} x} \right) + \frac{\mathrm{d} P}{\mathrm{d} x} &= 0 \\
> 	\text{(mass continuity)} \hspace{1cm} \Rightarrow \hspace{1cm} \left( 2 \rho v \frac{\mathrm{d} v}{\mathrm{d} x} - \frac{\mathrm{d} \rho}{\mathrm{d} x} v^{2} \right) + \frac{\mathrm{d} P}{\mathrm{d} x} &= 0 \\
> 	\frac{\mathrm{d} }{\mathrm{d} x} \left( \rho v^{2}  \right) + \frac{\mathrm{d} P}{\mathrm{d} x} &= 0 \\
> 	\frac{\mathrm{d} }{\mathrm{d} x} \left( \rho v^{2} + P \right) &= 0 \\
> 	\int \mathrm{d} \left( \rho v^{2} + P \right) &= 0
> \end{align}
> $$
> $$P + \rho v^{2} = \underbrace{\cancelto{0}{P_{0}} + \rho_{0} v_{\rm S}^{2}}_{\text{constant}}$$

> [!derivation]- Energy Conservation Derivation
> 
> $$
> \begin{align}
> 	\frac{\partial \epsilon}{\partial t} + \frac{1}{r^{2}} \frac{\partial }{\partial r} \left[ r^{2} (\epsilon + P) v \right] = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \frac{\mathrm{d} }{\mathrm{d} x} \left[(\epsilon + P) v \right] &= 0 \\
> 	\\
> 	\frac{\mathrm{d} }{\mathrm{d} x} \left[ \left( \frac{1}{2} \rho v^{2} + \frac{3}{2} n k_{\rm B} T + P \right) v \right] &= 0 \\
> 	\frac{\mathrm{d} }{\mathrm{d} x} \left[ \left( \frac{1}{2} \rho v^{2} + \frac{3}{2} P + P \right) v \right] &= 0 \\
> 	\rho v \; \frac{\mathrm{d} }{\mathrm{d} x} \left[ \frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} \right] &= 0 \\
> 	\rho v \; \frac{\mathrm{d} }{\mathrm{d} x} \left[ \frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} \right] &= 0 \\
> 	\int \mathrm{d} \left( \frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} \right) &= 0
> \end{align}
> $$
> $$\frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} = \underbrace{\frac{1}{2} v_{\rm S}^{2} + \cancelto{0}{\frac{5}{2} \frac{P_{0}}{\rho_{0}}}}_{\text{constant}}$$

Applying the "strong shock" condition ($v_{\rm S} \gg c_{\rm s}$) while assuming some adiabatic energy transport though a monatomic ideal gas, we can solve the above system of equations to find the threshold limits that cause the discontinuity.

$$c_{\rm s}^{2} = \frac{\partial P}{\partial \rho} \; \propto \; \gamma \rho^{\gamma-1} = \frac{\gamma P}{\rho} = \frac{5}{3} \frac{P}{\rho} \hspace{1cm} \text{where} \hspace{1cm} \gamma \equiv \frac{5}{3} \hspace{1cm} P \propto \rho^{\gamma}$$

$$
\begin{alignat}{3}
	&\require{enclose}\enclose{circle}{3} \implies &\hspace{1cm} \frac{1}{2} v^{2} + \frac{5}{2} \frac{P}{\rho} &= \frac{1}{2} v_{\rm S}^{2} \\
	&\require{enclose}\enclose{circle}{2} \implies &\hspace{1cm} \frac{1}{2} v^{2} + \frac{5}{2} \frac{1}{\rho} \left[ \rho_{0} v_{\rm S}^{2} - \rho v^{2} \right] &= \frac{1}{2} v_{\rm S}^{2} \\
	&&\frac{1}{2} v^{2} + \frac{5}{2} \left[ \left(\frac{\rho_{0}}{\rho}\right) v_{\rm S}^{2} - v^{2} \right] &= \frac{1}{2} v_{\rm S}^{2} \\
	&\require{enclose}\enclose{circle}{1} \implies &\hspace{1cm} \frac{1}{2} v^{2} + \frac{5}{2} \left[ \left(\frac{v}{v_{\rm s}}\right) v_{\rm S}^{2} - v^{2} \right] &= \frac{1}{2} v_{\rm S}^{2} \\
	&&-2 v^{2} + \frac{5}{2} v \, v_{\rm S} &= \frac{1}{2} v_{\rm S}^{2} \\
	&&\left( \frac{v_{\rm s}}{v} - 4 \right) \underbrace{\left( \frac{v_{\rm s}}{v} - 1 \right)}_{\substack{\text{trival solution.} \\ \text{nothing changes.}}} &= 0 \\
\end{alignat}
$$
$$
\boxed{ \quad 
v = \frac{1}{4} v_{\rm S}
\hspace{2cm}
\rho = 4 \rho_{0}
\hspace{2cm}
P = \frac{3}{4} \rho_{0} v_{\rm S}^{2}
\quad }
$$

Implementing the [[Thermodynamics#Ideal Gas Law]], we can show that the temperature of the shocked material rises to nearly coronal temperatures.

$$T = \left(\frac{\mu m_{\rm p}}{k_{\rm B}}\right) \frac{P}{\rho} = \left(\frac{\mu m_{\rm p}}{k_{\rm B}}\right) \left( \frac{3}{16} v_{\rm S}^{2} \right) 
\begin{aligned}[t]
	\quad &\sim 2 \times 10^{7} \left(\frac{v_{\rm S}}{1000 \; {\rm km/s}}\right)^{2} [\rm K] \\
	\quad &\sim 1.2 \left(\frac{v_{\rm S}}{1000 \; {\rm km/s}}\right)^{2} [\rm keV]
\end{aligned}$$