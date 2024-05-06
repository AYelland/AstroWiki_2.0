### Question
---
How would you compute the age of our universe using the Friedmann equation? What approximations can be made to simply this calculation?

### Answer
---
Using the [[Friedmann Equation]], we can estimate the age of the universe by assuming it is flat and matter dominated.

$$\Omega_{M} =1 \quad , \quad \Omega_{r} = \Omega_{k} = \Omega_{\Lambda} = 0 \hRightarrow H^{2}(a) = \fpar{\dot{a}}{a}^{2} = H_{0}^{2} a^{-3}$$

With these conditions, the scale factor can be found. (see [[Question 137]])

$$a(t) = \left( \frac{3}{2} H_{0} \, t \right)^{2/3} \hRightarrow H(t) = \frac{\dot a}{a} = \frac{H_{0} \, t^{-1/3}}{\frac{3}{2} H_{0} \, t^{2/3}} = \frac{2}{3t} \hTherefore t = \frac{2}{3 H(t)}$$

Evaluating this expression with the present-day Hubble constant $H(t) = H_{0}$, we find an estimate for the age of the universe...

$$t_{0} = \frac{2}{3 H_{0}} = \frac{2}{3} t_{H} \simeq 9 \; {\rm Gyr} \hWhere t_{H} \sim 14 \; {\rm Gyr}$$

...where $t_H$ is the [[Timescales#Hubble Time]].

> [!note]
> This is smaller than other estimates because we assumed the universe was matter-dominated. Matter is the second-fastest driving force in expansion ($\propto a^{-3}$), with radiation as the fastest ($\propto a^{-4}$), and dark energy the slowest ($\propto a^{0}$). As a result, we end up underestimating the age a bit.
