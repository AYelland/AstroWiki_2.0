---
banner: "![[galaxies.jpg]]"
banner_y: 0.35
aliases:
---
## Overview

Th **Oort Constants** are empirically derived parameters used to characterize the circular and noncircular components of the stellar motion in the solar neighborhood.

$$A \equiv \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \hspace{2cm} B \equiv - \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} + \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right]$$

They are defined in terms of the rotational velocity ($\Theta$) and radial position ($R$) of stars in the solar neighborhood, where $\Theta_{0}$ and $R_{0}$ are for the Sun's rotational velocity and position. 
- The Oort $A$ constant is associated to the shearing motion of the LSR.
- The Oort $B$ constant is associated to the angular momentum gradient in the LSR (vorticity/circulation).

These relations are directly derived from the relative radial and tangential velocities of other stars (with respect to the Sun) within the "Local Standard of Rest" (LSR).

$$v_{\rm r,rel} = A d \cos 2 \ell \hspace{2cm} v_{\rm \theta, rel} = A d \cos 2 \ell + B d$$
where
- $v_{\rm r,rel} \equiv$ relative radial velocity (along line-of-sight)
- $v_{\rm \theta,rel} \equiv$ relative tangential velocity (with respect to line-of-sight)
- $d \equiv$ distance from sun
- $\ell \equiv$ galactic longitude

## Measurements

To observationally measure the value of the Oort constants, we need:

1) Radial velocities of nearby stars ($v_{\rm r,rel}$) - use stellar spectra measurements
2) Transverse (on-sky) velocities of nearby stars ($v_{\rm \theta, rel}$) - use proper motions
3) Distances to nearby stars ($d$) - use [[parallax.png|parallax]]
4) Galactic longitude ($\ell$)

All of these quantities can be measured by [[Instruments#GAIA]]. The current values for the Oort constants are:

$$A = (15.3 \pm 0.4) \; {\rm km\,s^{-1}\,kpc^{-1}} \hspace{2cm} B= (-11.9 \pm 0.4) \; {\rm km\,s^{-1}\,kpc^{-1}}$$

**Instrument Constraints:**
- Limited by systematics


## Associated Relationships

### Rotational Velocity of Sun around Galactic Center

$$A - B = \frac{\Theta_{0}}{R_{0}} \hspace{1cm} \Rightarrow \hspace{1cm} \Theta_{0} = R_{0} (A-B) \quad \textcolor{gray}{\simeq 230 \; {\rm km/s}}$$

### Period of Sun around Galactic Center

$$\Theta_{0} = \omega_{0} R_{0} \hspace{1cm} \Rightarrow \hspace{1cm} T_{0} = \frac{2 \pi}{\omega_{0}} = \frac{2 \pi R_{0}}{\Theta_{0}} \quad \textcolor{gray}{\simeq  7.13 \times 10^{15 \; {\rm s}} \simeq 226 \; {\rm Myr}}$$

### Local Velocity Shear

$$A + B = - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \hspace{1cm} \Rightarrow \hspace{1cm} \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} = -(A+B) \quad \textcolor{gray}{\simeq -2.45 \; {\rm km\,s^{-1}\,kpc^{-1}}}$$

### Local Epicyclic Frequency

The frequency of the Sun orbit around the guiding center of the LSR as it orbits the galactic center.

$$\kappa^{2} = - 4 B \left( A - B \right) \quad \textcolor{gray}{\simeq 1.18 \times 10^{-15} \; {\rm s^{-1}} \simeq 0.037 \; {\rm Myr^{-1}}}$$

Over the duration of a single orbit around the galactic center ([[#Period of Sun around Galactic Center]]), there are $N_{0}$ oscillations about the guiding center.

$$N_{0} = T_{0} \kappa = \left(\frac{2 \pi R_{0}}{\Theta_{0}}\right) \left( - 4 B (A-B) \right)\quad \textcolor{gray}{\simeq 8.5 \; {\rm oscillations}}$$

## Derivation

By assuming all the stars in the solar neighborhood are on circular orbits around a galactic axisymmetric potential, we can use measurements of the speeds of stars near the Sun to infer information about the rotational properties of the Milky Way.

This is effectively measuring the mean motion of the "local standard of rest" (LSR), which is the collection of objects within $\sim 100 \; {\rm pc}$ of the Sun). This gives us information about the circular and noncircular components of the stellar motion in the solar neighborhood. 

![[oort_constants_diagram.png|align:center]]

Using general trigonometric relations (i.e. law of sines), we can relate the associated quantities in the diagram above...

$$\begin{align}
	\sin \ell &= \frac{R \cos \alpha}{R_{0}} \\
	\cos \ell &= \frac{d + R \sin \alpha}{R_{0}} \\
	\tan \ell &= \frac{R \cos \alpha}{d + R \sin \alpha}
\end{align} \hspace{2cm} 
\frac{R_{0}}{\cos \alpha} = \frac{R}{\sin \ell} = \frac{d}{\cos (\ell + \alpha)}$$

Combining them together, we can find the relative radial and tangential velocity of the star with respect to the Sun (along the line-of-sight).

$$\begin{align}
	v_{\rm r, rel} &= \Theta \cos \alpha + \Theta_{0} \cos (90^{\circ} - \ell) \\
    &= \Theta \cos \alpha - \Theta_{0} \sin \ell \\
    &= \left( \omega R \right) \left( \frac{R_{0}}{R} \sin \ell \right) - \left( \omega_{0} R_{0} \right) \sin \ell \\
    &= \left( \omega - \omega_{0} \right) R_{0} \sin \ell \\
	\\
    v_{\rm \theta, rel} &= \Theta \sin \alpha + \Theta_{0} \sin \left( 90^{\circ} - \ell \right) \\
       &= \Theta \sin \alpha - \Theta_{0} \cos \ell \\
       &= \left( \omega R \right) \left( \frac{R_{0} \cos \ell - d}{R} \right) - \left( \omega_{0} R_{0} \right) \cos \ell \\
       &= \left( \omega - \omega_{0} \right) R_{0} \cos \ell - \omega d
\end{align}$$

If we then focus our scope to the solar neighborhood by assuming $d \ll R_{0}$, we can define radial region by:

$$R_{0} - R\simeq d \cos \ell$$

This assumption allows us to take the Taylor expansion of the angular velocity. $\left[ \omega \equiv \omega(R) = \frac{\Theta(R)}{R} \right]$

$$\omega(R) \approx \omega(R_{0}) + \left. \frac{\mathrm{d} \omega}{\mathrm{d} R} \right|_{R_{0}} (R - R_{0}) + \underbrace{\left. \frac{\mathrm{d}^{2} \omega}{\mathrm{d} R^{2}} \right|_{R_{0}} (R - R_{0})^{2} + \dots}_{\text{drop higher order terms}}$$

$$\begin{align}
    \omega - \omega_{0} = \omega(R) - \omega(R_{0}) &= \left. \frac{\mathrm{d} \omega}{\mathrm{d} R} \right|_{R_{0}} (R - R_{0}) \\
    &= \left[ \frac{1}{R} \frac{\mathrm{d} \Theta}{\mathrm{d} R} - \frac{\Theta}{R^{2}} \right]_{R_{0}} (R - R_{0}) \\
    &= \left[ \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} - \frac{\Theta_{0}}{R_{0}} \right] \frac{(R - R_{0})}{R_{0}} \\
    &= \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \frac{d}{R_{0}} \cos \ell \\
\end{align}$$

Plugging this back into our relative velocities ($v_{\rm r,rel}$, $v_{\rm \theta,rel}$), we can re-express these relationships in terms of $\Theta$ and its derivatives. These relationships define our **Oort Constants**.
$$\begin{align}
    v_{\rm r, rel} &= \left( \omega - \omega_{0} \right) R_{0} \sin \ell \\
        &= \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] d \sin \ell \cos \ell \\
        &= \underbrace{\frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right]}_{\rm \equiv \; A} \; d \sin 2 \ell
\end{align}$$
$$\begin{align}
    v_{\rm \theta, rel} &= \left( \omega - \omega_{0} \right) R_{0} \cos \ell - \omega d \\
        &= \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] d \cos^{2} \ell - \left( \frac{\Theta_{0}}{R_{0}} + \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \frac{d}{R_{0}} \cos \ell \right) d \\
        &= \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] d (\cos 2\ell + 1) - \left( \frac{\Theta_{0}}{R_{0}} + \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \frac{d}{R_{0}} \cos \ell \right) d \\
        &= \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] d \cos 2\ell + \frac{\Theta_{0}}{R_{0}} \left( \frac{d}{2} - d - \frac{d^{2}}{R_{0}} \cos \ell \right) + \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \left( - \frac{d}{2} + \frac{d^{2}}{R_{0}} \cos \ell \right) \\
        &= \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] d \cos 2\ell - \frac{d}{2} \frac{\Theta_{0}}{R_{0}} \underbrace{\left( 1 + \frac{2 d}{R_{0}} \cos \ell \right)}_{\approx 1} - \frac{d}{2} \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \underbrace{\left( 1 - \frac{2 d}{R_{0}} \cos \ell \right)}_{\approx 1} \\
        &= \underbrace{\left( \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \right)}_{\equiv \; A} \,d \cos 2\ell + \underbrace{\left( - \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} + \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \right)}_{\equiv \, B} d
\end{align}$$

In summary, the relative radial and tangential velocities can be expressed in terms of the Oort Constants ($A$ and $B$).

$$
\begin{aligned}
	v_{\rm r,rel} &= A d \cos 2 \ell \\
	v_{\rm \theta, rel} &= A d \cos 2 \ell + B d
\end{aligned}
\hspace{1cm} \text{where} \hspace{1cm}
\boxed{ \;
\begin{aligned}
	A &\equiv ~~~\frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} - \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right] \\
	B &\equiv - \frac{1}{2} \left[ \frac{\Theta_{0}}{R_{0}} + \left( \frac{\mathrm{d} \Theta}{\mathrm{d} R} \right)_{R_{0}} \right]
\end{aligned} \;}
$$
