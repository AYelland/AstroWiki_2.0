### Question
---
Make a simple, classical argument to show that the spectrum of radiation from monoenergetic electrons with a speed v impinging on ions at an impact parameter b would be roughly flat up to a frequency ~ v/b.

### Answer
---
Consider the scattering of a non-relativistic charge ($q$) with mass ($m$) accelerating due to the presence an ion with charge ($Q$). For an electron-nucleus system, $q=-\,e$  &  $Q = +Ze$.

![[scattering_impact_diagram.png|align:center|400]]

*(Note: this is just [[Bremsstrahlung Radiation|bremsstrahlung radiation]])*

The [[Larmor Formula]] tells us the power/radiation emitted will vary with the acceleration of the charge. However, we will assume the speed is $v$ uniform in the region of interest where most power is emitted (near closest approach). Using Coulomb's force for the acceleration...

$$\begin{align}
	a(r) = \frac{F(r)}{m} &= \frac{1}{m} \left( \frac{1}{4 \pi \epsilon_{0}} \frac{q \,Q}{r^{2}} \right) \\
	&= \frac{q \, Q}{4 \pi \epsilon_{0} m} \fpar{1}{(vt)^{2} + b^{2}} \\
	&= \frac{q \, Q}{4 \pi \epsilon_{0} m \, b^{2}} \left[ 1 + \fpar{vt}{b}^{2}\right]^{-1} \\
	&= \frac{q \, Q}{4 \pi \epsilon_{0} m \, b^{2}} \left[ 1 + \fpar{t}{\tau}^{2}\right]^{-1} \hWhere \tau = \frac{b}{v}
\end{align}$$

...where ($r$) is the distance between the particles and ($\tau = b/v$) is the timescale which the accelerating charge emits radiation *on the approach*. To account for electron deceleration radiation as it leaves the interaction region, we can multiply the timescale by two ($\tau = b/v \; \longrightarrow \; \tau' = 2 \tau = 2 b /\nu$) such that $t'$ represents the "time within the interaction region". 

This timescale plays a significant role in the radiation power prescribed by [[Larmor Formula]].

$$P = \fpar{q^{2}}{6 \pi \epsilon_{0} c^{3}} \, a^{2} \quad \propto \quad \left[ 1+ \fpar{t}{\tau}^{2} \right]^{-2} \hWhere \tau = \frac{b}{v}$$

![[scattering_impact_power.png|align:center|350]]

From this, we see that faster charges ($v\uparrow$) or charges with a closer approach ($b \downarrow$) yield a shorter pulse of radiation. 

With further thought, we can conclude that this interaction timescale ($\tau$) is the smallest radiation timescale for [[Bremsstrahlung Radiation|bremsstrahlung radiation]]. As the timescale decreases ($\tau \downarrow$) , the power also decreases ($P \downarrow$). This means that the charges in the system aren't moving on timescales smaller than this and still radiating energy.

$$\tau = \frac{b}{v} \hRightarrow \boxed{\; \nu = \frac{1}{\tau} = \frac{v}{b} \;} \hspace{1cm} \text{or} \hspace{1cm} \boxed{\; \nu = \frac{1}{\tau'} = \frac{v}{2b} \simeq \frac{v}{b} \;}$$

**The Radiation Spectrum:**
Converting the radiation (power) spectrum to frequency space through a Fourier Transform, we can see more concrete evidence of this statement, along with the flatness of the spectrum.

For details of this derivation, see *"Longair, Section 6.3 - Bremsstrahlung"*, *"Bradt, pg 190"*,  or [here](https://www-zeuthen.desy.de/~pohlmadq/teach/405-505-f05/sess18.pdf). 

Skipping the math, we use the proportionality between the power and the acceleration to determine the power's dependence on the timescale ($\tau$). Assuming that most of the acceleration occurs within the interaction region, the Fourier Transform of the acceleration has integration bounds of $t \in [ \; - \tau, \, \tau \; ]$.

$$P(\nu) \propto P(\omega) \quad \propto \quad \intInfty a^{2} \, e^{- i \omega t} \; \rd t 
\quad \propto \quad \int_{-\tau}^{\tau} \left[ \; (vt)^{2} + b^{2} \; \right]^{-2} \; e^{- i \omega t} \; \rd t \quad \propto \quad \frac{1}{b^{3} v} \, e^{-\omega \tau}
$$

With this result, we can look at the high and low frequency limits to determine the overall behavior of the power spectrum.

$$\begin{alignat}{4}
	&\text{Low Frequency ($\nu$):} &\hspace{1.5cm} &\nu \propto \omega \ll \frac{1}{\tau} = \frac{v}{b} &\hRightarrow &P(\nu) \propto \frac{1}{b^{3} v} \\
	&\text{High Frequency ($\nu$):} &\hspace{1.5cm} &\nu \propto \omega \gg \frac{1}{\tau} = \frac{v}{b} &\hRightarrow &P(\nu) \propto 0 \\
\end{alignat}$$

![[scattering_impact_powerspectrum.png|align:center|500]]