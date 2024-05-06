### Question
---
What is the density profile of a self-gravitating isothermal gas sphere? What is the corresponding rotation curve for this system?

### Answer
---
##### What is the density profile of a self-gravitating isothermal gas sphere?

![[Galaxy Profiles#Isothermal Sphere]]

##### What is the corresponding rotation curve for this system?

To calculate the shape of the [[Velocity Dispersion#Rotation Curve|rotation curve]], we will assume circular motion...

$$v_{\phi} = \sqrt{\frac{G M_{r}}{r}}$$

...and calculate $M_r$ from [[Stellar Structure#Mass Continuity]] with our isothermal density profile.

$$M_{r} = \int_{0}^{r} 4 \pi r^{2} \rho \; \rd r = \int_{0}^{r} 4 \pi r^{2} \fpar{\sigma^{2}}{2 \pi r^{2} G} \; \rd r  = \frac{2\sigma^2 r}{G}$$

Bringing these together:

$$v_{\phi} = \sqrt{\frac{G}{r} \fpar{2 \sigma^{2} r}{G}} = \sigma \sqrt{2}$$

We find a *flat rotation curve*, which arises since $M_r\propto r$. 