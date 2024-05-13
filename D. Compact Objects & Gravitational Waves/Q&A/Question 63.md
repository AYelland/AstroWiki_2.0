### Question
---
Explain why you might expect most of the emission of an accreting neutron star to be in the form of X-rays. How does an X-ray pulsar pulse?

### Answer
---
##### Explain why you might expect most of the emission of an accreting neutron star to be in the form of X-rays. 

As with any accretion disk formation, matter loses angular momentum and losses in gravitational potential energy are emitted by radiating light. We want to find the energy, wavelength, or frequency of this radiation.

The easiest way to do that is by finding the temperature of the accretion disk. If we assume that disk radiates like a [[Blackbody Radiation|blackbody]], then we can apply the [[Blackbody Radiation#Stefan-Boltzmann Law]] to find a relationship between power of the emission ([[Luminosity|luminosity]]) for a two-sided disk and the temperature.

$$L = F \cdot A = \left( \sigma T_{\rm eff}^{4} \right) \cdot \left( 2 \pi R^{2} \right) = 2 \pi \sigma R^{2} T_{\rm eff}^{4} \hspace{1cm} \Rightarrow \hspace{1cm} T_{\rm eff} = \left(\frac{L}{2 \pi \sigma R^{2}}\right)^{1/4}$$

If we further assume this is accretion is [[Luminosity#Eddington Limit|Eddington-limited]], then we can calculate $L$ using the typical [[Neutron Star|neutron star]] mass of $1.4 \; {\rm M_{\odot}}$. 

$$L = 3.2 \times 10^{4} \left( \frac{M}{M_{\odot}} \right) L_{\odot} \simeq 10^{31} \; {\rm W}$$

Then, using the typical [[Neutron Star|neutron star]] radius of $\sim 10 \; {\rm km}$, we can calculate $T_{\rm eff}$. 

$$T = \left( \frac{L}{2 \pi R^{2} \sigma}\right)^{1/4} \simeq 10^{7} \; {\rm K}$$

By [[Blackbody Radiation#Wien's Displacement Law]], the temperature of the radiation peaks at...

$$T \simeq 10^{7} \; {\rm K} \hspace{1cm} \Rightarrow \hspace{1cm} \lambda \sim 0.3 \; {\rm nm} \hspace{1cm} \nu \sim 1 \; {\rm Hz} \hspace{1cm} E \sim {\rm keV}$$

This energy, wavelength, frequency, and temperature correlate to [[Electromagnetic Spectrum|x-ray]] values.

##### How does an X-ray pulsar pulse?

Here, there are two questions being asked...

**1) *What mechanism generates the beams of radiation at the poles of an accretion-powered pulsar?***

X-ray [[Neutron Star#Pulsar|pulsars]] are accretion-powered pulsars paired with a normal stellar companion in a binary system. Depending on the size of the companion, it could be classified as a [[Binary Stars#Low Mass X-Ray Binary (LMXB)|LMXB]], [[Binary Stars#Intermediate Mass X-Ray Binary (IMXB)|IMXB]], or [[Binary Stars#High Mass X-Ray Binary (HMXB)|HMXB]].

In these systems, the accreted material from the stellar companion is channeled by the [[Neutron Star|neutron star's]] magnetic field on to the magnetic poles, producing two or more localized "hot spots" or accretion columns. The in-falling material reaches [[Fluid Mechanics#Supersonic|supersonic]] speeds before it impacts the [[Neutron Star|NS]] surface, and the associated gravitational potential energy released by the in-falling gas is primarily emitted in x-ray. The temperatures of the hotspots are correlated to x-ray emission, such that as the neutron star rotates, pulses of X-rays are observed as the hotspots move in and out of the line of sight.

The rate of accretion in [[Neutron Star|neutron stars]] is highly dependent on the magnetic field strength and the location of the [[Question 64|magnetospheric radius]] ($R_{\rm M}$). *([[xray_pulsars.pdf|Walter+Ferrigno, 2017]])*

![[NS_pulsar_accretionColumn_lightCylinder.png|align:center|500]]

- High Magnetic Fields
	- Accretion disk truncated at the [[Question 64|magnetospheric radius]] ($R_{\rm M}$)
	- Accreted material is directed along field lines to magnetic poles and falls into [[Neutron Star|NS]] in a quasi- cylindrical accretion column (creating a "hot spot")
	- Releases gravitational energy in the form of high-energy radiation (non-isotropically)
		- [[Bremsstrahlung Radiation|Bremsstrahlung]]
		- [[Compton Scattering|Comptonization]]
		- [[Cyclotron Radiation|Cyclotron]] Resonant Scattering Features (CRSF)

- Low Magnetic Fields 
	- Accretion disk truncated at the [[Question 64|magnetospheric radius]] ($R_{\rm M}$), but its much closer to the [[Neutron Star|NS]] 
		- Material not funneled to the magnetic poles, but instead the disk extends to the [[Neutron Star|NS]] surface
	- The added angular momentum results in star being spun up (associated with [[Neutron Star#Millisecond Pulsar (MSP)|MSP]] spin-up)
	- The accreted material on the surface of the [[Neutron Star|NS]] accumulates without thermonuclear ignition (similar to a [[Stellar Explosions#Nova|nova event]])
	- When the material ignites, the x-ray emission propagates through the atmosphere of the [[Neutron Star|NS]], allows us to detect the emission as it rotates (non-isotropically)


**2) *What do we observe we looking at a pulsar, and what are the "pulses"?***

A pulsar's magnetic field axis is misaligned with its geometric spin axis. This means that the polar beams (observed in radio) appear like a lighthouse with two bulbs as one (or both if aligned fortunately) of the beams pass over Earth periodically and crosses our line-of-sight.

A challenge to this picture comes from [[Instruments#NICER]]. It has observed multiple X-ray pulses coming from hotspots on the same hemisphere, suggesting a much more complicated magnetic field configuration. In addition to seeing the radio pulses from the beams, these hotspot emit in the x-ray consistently. Due to the gravitational well, the light can be bend around the neutron star, providing a sinusoidal emission curve.