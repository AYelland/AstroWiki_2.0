---
banner: "![[solar_system.png]]"
banner_y: 0.5
aliases:
  - migration processes
  - planetary migration
  - migration
---
## Tidal Migration
*(Usually quoted with **stars** and **planets**, but it can be applied much more generally.)*

When the tidal forces on the planet creates a bulge, the torque between the two bodies can either increase/decrease the semi-major axis of the orbit. This is due to an inequality between the planet's rotational period and the satellite's orbital period. This effect is strongest in highly-eccentric orbits near pericenter.

**How does it work?**

![[tidal_migration.png]]

For many two-body systems, tidal bulges created through gravitational attraction are not aligned with the line intersecting with with center of the two bodies. Because of this, there is a torque between the two between the two bodies that can directly affect their orbits and rotations.

This specifically can occur in *two different scenarios*:
1) The rotational period is shorter (faster rotational frequency) than the orbital period 
	- The tidal bulge is **ahead** of the line of attraction.
	- The central body loses angular momentum.
	- The orbiting body gains angular momentum.
	- The semi-major axis of the orbiting body increases with time.
	$$P_{\rm rot} < P_{\rm orbit} \hspace{1cm} \Rightarrow \hspace{1cm} \text{semi-major axis increases}$$
	
2) The rotational period is longer (slower rotational frequency) than the orbital period
	- The tidal bulge is **behind** of the line of attraction.
	- The central body gains angular momentum.
	- The orbiting body loses angular momentum.
	- The semi-major axis of the orbiting body decreases with time.
	$$P_{\rm rot} > P_{\rm orbit} \hspace{1cm} \Rightarrow \hspace{1cm} \text{semi-major axis decreases}$$

If the orbiting body is in an eccentric orbit, the strength of the tidal forces is strongest when it is near the pericenter. The orbit is slowed and its semi-major axis decreases, reducing its eccentricity.

### Tidal Locking

When two astrophysical bodies at **tidally locked**, there is no angular momentum being transferred between the two orbiting bodies, and they have reached stable equilibrium orbit such that the semi-major axis only fluctuates minimally. 

There are two types of tidal locking:

> [!note]
> Some scientific sources exclusively use a $1:1$ synchronous rotation to define *tidal locking*, and consider the $N_{1}:N_{2}$ spin-orbit resonance separately. That said, both systems rely [[#Tidal Migration]] to achieve and maintain a stable semi-major axis without the exchange of angular momentum.

#### Synchronous Rotation

$$P_{\rm rot} = P_{\rm orbit} \hspace{1cm} \Rightarrow \hspace{1cm} \text{stable semi-major axis}$$

*Synchronous Rotation* occurs when there is no change in the net rotation rate in one of the bodies over the course of a complete orbit. In other words, when the rotational period one body is equal to the orbital period of the other, the same hemisphere of the smaller body always faces the larger object. 

**Example:** the Earth-Moon system

#### Spin-Orbit Resonance
*(Also known as **asynchronous locking**)*

$$N_{1} P_{\rm rot} = N_{2} P_{\rm orbit} \hspace{1cm} \text{where} \hspace{1cm} N_{1},N_{2} \in \mathbb{Z}\hspace{1cm} \Rightarrow \hspace{1cm} \text{stable semi-major axis}$$

*Spin-Orbit Resonance* occurs when the orbit of the smaller body has an integer resonance with spin of the larger body. 

**Example:** the 3:2 spin-orbit resonance of Mercury around the Sun

#### When is tidal locking more likely to occur?

Two astrophysical bodies are more likely to become tidally locked with they are closer together. They need higher torques to migrate quickly and become tidally locked on a reasonable time. The closer together they are, they greater the influence they will have on each others spin and orbit.

## Disk Migration

Disk migration occurs when after some of the planetesimals have formed and the hot protoplanetary disk still exists. 

Through the [[Orbital Resonance|orbital resonances]] and co-rotating resonances (from the gravitational attraction between the planet and the surrounding gas), the planet can be pushed or pulled from its orbit. As the planet moves on its orbit, it perturbs the gas density distribution, and in response, the gas changes the angular momentum of the planet. This can cause:
- An increase of the semi-major axis over time leading to outward migration (i.e. away from the star)
- An decrease of the semi-major axis over time leading to outward migration (i.e. towards from the star)

Disk migrations has been separated into three different types; however, the boundaries between these types is blurry due to non-linear effects.
#### Type I

The migration of low-mass planets only weakly affects the gas density profile in the disk and the migration rate is proportional to the planet's mass. *(Note: the planet remains entirely embedded within the gas as it migrates)*

The most important resonances for type-I migration are those located close to the planet. The direction of the planet's migration is dependent on the following two, competing effects.
- The interaction with the gas disk *interior* to the planet's orbit adds angular momentum to the planet.
- The interaction with the gas disk *exterior* to the planet's orbit removes angular momentum to the planet.
Whichever is stronger will dominate the direction of migration.

> [!note] Additional Information
> 
> - Theoretical calculations suggest that the planet migrates inward in almost all circumstances in short time scales ($10^{6} \, {\rm yr}$).
> - In a highly turbulent disk, Type I migration may be closer to a random walk than a smooth inward migration.
> - May only have minor effect for terrestrial planets due to their low masses and because their final assembly occurs after the gas disk has dispersed; however, it may greatly affect the formation of giant planets through the [[Core-Accretion Theory]].

#### Type II

As massive planets moves through disk on their orbits, they strongly perturb the gas. The exchange of angular momentum *repels* the gas from the vicinity of the planet's orbit, creating an annular gap around the planet where the surface density of gas is low. *(Note: The depth of this gap depends on the temperature and viscosity of the gas and the planet mass.)*

The direction and rate of migration then depends upon how quickly the gas disk responds and tries to flow back into the gap. This means the motion of the planet follows the viscous evolution of the disk.
- If the gas is flows inward towards the host protostar, the planet also moves inward on a viscous timescale. (inner disk)
- If the gas is flows outward by viscous expansion, the planet also moves outward on a viscous timescale. (outer disk)
Because of this, Type II migration is typically slower than Type I migration. 

> [!note] Additional Information
> 
> - Planets that have formed a gap can continue to accrete gas through narrow streams of material that cross the gap. However, the rate of gas accretion declines as the planet grows more massive and the gap becomes deeper.

#### Type III
*(Also known as **runaway migration**)*

Alternatively to Type I or Type II migration, Type III migration is characterized by extremely short migration timescales. Large-scale vortices in the disk rapidly draw the planet in towards the star in a few tens of orbits.

This only applies to fairly extreme disk / planet cases where the migration is driven by the co-orbital torques between gas and an initial, relatively fast, planetary radial motion. The planet's radial motion displaces gas in its co-orbital region, creating a density asymmetry between the gas on the leading and the trailing side of the planet. This creates a partial gaps in the gas disk, allowing that asymmetry to persist and the planet to migrate very quickly inwards/outwards.

## Planetesimal-Driven Migration

Planetesimal-Driven Migration occurs when a planet experiences a gravitational slingshot from smaller bodies (such as [[Smaller Non-Planetary Bodies#planetesimals]]) in their vicinity. When a planet ejects a planetesimal from the planetary system, it must give up energy and it moves closer toward the star (and vise versa). To a degree, this effect only becomes relevant when a planet interacts with a mass comparable to its own. 

Due to the ratio of solids to gas in a typical protoplanetary disk, it seems [[Planetary Classes#Ice Giants]] are more affected by this than other massive planets.

> [!space] In the Solar System...
> 
> The number of Trans-Neptunian Objects (TNOs) provides strong evidence for planetesimal migration having occurred early in Solar System. Many TNOs have been observed to be trapped in 3:2 resonance with Neptune, and this distribution could insinuate the outward migration of Neptune through the scattering of planetesimals to further inward orbits. Once inside of the Neptunian orbit, they would be ejected from the planetary system or sent on highly eccentric orbits by Jupiter, causing Jupiter to migrate inwards.

## Gravitational Scattering

Gravitational scattering by larger planets or over-densities in the protoplantetary disk can very quickly create major changes orbital radii. This can lead to significant, dynamical instabilities that can result in planets being ejected or colliding with the star. If this doesn't occur, then it can put systems near the limits of stability, requiring other migration methods to restore the system to a better configuration. 

For example, when a planet is put into a highly eccentric orbits, this will enable [[#Tidal Migration]] to take over when the planet is near the pericenter of its orbit.

In the [[Nice Model]], systems with an outer disk of planetesimals can also undergo dynamical instabilities from the resonance crossings during [[#Planetesimal-Driven Migration]]; however, for planets with large, eccentric orbits, this dynamical friction with the planetesimals can serve as a means of dampening these orbits and negate some of the effects of gravitational scattering.

> [!space] In the Solar System
>  Due to close encounters with Jupiter and/or Saturn, Uranus and Neptune may have been gravitationally scattered onto large, eccentric orbits at some point in their evolution.

## Kozai Cycles and Tidal Friction

An inclined orbit (relative to the plane of a binary star system) can shrink due to a combination of Kozai cycles and tidal friction. Kozai Cycles are mediated by the [[#Kozai Mechanism]], where the planet's orbit experiences a periodic exchange of eccentricity and inclination. This process can cause near-circular orbits into highly-eccentric orbits, and flip an inclined orbit between a prograde and a retrograde motion.

As the cycle repeats and the semi-major axis evolves, there is a chance the planet's orbit will shrink enough such that it's no longer influenced by one of the binary stars. At this point, the Kozai cycles end and its orbit will then shrink more rapidly as it is tidally circularized.

### Kozai Mechanism

Perturbation of a binary system by a third object which results in a periodic exchange between the binary orbit's eccentricity and inclination.

 <iframe width="560" height="315" src="https://www.youtube.com/embed/1roRAwWb8lE?si=WTqK9V1KZ2fTcTkN" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

This mechanism is important for:
- irregular planetary satellites
- [[Smaller Non-Planetary Bodies#Trans-Neptunian Object (TNO)]]
- extrasolar planets
- multiple star systems
- [[Black Hole|black hole mergers]]

---
## Resources
- http://www.scholarpedia.org/article/Planetary_formation_and_migration
- https://en.wikipedia.org/wiki/Planetary_migration