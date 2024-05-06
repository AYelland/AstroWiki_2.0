### Question
---
What is "Press-Schechter theory" and why is it wrong?

### Answer
---
##### What is "Press-Schechter theory"...

![[Press-Schechter#Press-Schechter Theory]]

Using this theory, we can find the [[Press-Schechter#Press-Schechter Halo Mass Function]] that tells us the number of halos (collapsed structures) we will find in some volume element.

$$N(M) \; \rd M = \frac{1}{\sqrt{2 \pi}} \; \fpar{\delta_{c}}{\sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \; \td{\sigma_{M}}{M} \; \rd M$$
$$\Downarrow$$
$$n(M) \; \rd M = \frac{1}{\sqrt{2 \pi}} \; \fpar{\rho_{0} \delta_{c}}{M \sigma_{M}^{2}} \exp \left[ - \frac{\delta_{c}^{2}}{2 \sigma_{M}^{2}} \right] \; \td{\sigma_{M}}{M} \; \rd M$$

##### ...and why is it wrong?

The PS formalisms is wrong because it only accounts for $1/2$ of the mass in the universe (all of the mass should be a halo). This can be see through the normalization of the [[Press-Schechter#Press-Schechter Halo Mass Function]].

![[Press-Schechter#Normalization]]

Therefore, to correct the Press-Schechter formalism, we introduce a "fudge factor" to our equality.

$$P( \,> M) = 2 \cdot P \left( \delta(M) > \delta_{\rm crit} \right)$$

This "fudge factor" originates from the *cloud-in-cloud* problem, where there could be an underdensity within an overdense region on a given mass scale. The PS formalism would say that these objects are not part of a halo with mass $> M$, though they should be included in the collapse.

![[press-schechter-theory_underdensity.png|align:center|350]]

Another way to look at it is that once things go nonlinear, the collapse is able to draw matter in from less dense regions, hence much of the mass does end up in the overdense regions, albeit a different M.

> [!bonus]- The Extended Press-Schechter Formalism
> 
> In order to address the fudge factor properly, the [[Press-Schechter#Extended Press-Schechter Theory]] has been developed.
> 
> ![[Press-Schechter#Extended Press-Schechter Theory]]