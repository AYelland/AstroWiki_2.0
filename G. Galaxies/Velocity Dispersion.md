---
banner: "![[galaxies.jpg]]"
banner_y: 0.35
aliases:
---
## Galaxy Velocity Dispersion

A series of relationships derived from the virial theorem, relating velocity dispersion to the mass of the system. In the simplest case, the relation looks something like $$M = \frac{v^2r}{G} \simeq \frac{3 \sigma^{2} R}{2 G}$$where $\sigma$ is the 1D velocity dispersion (radial typically) we can actually measure. This applies to systems that are approximately isotropic, that is a disked galaxy with a net rotation wont have $v\sim \sigma$ since the distribution will be bimodal. In such a case one would be better off using the dispersion of $|\vec{v}|$ to infer the rotational velocity, or just use $v_{circ}$ explicitly. Relationship reliable up to an order $\sim 1-10$ factor

> [!derivation]
> 
> The speeds of the objects in the galaxy have two components
> 1. The center of mass motion of the whole cluster of objects
> 2. The relative motion within the cluster of objects 
> 
> Thus, if we measure the speeds of many objects, we should see a mean speed (corresponding to the center of mass motion) with some of them slower or faster, corresponding to the relative motion within that object. If we assume this speed distribution is Gaussian, then the standard deviation of that Gaussian describes the speed of a typical star within that cluster (without considering the net motion of the cluster). 
> 
> From the [[Virial Theorem]] of a gravitational bound star of mass ($m$), speed ($v$) and distance ($r$) from the center of a spherical mass distribution of mass ($M$)... 
> 
> $$2 \left\langle T \right\rangle + \left\langle U \right\rangle = 2 \left( \frac{1}{2} m v^{2} \right) + \left( -\frac{G M m}{r} \right) = 0 \hspace{1cm} \Rightarrow \hspace{1cm} v^{2} = \frac{G M}{r}$$
> 
> Let's now estimate $v$ and $r$ :
> - If the system is isotropic, then $\sigma_{x} = \sigma_{y} = \sigma_{z}$ and the total velocity dispersion is $\sigma_{\rm 3D} = \sqrt{\sigma_{x}^{2} + \sigma_{y}^{2} + \sigma_{z}^{2}} = \sqrt{3} \, \sigma_{\rm 1D}$. That said, if we make an observation, we really measure a 1-dimensional dispersion (toward us and away from us, denoted $\sigma_{r}$ for radial). A good estimate for the 3D speed of a star is then $v^{2} \simeq 3 \sigma_{r}^{2}$. 
> - A reasonable estimate for the radial location of the average star is $r \simeq R/2$, where $R$ is the galactic radius
> 
> Putting these estimates into the virial theorem and rearranging, we have $$v^{2} = \frac{G M}{r} \hspace{1cm} \Rightarrow \hspace{1cm} \sigma^{2} \simeq \frac{2 G M}{3 R} \hspace{0.5cm} \therefore \hspace{0.5cm} M \simeq \frac{3 \sigma^{2} R}{2 G}$$This result however is only valid up to an order $\sim 1-10$ factor.


## Cluster Velocity Dispersion

Goes back to Zwicky in the 1930s observing the [[Galaxy Cluster#Coma Cluster]]. 

The galaxies in [[Galaxy Cluster|clusters]] are moving with speeds far greater than what can be explained by the observed stellar mass. In order to achieve these speeds, the galaxies would need much more mass and would be much brighter ([[Question 108|Schechter Luminosity Function]]).

Clusters galaxies do tend to have an anomalous mass-light ratio (meaning there is more mass for a given luminosity than expected in comparison to the same luminosity outside of a cluster) due to being a denser region primarily [[Question 107|populated by "red and dead" ellipticals]]; however, the discrepancy between the inferred mass and the kinematics is still an order of magnitude.

In a similar manner to to measuring the mass of elliptical galaxies using *stellar* [[Velocity dispersion#Velocity dispersion|velocity dispersion]] (which can also be evidence for dark matter), we can measure the mass of a cluster via the galaxy velocity dispersion by assuming it is virialized, finding $$M \simeq \frac{3}{2}\frac{\sigma^2R}{G}$$In the [[Galaxy Cluster#Coma Cluster]], Zwicky measured velocity dispersions of $\sim 1000\,\pu{km s^{-1}}$ and inferred a mass. Then comparing that mass to that expected from the light (and realizing our inferred mass from kinematics is much larger) Zwicky offered the following possible resolutions:
1.  stars in the Coma Cluster behave very differently than those in the local Milky Way (emitting much less light at equivalent mass, which turns out to be somewhat true relative to field galaxies but not by a sufficient amount) or
2.  the Coma Cluster is not in equilibrium or
3.  the laws of physics are different here and in the Coma Cluster or
4.  the Coma Cluster contains lots of additional mass which doesn't emit much light: ie **dark matter** exists

## Rotation Curve

Through Newtonian dynamics, we can related the circular velocity ($v_{\rm c} \equiv v_{\phi}$) of a stars in a galaxy to the mass contained ($M_{\rm r}$) within the galactocentric radius $r$.

$$F_{\rm c} = m \frac{v_{\phi}^{2}}{r} = \frac{G M_{r} m}{r^{2}} =F_{\rm g} \hspace{1cm} \Rightarrow \hspace{1cm} v_{\phi} = \sqrt{\frac{G M_{r}}{r}} \quad \propto r^{-1/2}$$

The majority of the stellar mass in the Milky Way is contained within about $r \sim 10 \; {\rm kpc}$. After that, we expect to see the circular velocity decrease, approaching a $1/\sqrt{r}$ curve as there isn't a lot of mass to add to the enclosed mass as radius increases. 

![[rotation_curves.png|align:center|550]]

> [!image] Plot from Xiaowei's Paper
> 
> - All of the dotted curves represent baryonic matter, with the gray dotted curve as the sum of all baryonic matter. 
> - The black line is a fit modelling a DM halo as an Einasto profile (see [[Question 118]]). 

As we can see, the baryonic matter cannot explain the rotation curves of the Milky Way (also seen in other galaxies). There must be an additional mass contribution to the rotation curve (i.e. dark matter).

> [!note] We can use [[Spectral Features#21cm line]] to map rotation curves as well. (see [[Question 103]]).

## Escape Velocity

In a similar manner to the circular velocity, one can estimate the escape velocity at various galactocentric radii by looking at the distribution of stellar speeds, and assuming (roughly speaking) that the distribution of speeds of stars bound to the Milky Way goes to 0 at the escape velocity, since anything going faster should escape. When doing this, and calculating the escape velocity resulting from all the baryons we know about, one finds the following (from Cian's paper)

![[escape_velocity.png|align:center]]

The very large deficit in escape velocity resulting from the baryons can only be accounted for by a very massive and extended halo of some other invisible matter.

## Tully-Fisher Relation

The **Tully-Fisher Relation** (1977) is an empirical relationship between the circular/rotational velocity of a [[Galaxy Classification#Spiral Galaxy|spiral galaxy]] and its [[Luminosity|luminosity]]. *(Analogue to [[Velocity Dispersion#Faber-Jackson Relation|Faber-Jackson]] for spiral galaxies.)*

$$L \propto v_{\rm rot}^{\gamma} \hspace{1cm} \text{where} \hspace{1cm} \gamma \simeq 4$$

**Assumptions**:
- Galaxy radiates as a thin disk
- The mater in the disk is [[Virial Theorem|virialized]]
- Assume that a simple (constant) mass-light ratio applies to all spiral galaxies.

> [!derivation]
> 
> Beginning with the [[Virial Theorem]] and assuming circular motion of a test mass ($m$) around the galactic mass ($M$)....
> 
> $$2 \left\langle T \right\rangle + \left\langle U \right\rangle = 2 \left( \frac{1}{2} m v_{\rm rot}^{2} \right) + \left( - \frac{G M m}{R} \right)= 0 \hspace{1cm} \Rightarrow \hspace{1cm} v_{\rm rot}^{2} = \frac{G M}{R}$$ 
> 
> ...we will assume the disk (spiral galaxy) emits with the following [[Luminosity|luminosity]], dependent on the [[Intensity#Specific Mean Intensity|mean surface brightness]] ($J_{0}$).
> 
> $$L = F \cdot A = (4 \pi J_{0}) \cdot (2 \pi R^{2}) = 8 \pi^{2} J_{0} R^{2} \hspace{1cm} \Rightarrow \hspace{1cm} R = \sqrt{\frac{L}{8 \pi^{2} J_{0}}}$$
> 
> If we let $\Gamma = M/L$ be the mass-light ratio, then we can express the circular velocity as...
> 
> $$v_{\rm rot}^{4} = \frac{\left( G M \right)^{2}}{R^{2}} = \frac{\left(G \, \Gamma  L \right)^{2} \cdot \left( 8 \pi^{2} J_{0} \right)}{L} = \underbrace{\left(8 \pi^{2} G^{2} \Gamma^{2} J_{0} \right)}_{\rm constant} \, L \hspace{1cm} \Rightarrow \hspace{1cm} L \propto v_{\rm rot}^{4}$$

> [!bonus] Hubble Law and Distance Ladder
> - The Tully-Fisher relation can be used to get approximate distances to galactic sources from their circular velocities (via redshift measurements on each side), and thus, it can play a role in the [[Cosmic Distance Ladder]].
> - These days however, its more so used as a consistency check for simulations along with the [[Question 108|Schechter Luminosity Function]]
> 	- If the simulations can reproduce these relations, they are doing an ok job.
> - The Tully-Fisher relation exhibits more of a scatter on a $L-v$ plot when measuring in blue filters than in red. 
>	- Young, blue stars contribute to the majority of the light of a spiral galaxy
>	- Larger red stars contribute most of the mass.
>	- If we measure $L$ from the blue stars (which don't reflect well the total mass of the system), then the mass-light ratio won't accurately describe the mass of the system. 
>	- As a result, better to measure $L$ in the [[Electromagnetic Spectrum|NIR]]


## Faber-Jackson Relation

The **Faber-Jackson Relation** (1976) is an empirical relationship between the stellar [[Velocity Dispersion#Galaxy Velocity Dispersion|velocity dispersion]] of an [[Galaxy Classification#Elliptical Galaxy|elliptical galaxy]] and its [[Luminosity|luminosity]]. *(Analogue to [[Velocity Dispersion#Tully-Fisher Relation|Tully-Fisher]] for elliptical galaxies, but its not as well calibrated)*

$$L \propto \sigma^{\gamma} \hspace{1cm} \text{where} \hspace{1cm} \gamma \simeq 4$$

**Assumptions**:
- Galaxy radiates as a sphere
- The mater in the sphere is [[Virial Theorem|virialized]]
- Assume that a simple (constant) mass-light ratio applies to all elliptical galaxies.

> [!derivation]
> 
> Beginning with the [[Virial Theorem]] and assuming circular motion of a test mass ($m$) around the galactic mass ($M$)....
> 
> $$2 \left\langle T \right\rangle + \left\langle U \right\rangle = 2 \left( \frac{1}{2} m \left(\sqrt{3} \sigma  \right)^{2} \right) + \left( - \frac{G M m}{R} \right) = 0 \hspace{1cm} \Rightarrow \hspace{1cm} \sigma^{2} = \frac{G M}{3 R}$$ 
> 
> ...we will assume the sphere (elliptical galaxy) emits with the following [[Luminosity|luminosity]], dependent on the [[Intensity#Specific Mean Intensity|mean surface brightness]] ($J_{0}$).
> 
> $$L = F \cdot A = (4 \pi J_{0}) \cdot (4 \pi R^{2}) = 16 \pi^{2} J_{0} R^{2} \hspace{1cm} \Rightarrow \hspace{1cm} R = \sqrt{\frac{L}{16 \pi^{2} J_{0}}}$$
> 
> If we let $\Gamma = M/L$ be the mass-light ratio, then we can express the circular velocity as...
> 
> $$\sigma^{4} = \frac{\left( G M \right)^{2}}{9 R^{2}} = \frac{\left(G \, \Gamma  L \right)^{2} \cdot \left( 16 \pi^{2} J_{0} \right)}{9 L} = \underbrace{\left(\tfrac{16}{9} \pi^{2} G^{2} \Gamma^{2} J_{0} \right)}_{\rm constant} \, L \hspace{1cm} \Rightarrow \hspace{1cm} L \propto \sigma^{4}$$


## M-Sigma Relation
*("the [[#Faber-Jackson Relation]] for black holes")*

![[Msigma.jpg|align:center|400]]

The **mass-velocity dispersion (M-$\sigma$) relation** between the mass of a [[Black Hole#Supermassive Black Hole|SMBH]] and the stellar velocity dispersions in the [[Anatomy of a Galaxy#Galactic Bulge|galactic bulge]]. Measurements the index at $n \sim 5$, but originally, it was thought to be closer to $4$. 

$$M \propto \sigma^{n} \hspace{2.5cm} \textcolor{gray}{ \;\left[ \frac{M}{M_{\odot}} \simeq 2 \times 10^{8} \left(\frac{\sigma}{200 \,\pu{km/s}}\right)^{5.1} \; \right]}$$

**Key Points:**
- Measuring black hole masses is hard, but stellar velocity dispersions are not. This allows us to predict their masses. 
- Implies that galaxies and their [[Black Hole#Supermassive Black Hole|SMBH]] coevolve.
	- Measurements of $\sigma$ come from well outside the sphere of influence of the SMBH, so something must connect the galaxy and BH $\implies$ must coevolve.

> [!bonus]- Measuring BH Masses is Hard
> Prior to the M-$\sigma$ relation (discovered in 2000), there was a large discrepancy between the three techniques used to calculate black hole masses.
> 
> 1. Direct/dynamical measurements of the motion of stars or gas near the black hole.
> 	- Gave BH masses that averaged $\approx 1 \%$ of the [[Anatomy of a Galaxy#Galactic Bulge|galactic bulge]] mass (the "Magorrian relation"). 
> 2. [[Methods#Reverberation Mapping]] in [[Active Galactic Nuclei|AGN]]
> 	- Gave BH masses that averaged $\approx 0.1 \%$ of the [[Anatomy of a Galaxy#Galactic Bulge|galactic bulge]] mass
> 3. "Sołtan Argument" - computes the cosmological density in black holes needed to explain the quasar light
> 	- Gave BH masses that averaged $\approx 0.1 \%$ of the [[Anatomy of a Galaxy#Galactic Bulge|galactic bulge]] mass
> 
> The M–σ relation resolved this discrepancy by showing that most of the direct black hole masses published prior to 2000 were significantly in error, presumably because the data wasn't able to resolve the black hole's dynamical sphere of influence. 
> 
> The mean ratio of black hole mass to bulge mass ($M_{\rm BH}/M_{\rm bulge}$) in big early-type galaxies is now believed to be approximately 1 : 200, and increasingly smaller as one moves to less massive galaxies. 
