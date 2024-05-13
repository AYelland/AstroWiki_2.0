---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
Electromagnetic radiation emitted by **non-relativistic accelerating charged particles deflected by a magnetic field**. ($v \ll c \implies \gamma \sim 1$ ) 

The relativistic counterpart to this is [[Synchrotron Radiation]].

![[cyclotron.png|align:center|400]]

> [!note] Cyclotron Frequency
> 
> The **cyclotron frequency** ($\omega_{\rm c} \equiv \omega_{\rm B}$) is an angular frequency of a charged particle ($q$) moving perpendicular to the direction of a uniform magnetic field ($B$). 
> 
> This frequency can be derived from balancing the *Lorentz Force* and and the *Centripetal Force*, assuming the charge ($q$) moves circular motion around the magnetic field.
> 
> $$F_{\rm B} = \frac{q}{c} \, \left( \vec{v} \times \vec{B} \right) = \frac{q B v}{c} \hspace{2.5cm} F_{\rm circ} = m_{0} \frac{v^{2}}{r} = m_{0} \, \omega_{\rm c} \, r$$
> $$m_{0} \, \omega_{\rm c} \, v = \frac{q B v}{c} \hspace{1cm} \Rightarrow \hspace{1cm} \omega_{\rm c} = \frac{q B}{m_{0} c}$$
> 
> *Note: The mass ($m_{0}$) is the rest mass.*

^505df7

The power emitted from cyclotron radiation is:

$$P = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, a^{2} = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \left(\frac{q B v}{m c}\right)^{2} = \left(\frac{q^{4} B}{6 \pi \epsilon_{0} c^{3}}\right) \frac{\beta^{2}}{m^{2}} \hspace{1cm} \Rightarrow \hspace{1cm} P \propto m^{-2}$$

...which tells us that there is much stronger emission from lighter particles that heavier particles ($P \propto m^{-2}$). Therefore, electrons have much more radiation that protons, and hence, particle accelerators use protons to reduce the energy loss and radiation noise.

The spectrum of cyclotron radiation looks like a delta function for a constant magnetic field. In addition to this, we also see weak harmonics and sub-harmonics at integer multiples of the cyclotron frequency. The relative strength of these delta functions can be used to measure magnetic fields.
$$\nu_{c} = \frac{\omega_{\rm c}}{2 \pi} = \frac{q B}{2 \pi m c}$$
![[cyclotron_spectrum.png|align:center|400]]
