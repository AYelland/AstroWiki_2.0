### Question
---
Explain how interstellar dust grains can result in linear polarization of transmitted light. How is the direction of polarization related to the average direction of the interstellar magnetic field (as projected on the plane of the sky)? What major discovery in 2014 was derailed by this phenomenon?

### Answer
---
##### Explain how interstellar dust grains can result in linear polarization of transmitted light. How is the direction of polarization related to the average direction of the interstellar magnetic field (as projected on the plane of the sky)?

**Dust Alignment:**
[[Interstellar Medium#Dust]] grains are conglomerates of chemical molecules, and they are not all spherically symmetric. Their asymmetry can result in various distributions of charge and mass across the dust grain, and therefore, an external magnetic field has a non-zero effect on the dust grains such that it can induce a preferential average alignment of the dust grains' magnetic dipole moments with an external magnetic field.

This alignment is *not ferromagnetic*, but instead *paramagnetic* due to the very weak spin-spin interactions within a given dust grain. The net alignment of the magnetic dipole moments ($\vec{\mu}$) of the grain population will be parallel to the magnetic field ($\vec{B}$) (a lower energy configuration, $\theta=0$), but this is an average of independent, randomly spinning grains, each weakly attracted to the magnetic field.

$$\text{Magnetic Potential Energy:} \quad U = - \vec{\mu} \cdot \vec{B} = - \mu B \,\cos \theta \hspace{1cm} \text{where} \hspace{1cm} \theta \in [0, \pi]$$

In addition to this, there are other mechanisms assist with the grain alignment over time through energy minimization, including Radiative Torque Alignment (RTA), but I won't go into details. *(see [here](https://ntrs.nasa.gov/api/citations/20200001522/downloads/20200001522.pdf))*

![[dust_alignSpin.png|align:center|500]]
![[dust_grainAlign.png|align:center|500]]

The degree of polarization is dependent on the grain size, composition, and the overall alignment.

> [!note]- Ferromagnetic vs. Paramagnetic vs. Diamagnetic
> 
> - **Ferromagnetic** materials are strongly attracted to the magnetic field and aligned to both magnetic poles.
> 	- They retain their magnetic properties when the magnetic field is removed.
> - **Paramagnetic** materials are weakly attracted to magnetic field and aligned to a single magnetic pole.
> 	- They become magnetized in a magnetic field but their magnetism disappears when the field is removed.
> - **Diamagnetic** materials repel both magnetic poles as they created their own induced magnetic field in the opposite direction.
> 	- All materials have this property; paramagnets and ferromagnets simply have attractive forces stronger than the repellant force.

**Polarization of Background Light:**
As the un-polarized light interacts with the dust cloud, it is preferentially absorbed along the "long axis" of the dust grains (perpendicular to the external magnetic field). Thus, the light coming out the other side of the dust cloud will be polarized along the "short axis" (parallel to the external magnetic field), given that the orthogonal component will be largely attenuated. *(left image below)*

**Polarization of Thermal Radiation:**
The absorption of light in the dust grains causes them to heat up and re-emit as a [[Blackbody Radiation|blackbody]]. Given the alignment of the grains, the thermal radiation will preferentially emitted along the "long axis", such that it is polarized perpendicular to the magnetic field. *(right image below)*

![[dust_polarization.jpg|align:center]]

##### What major discovery in 2014 was derailed by this phenomenon?
*(Publishment: [Nature](https://www.nature.com/articles/nature.2015.16830))*

Typically dust has temperatures of $T \sim 2- 200 \; {\rm K}$.

For dust at temperatures $T \sim 20 \; {\rm K}$, the thermal ([[Blackbody Radiation|blackbody]]) radiation peaks in the [[Electromagnetic Spectrum|infrared/microwave]] (with wavelength of $\lambda_{\rm peak} \sim 150 \; {\rm \mu m}$ by [[Blackbody radiation#Wien's displacement law|Wien's Law]]), very close to the [[Cosmic Microwave Background|CMB]].

In 2014, the [[Instruments#BICEP|BICEP2]] team claimed to have measured B-mode polarization in the [[Cosmic Microwave Background|CMB]], providing evidence for primordial gravitational wave signals during inflation. However, after some further analysis and additional data (from [[Instruments#Planck]]), this revealed that the signal could entirely be produced by polarized thermal emission from [[Galaxies - General#The Milky Way|Milky Way]] dust.

> [!note] B-mode Polarization
> - Polarization at $45 \degree$ angle with respect to the plane wave direction of propagation.
> - Theory says that inflationary [[Gravitational Waves|gravitational waves]] shoud produce B-mode polarization in the [[Cosmic Microwave Background|CMB]]

> [!cian] 
> Apparently the BICEP signal was at $150 \,\pu{GHz} \sim 2\,\pu{mm}$, so by [[Blackbody Radiation#Wien's Displacement Law|Wien's Law]] this would correspond to a temperature on the order of $1\,\pu{K}$? There is some $\sim 1-10\,\pu{K}$ dust in the Milky Way, but its mostly between $20$ and $200\,\pu{K}$.

