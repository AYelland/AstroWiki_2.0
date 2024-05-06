---
banner: "![[ism.png]]"
banner_y: 0.6
aliases:
---
**Larmor formula** describes the total power radiated by a non-relativistic point charge as it accelerates. 

## Non-Relativistic Power

For a point charge ($q$) accelerating with acceleration ($a$), the power radiated ($P$) in SI units is...

$$P = \fpar{q^{2}}{6 \pi \epsilon_{0} c^{3}} \, a^{2} \hWhere \left[ P \right] \equiv {\rm Watts} = {\rm J/s}$$

## Relativistic Power

The relativistic version of this expression is similar; however, we use Lorentz Transformations to convert our system from the in the inertial frame to the observer frame. (the primed values are in the inertial frame).

$$P' = \fpar{q^{2}}{6 \pi \epsilon_{0} c^{3}} \, a'^{\ 2}$$

Here, we see that we must convert the acceleration ($a'$) and power ($P'$) to the inertia frame.

For the acceleration, we apply the chain rule to the acceleration, such that we can replace the relativistic proper acceleration by...

$$a' \equiv \gamma^{2} a \hRightarrow P' =\fpar{q^{2}}{6 \pi \epsilon_{0} c^{3}} \, \gamma^{4} a^{2}$$

> [!note]- Lorentz Transformations of Acceleration
> 
> Applying a Lorentz Transformation for each coordinate...
> 
> $$a \equiv a_{\perp} = \sqrt{{a_{\rm y}}^{2} + {a_{\rm z}}^{2}}$$
> $$\alpha \equiv a'_{\perp} = \sqrt{{a'_{\rm y}}^{2} + {a'_{\rm z}}^{2}}$$
> 
> $$a_{\rm y} \equiv \td{v_{\rm y}}{t} = \td{v_{\rm y}}{t'} \, \td{t'}{t} = \frac{1}{\gamma} \, \td{v'_{\rm y}}{t'} \, \td{t'}{t} = \frac{1}{\gamma^{2}} \, \td{v'_{\rm y}}{t'} = \frac{a'_{\rm y}}{\gamma^{2}}$$
> $$a_{\rm z} \equiv \td{v_{\rm z}}{t} = \td{v_{\rm z}}{t'} \, \td{t'}{t} = \frac{1}{\gamma} \, \td{v'_{\rm z}}{t'} \, \td{t'}{t} = \frac{1}{\gamma^{2}} \, \td{v'_{\rm z}}{t'} = \frac{a'_{\rm z}}{\gamma^{2}}$$
> 
> $$\alpha \equiv a'_{\perp} = \sqrt{\left( \gamma^{2} a_{\rm y} \right)^{2} + \left( \gamma^{2} a_{\rm z} \right)^{2}} = \gamma^{2} \sqrt{{a_{\rm y}}^{2} + {a_{\rm z}}^{2}} = \gamma^{2} a_{\perp} = \gamma^{2} a$$

For the power emitted from an electron, the transformation can similarly be found, such that...

$$P' \equiv P \hRightarrow P =\fpar{q^{2}}{6 \pi \epsilon_{0} c^{3}} \, \gamma^{4} a^{2}$$

> [!note]- Lorentz Transformations of Power
> 
> $$P' \equiv \td{E}{t} = \td{E}{E'} \, \td{E'}{t'} \, \td{t'}{t} = \gamma \, \td{E'}{t'} \, \frac{1}{\gamma} = P$$

We can now go further. Balancing the Coulomb force and Centripetal force of an electron ($q \equiv e$) in a constant magnetic field (circular motion), we can find the [[Synchrotron Radiation#^19855b|synchrotron frequency]] ($\omega_{\rm s}$). The perpendicular velocity can be described with the *pitch angle* ($\alpha$) between the velocity vector and B-field (constant).

$$a_{\perp} \equiv \omega_{\rm s} \, v \sin \alpha = \fpar{e B}{\gamma m c} \, v \sin \alpha \hRightarrow P =\fpar{e^{2}}{6 \pi \epsilon_{0} c^{3}} \fpar{e B}{m c}^{2} \, \gamma^{2} v^{2} \sin^{2} \alpha$$

By convention, we re-express the power in terms of the [[Thomson Scattering#^cross-section|Thompson cross section]] and the magnetic energy density ($U_{\rm B}$). Using SI units....

$$\sigma_{T} = \frac{8 \pi}{3} \left( \frac{1}{4 \pi \epsilon_{0}} \frac{e^{2}}{m c^{2}} \right)^{2} \hspace{2.5cm} U_{\rm B} = \frac{B^{2}}{2 \mu_{0}}$$

$$\begin{align}
	P &= \fpar{e^{2}}{6 \pi \epsilon_{0} c^{3}} \fpar{e B}{m c}^{2} \, \gamma^{2} v^{2} \sin^{2} \alpha \\
	P &= \fpar{e^{2}}{6 \pi \epsilon_{0} c^{3}} \fpar{e}{m c}^{2} \fpar{B^{2}}{2 
	\mu_{0}} (2 \mu_{0}) \, \gamma^{2} (\beta c)^{2} \sin^{2} \alpha \\
	P &= \fpar{2 \mu_{0} e^{4}}{6 \pi \epsilon_{0} m^{2} c^{5}} U_{\rm B} \, \gamma^{2} \beta^{2} \, c^{2} \sin^{2} \alpha \\
	P &= \left( \frac{8 \pi}{3} \fpar{e^{4}}{16 \pi^{2} \epsilon_{0}^{2} m^{2} c^{6}} \right) \, 2 \, U_{\rm B} \, \gamma^{2} \beta^{2} \, c \sin^{2} \alpha \hspace{1cm} \textcolor{gray}{\left[ \; c^{2} = \frac{1}{\epsilon_{0} \mu_{0}} \; \right]} \\
	P &= \underbrace{\left( \frac{8 \pi}{3} \fpar{e^{2}}{4 \pi \epsilon_{0} m c^{3}}^{2} \right)}_{\sigma_{\rm T}} \, 2 \, U_{\rm B} \, \gamma^{2} \beta^{2} \, c \sin^{2} \alpha
\end{align}$$
$$P = 2 \, \sigma_{\rm T} \, \beta^{2} \, \gamma^{2} \, c \, U_{\rm B} \, \sin^{2} \alpha \hRightarrow \boxed{ \; \expval{P} = \frac{4}{3} \, \sigma_{\rm T} \, \beta^{2} \, \gamma^{2} \, c \, U_{\rm B}  \; }$$
