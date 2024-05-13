---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
**Larmor formula** describes the total power radiated by a non-relativistic point charge as it accelerates. 

## Non-Relativistic Power

For a point charge ($q$) accelerating with acceleration ($a$), the power radiated ($P$) in SI units is...

$$P = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, a^{2} \hspace{1cm} \text{where} \hspace{1cm} \left[ P \right] \equiv {\rm Watts} = {\rm J/s}$$

## Relativistic Power

The relativistic version of this expression is similar; however, we use Lorentz Transformations to convert our system from the in the inertial frame to the observer frame. (the primed values are in the inertial frame).

$$P' = \left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, a'^{\ 2}$$

Here, we see that we must convert the acceleration ($a'$) and power ($P'$) to the inertia frame.

For the acceleration, we apply the chain rule to the acceleration, such that we can replace the relativistic proper acceleration by...

$$a' \equiv \gamma^{2} a \hspace{1cm} \Rightarrow \hspace{1cm} P' =\left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, \gamma^{4} a^{2}$$

> [!note]- Lorentz Transformations of Acceleration
> 
> Applying a Lorentz Transformation for each coordinate...
> 
> $$a \equiv a_{\perp} = \sqrt{{a_{\rm y}}^{2} + {a_{\rm z}}^{2}}$$
> $$\alpha \equiv a'_{\perp} = \sqrt{{a'_{\rm y}}^{2} + {a'_{\rm z}}^{2}}$$
> 
> $$a_{\rm y} \equiv \frac{\mathrm{d} v_{\rm y}}{\mathrm{d} t} = \frac{\mathrm{d} v_{\rm y}}{\mathrm{d} t'} \, \frac{\mathrm{d} t'}{\mathrm{d} t} = \frac{1}{\gamma} \, \frac{\mathrm{d} v'_{\rm y}}{\mathrm{d} t'} \, \frac{\mathrm{d} t'}{\mathrm{d} t} = \frac{1}{\gamma^{2}} \, \frac{\mathrm{d} v'_{\rm y}}{\mathrm{d} t'} = \frac{a'_{\rm y}}{\gamma^{2}}$$
> $$a_{\rm z} \equiv \frac{\mathrm{d} v_{\rm z}}{\mathrm{d} t} = \frac{\mathrm{d} v_{\rm z}}{\mathrm{d} t'} \, \frac{\mathrm{d} t'}{\mathrm{d} t} = \frac{1}{\gamma} \, \frac{\mathrm{d} v'_{\rm z}}{\mathrm{d} t'} \, \frac{\mathrm{d} t'}{\mathrm{d} t} = \frac{1}{\gamma^{2}} \, \frac{\mathrm{d} v'_{\rm z}}{\mathrm{d} t'} = \frac{a'_{\rm z}}{\gamma^{2}}$$
> 
> $$\alpha \equiv a'_{\perp} = \sqrt{\left( \gamma^{2} a_{\rm y} \right)^{2} + \left( \gamma^{2} a_{\rm z} \right)^{2}} = \gamma^{2} \sqrt{{a_{\rm y}}^{2} + {a_{\rm z}}^{2}} = \gamma^{2} a_{\perp} = \gamma^{2} a$$

For the power emitted from an electron, the transformation can similarly be found, such that...

$$P' \equiv P \hspace{1cm} \Rightarrow \hspace{1cm} P =\left(\frac{q^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \, \gamma^{4} a^{2}$$

> [!note]- Lorentz Transformations of Power
> 
> $$P' \equiv \frac{\mathrm{d} E}{\mathrm{d} t} = \frac{\mathrm{d} E}{\mathrm{d} E'} \, \frac{\mathrm{d} E'}{\mathrm{d} t'} \, \frac{\mathrm{d} t'}{\mathrm{d} t} = \gamma \, \frac{\mathrm{d} E'}{\mathrm{d} t'} \, \frac{1}{\gamma} = P$$

We can now go further. Balancing the Coulomb force and Centripetal force of an electron ($q \equiv e$) in a constant magnetic field (circular motion), we can find the [[Synchrotron Radiation#^19855b|synchrotron frequency]] ($\omega_{\rm s}$). The perpendicular velocity can be described with the *pitch angle* ($\alpha$) between the velocity vector and B-field (constant).

$$a_{\perp} \equiv \omega_{\rm s} \, v \sin \alpha = \left(\frac{e B}{\gamma m c}\right) \, v \sin \alpha \hspace{1cm} \Rightarrow \hspace{1cm} P =\left(\frac{e^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \left(\frac{e B}{m c}\right)^{2} \, \gamma^{2} v^{2} \sin^{2} \alpha$$

By convention, we re-express the power in terms of the [[Thomson Scattering#^cross-section|Thompson cross section]] and the magnetic energy density ($U_{\rm B}$). Using SI units....

$$\sigma_{T} = \frac{8 \pi}{3} \left( \frac{1}{4 \pi \epsilon_{0}} \frac{e^{2}}{m c^{2}} \right)^{2} \hspace{2.5cm} U_{\rm B} = \frac{B^{2}}{2 \mu_{0}}$$

$$\begin{align}
	P &= \left(\frac{e^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \left(\frac{e B}{m c}\right)^{2} \, \gamma^{2} v^{2} \sin^{2} \alpha \\
	P &= \left(\frac{e^{2}}{6 \pi \epsilon_{0} c^{3}}\right) \left(\frac{e}{m c}\right)^{2} \left(\frac{B^{2}}{2 
	\mu_{0}}\right) (2 \mu_{0}) \, \gamma^{2} (\beta c)^{2} \sin^{2} \alpha \\
	P &= \left(\frac{2 \mu_{0} e^{4}}{6 \pi \epsilon_{0} m^{2} c^{5}}\right) U_{\rm B} \, \gamma^{2} \beta^{2} \, c^{2} \sin^{2} \alpha \\
	P &= \left( \frac{8 \pi}{3} \left(\frac{e^{4}}{16 \pi^{2} \epsilon_{0}^{2} m^{2} c^{6}}\right) \right) \, 2 \, U_{\rm B} \, \gamma^{2} \beta^{2} \, c \sin^{2} \alpha \hspace{1cm} \textcolor{gray}{\left[ \; c^{2} = \frac{1}{\epsilon_{0} \mu_{0}} \; \right]} \\
	P &= \underbrace{\left( \frac{8 \pi}{3} \left(\frac{e^{2}}{4 \pi \epsilon_{0} m c^{3}}\right)^{2} \right)}_{\sigma_{\rm T}} \, 2 \, U_{\rm B} \, \gamma^{2} \beta^{2} \, c \sin^{2} \alpha
\end{align}$$
$$P = 2 \, \sigma_{\rm T} \, \beta^{2} \, \gamma^{2} \, c \, U_{\rm B} \, \sin^{2} \alpha \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{ \; \left\langle P \right\rangle = \frac{4}{3} \, \sigma_{\rm T} \, \beta^{2} \, \gamma^{2} \, c \, U_{\rm B}  \; }$$
