### Question
---
Describe the internal structure of the sun. What is the Schwarzschild criterion for convective instability, and how does it delineate the convective and radiative zones in the sun?

### Answer
---
The [[Stellar Structure#Schwarzschild Criterion]] defines the limit at which a radiative zone is no longer stable against the formation of convective cells. The criteria for stability **against** and **for** convection is...

$$
\left\{ \; 
\begin{alignat}{3}
	&\text{Stable (Radiation):} &\hspace{1cm} \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right| &< \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad} \\
	&\text{Unstable (Convection):} &\hspace{1cm} \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right| &\gtrsim \left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad}
\end{alignat}
\; \right\}
\hspace{1cm} \text{where} \hspace{1cm}
\left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad} = \frac{T}{P} \left( 1 - \frac{1}{\gamma_{\rm ad}} \right) \frac{\mathrm{d} P}{\mathrm{d} r}
$$

where $\gamma=\gamma_{\rm ad}$ is the assumed [[Polytropes|polytropic]] exponent (or adiabatic index). We take absolute values because these gradient quantities are often negative. 

The limit on the temperature gradient means that
- Small temperature gradients yields [[Stellar Structure#Radiative Energy Transport]]
- Large temperature gradients yields [[Stellar Structure#Convective ("Adiabatic") Energy Transport]]

![[Stellar Structure#^schwarzchild-limits]]

*(more details can be found at [[Stellar Structure#Schwarzschild Criterion]])*

> [!note] 
> We can also reframe this equation in terms of logarithmic derivatives since $(1/x) df/dx = d \ln(f)/dx$). 
> $$\left| \frac{\mathrm{d} T}{\mathrm{d} r} \right|_{\rm ad} = \left( 1 - \frac{1}{\gamma_{\rm ad}} \right) \frac{\mathrm{d} (\ln P)}{\mathrm{d} (\ln r)}$$