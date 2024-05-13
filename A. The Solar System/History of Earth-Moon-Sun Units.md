---
banner: "![[solar_system.png]]"
banner_y: 0.5
aliases:
---
## Deriving [[Units & Conversions#Earth Radius ($R_{ oplus}$)|Earth Radius]]

> [!aside] The Earth is Round
> The ancient Greek philosopher Aristotle (c.384–322 BCE) was able to deduce that the Earth was spherical from observations such as the shape of the Earth’s shadow during lunar eclipses and the changing view of stars in the sky during travel from north to south.

Eratosthenes (c.276–196 BCE) found the [[Units & Conversions#Earth Radius]] by measuring the arclength between the Egyptian cities Syene and Alexandria. He did this by using angles of the incident solar light rays penetrating a deep well on the same day each year.
- When the Sun was directly overhead in Syene, Egypt, the light rays were at zenith ($\theta = 0^{\circ}$)
- On the same day in Alexandria, Egypt, the light rays were $7^{\circ}$ south of zenith ($\theta = 7^{\circ}$)
- The latitudinal distance between Syene and Alexandria was $L \approx 800 \; {\rm km}$.


![[deriving_earthRadius.png|400]]

$$
\text{arclength} = \text{fractional angle} \times \text{circumference}
\hRightarrow
L = \left(\frac{\theta}{360^{\circ}}\right) \times \left( 2 \pi R_{\oplus} \right)
$$
$$
R_{\oplus} = \left(\frac{360}{\theta}\right) \times \frac{L}{2 \pi} \approx 6548 \; {\rm km}
\hspace{1cm}
\text{(3\% error)}
$$

> [!today] Today's Value
> $$R_{\oplus} \approx 6371 \; {\rm km}$$
> Due to the gravitational pull of the moon and other celestial/planetary bodies, the Earth is "flattened" some such that  equatorial radius is $\sim 6378 \; {\rm km}$, but its polar radius is $\sim 6357 \; {\rm km}$.


## Deriving [[Units & Conversions#Lunar Radius ($R_{ rm Moon}$)|Lunar Radius]] &  [[Units & Conversions#Earth-Moon Distance ($D_{ rm EM}$)|Earth-Moon Distance]]

By measuring the relative size of the moon with the umbral shadow during lunar eclipses, Aristarchus (3rd century BCE) calculated the approximate size of the moon through a geometrical argument.

![[deriving_earthMoonDistance.png|align:center|500]]

Taking the angle of the limbs to be $(\theta \approx 1/4 \degree)$, we can use the small angle approximation...

![[moon_ang_diameter.png|align:center|400]]

$$\tan \theta \approx \theta = \frac{R_{\rm moon}}{D_{\rm EM} - R_{\oplus}}$$

...to get the lunar radius in terms of the earth radius.

$$
\begin{align}
	2 R_{\oplus} &= 2 R_{\rm umbral} + 2 D_{\rm EM} \tan \theta \\
	R_{\oplus} &= R_{\rm umbral} + D_{\rm EM} \tan \theta \\
	R_{\oplus} &= \left( f \cdot R_{\rm moon} \right) + \left( R_{\oplus} + \frac{R_{\rm moon}}{\theta} \right) \left( \theta \right) \hRightarrow
	R_{\rm moon} \approx \left(\frac{1 - \theta}{1 + f}\right) R_{\oplus}
\end{align}
$$

From here, we can immediately get the earth-moon distance.

$$R_{\rm moon} \approx \left(\frac{1 - \theta}{1 + f}\right) R_{\oplus} \hspace{3cm}D_{\rm EM} \approx R_{\oplus} + \frac{R_{\rm moon}}{\theta} \approx \left(\frac{1 + f \theta}{\theta + f \theta}\right) R_{\oplus}$$

> [!today] Today's Value
> $$R_{\rm moon} \approx 1737.4 \; {\rm km} \hspace{2cm} D_{\rm EM} \approx 384400 \; {\rm km}$$

## Deriving [[Units & Conversions#Astronomical Unit (${ rm AU}$)|Astronomical Unit (Sun-Earth Distance)]]

![[parallax.png|align:center|450]]

Historically, there has been a variety of methods used to measure the distance between the sun and earth, mostly involving parallax with another object.

- Lunar Orbit (Aristarchus, 310–233 BCE)
	- $1 \; {\rm AU} \sim 1.49 \times 10^{8} \; {\rm km}$
- Parallax with Mars (Jean Richer and Giovanni Domenico Cassini, 1672) 
	- $1 \; {\rm AU} \sim 1.40 \times 10^{8} \; {\rm km}$
- Rare Venus Transits (Edmond Halley, 1761/1769) - occur less than twice per century
	- Difficulties in accurately measuring the contact times due to solar limb darkening and Venus’s image having a diffuse edge. (measurements did not improve later.)
	- $1 \; {\rm AU} \sim 1.53 \times 10^{8} \; {\rm km}$
- Parallax with Mars (David Gill, 1877) 
	- Traveled to Ascension Island in South Africa to observe Mars just after sunset and before sunrise over the course of two days. 
	- Using the diameter of Earth and latitude of the observer as a baseline for a parallax determination of Mars.
	- $1 \; {\rm AU} \sim 1.496 \times 10^{8} \; {\rm km}$  ($2 \% \; {\rm error}$)
- Radar & Telemetry – (Modern Methods)
	- $1 \; {\rm AU} \sim 1.496 \times 10^{8} \; {\rm km}$ 

> [!today] Today's Value
> $$D_{\rm ES} = 1 \; {\rm AU} \approx 1.496 \times 10^{8} \; {\rm km}$$

## Deriving [[Units & Conversions#Solar Mass (${ rm M_{ odot}}$)|Solar Mass]]

There are two ways to easily find a value for the solar mass:

1) **Balancing Centripetal Force & Gravitational Force for Earth's Orbit**
	With the aphelion and perihelion of Earth's orbit differing up to $3 \%$, we can approximate the orbit as circular.
	$$
	\begin{aligned}[b]
	F_{\rm centripetal} &= F_{\rm graviational} \\
	M_{\oplus} \omega^{2} r &= \frac{G M_{\oplus} M_{\odot}}{r^{2}} \\
	M_{\oplus} \left(\frac{2 \pi}{P_{\oplus}}\right)^{2} (D_{\rm ES}) &= \frac{G M_{\oplus} M_{\odot}}{(D_{\rm ES})^{2}}
	\end{aligned}
	\hRightarrow
	M_{\odot} = \left(\frac{4 \pi^{2}}{G P_{\oplus}^{2}}\right) (D_{\rm ES})^{3}
	$$

2) **Using [[Kepler's Laws of Planetary Motion]]**
	Beginning with the area of an ellipse and [[Kepler's Laws of Planetary Motion#Kepler's 2nd Law]], we approximate that the sun is much bigger than Earth ($M_{\oplus} \ll M_{\odot}$) where $a \equiv$ the sun-earth distance$\equiv D_{\rm ES}$.
	$$
	\begin{aligned}[b]
		\pi a^{2} \sqrt{1 - \varepsilon^{2}} &= \int_{0}^{P_{\oplus}} \frac{\mathrm{d} A}{\mathrm{d} t} \; \mathrm{d} t \\
		\pi a^{2} \sqrt{1 - \varepsilon^{2}} &= \frac{L P_{\oplus}}{2 \mu} \\
		\left( \pi a^{2} \right)^{2} &= \frac{P_{\oplus}}{2 \mu} \sqrt{G M \mu^{2} a} \\
		\left(\frac{2 \pi}{P_{\oplus}}\right)^{2} &= \frac{G M \mu}{a^{3}}
	\end{aligned}
	\hRightarrow
	M_{\odot} = \left(\frac{4 \pi^{2} a^{3}}{G P_{\oplus}^{2}}\right) - M_{\oplus} \approx \frac{4 \pi^{2} a^{3}}{G P_{\oplus}^{2}}
	$$

> [!today] Today's Value
> $$M_{\odot} \approx 1.98848 \times 10^{30} \; {\rm kg}$$

