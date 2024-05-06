### Question
---
What evidence is there for "superluminal" jets from black holes, and how does one explain the superluminal motion?

### Answer
---
**Superluminal Motion** is the apparent faster-than-light motion seen in relativistic jets, due to the line-of-sight projections of a given observer.

Evidence of this phenomenon appears in radio knots of [[Active Galactic Nuclei|AGN]] jets. For example, we have observed the apparent motion of the relativistic jets in AGN 3C 279 over the span of $10 \; {\rm yr}$, and it appears that they have traveled $40 \; {\rm lyr}$. 

![[superluminalJet_3C279.jpg|align:center]]

*(resolution can be improved through Long Baseline Interferometry)*

**Explanation:**

Superluminal motion is a special relativistic projection effect caused by relativistic beaming along the line-of-sight. To see mathematically see this effect, we can use the above diagram to describe how an observer will see some projectile (jet knot) move across the observing sky.

![[superluminalJet_diagram.png|align:center|500]]

Lets assume a jet is emitted from $A$ and travels to $B$ with velocity $v$ over the duration of $\delta t \equiv t_{2} - t_{1}$ . For this to be seen by the observer, the light will have to travel some time from ($A$, $B$) such that its received at ($t'_{1}$, $t'_{2}$), respectively.

$$\delta t \equiv t_{2} - t_{1} \hRightarrow t'_{1} = t_{1} + \fpar{D_{\rm L} + v \delta t \cos \theta}{c} \hspace{1.5cm} t'_{2} = t_{2} + \fpar{D_{\rm L}}{c}$$

$$\delta t' \equiv t'_{2} - t'_{1} = \left( t_{2} + \frac{D_{\rm L}}{c} \right) - \left( t_{1} + \frac{D_{\rm L} + v \delta t \cos \theta}{c} \right) = \delta t \left( 1 - \beta \cos \theta \right) \hWhere \beta \equiv \frac{v}{c}$$

To the observer, it appears as though the jet has traveled from $C$ to $B$ on the sky, with the apparent velocity of...

$$v_{\rm app} = \frac{\delta x'}{\delta t'} = \frac{v \delta t \sin \theta}{\delta t \left( 1 - \beta \cos \theta \right)} = \frac{v \sin \theta}{1 - \beta \cos \theta} \hRightarrow \beta_{\rm app} \equiv \frac{v_{\rm app}}{c} = \frac{\beta \sin \theta}{1 - \beta \cos \theta}$$

By plugging in some test values, we can easily see how the projection gives us superluminal motion for small angles (small $\theta$) and relativistic velocities (high $\beta$).

$$\sin \theta \approx \theta \hspace{1cm} \cos \theta \approx 1 \hspace{1cm} \longrightarrow \hspace{1cm} \beta_{\rm app} \approx \frac{\beta \theta}{1 - \beta}$$

![[superluminalJet_projection_map.png|align:center|550]]

This apparent velocity is maximized when...
$$\pd{\beta}{\theta} = 0 \quad \implies \quad \cos \theta_{\rm max} = \beta \quad \implies \quad \beta_{\rm app}^{\rm max} = \frac{\beta \sin \theta_{\rm max}}{1 - \beta \cos \theta_{\rm max}} = \frac{\beta/\gamma}{1 - \beta^{2}} = \beta \gamma$$