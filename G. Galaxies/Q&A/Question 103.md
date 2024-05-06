### Question
---
Sketch the rotation curve of our Galaxy, with approximate scales on the axes. How can information about the rotation curve be determined from 21 cm observations?

### Answer
---
##### Sketch the rotation curve of our Galaxy, with approximate scales on the axes.

![[Velocity Dispersion#Rotation Curve]]

##### How can information about the rotation curve be determined from 21 cm observations?

If we make observations of the [[Spectral Features#21cm line]] in the disk, then we can directly probe the profile of the rotation curve within the Earth's galactic orbit. (geometry breaks down past that)
 
 When we have multiple disconnected clouds of [[Interstellar Medium#Atomic Hydrogen|neutral hydrogen]] along some line-of-sight in the disk (each on a $\sim$ circular orbit), the observed [[Spectral Features#21cm line]] signal will be Doppler shifted with respect to the relative velocity of Earth.

![[21cm_rotation_curves.png]]

If all of the clouds are moving with the same speed, then the largest Doppler shift will be for the cloud whose tangental velocity is directed along our chosen line-of-sight (i.e. towards/away from Earth, "B" above). 

If the clouds aren't moving with the same speed, then the scale of the Doppler shifts could shifted around. This provides some systematic error as we wouldn't know which doppler shift is associated with the maximum, tangential velocity. To address this error, we must use other tracers in the disk to span the other dimensions of phase space. (21cm observations only probe the radial velocity, not the velocity in the sky plane.)

Once we've measured and identified the magnitude of the rotational velocity ($v_{\rm rot} = v_{\rm B}$), we can apply [[Kepler's Laws of Planetary Motion#Kepler's 3rd Law]] assuming a circular orbit (or equivalently circular motion with gravity) to find the radius ($r$) of the orbit.

$$v_{\rm B} = \sqrt{\frac{G M_{r}}{r}} \quad \propto r^{-1/2}$$

With the empirical velocity-radius pairs, we can then compare to the theorized model for the rotation curve. The discrepancies give use evidence for [[Dark Matter|dark matter]] and allows use to model the [[Galaxy Profiles#DM Halo Density Profiles|DM halo density profile]].

> [!note] About the "bumps" in the rotation curve...
> 
> In many rotation curves (including in Megan's notes), we see "bumps" in the rotation curve.
> 
> ![[MW_rotation_curve_closeup.png|align:center|450]]
> ![[rotation_curve_megan.png|align:center|450]]
> 
> These "bumps" originate from discontinuities in the [[Interstellar Medium#Atomic Hydrogen|atomic hydrogen]] clouds in the disk. Geometrically, the maximum rotational velocity of a cloud is not seen directly, but instead, we see projections of rotational velocity. (imagine points $A$ and $C$ in the diagram above, without point $B$). This means the observed Doppler shift is less-than what it should be, giving a lower overall contribution to the rotation curve at the associated radius.

*(This measurement is hard to make near the galactic center because the [[Anatomy of a Galaxy#Galactic Bulge|galactic bulge]] has higher temperatures and less atomic hydrogen.)*
