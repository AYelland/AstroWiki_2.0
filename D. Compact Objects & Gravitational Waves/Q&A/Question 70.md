### Question
---
How are the magnetic fields of neutron stars estimated in (i) X-ray binaries? (ii) radio pulsars?

### Answer
---
##### (i) X-ray binaries?

In an [[Binary Stars#X-Ray Binary]] containing a [[Neutron Star|neutron star]], hot plasma near the surface of the NS produces a spectral continuum of [[Cyclotron Radiation|cyclotron]] resonant scattering features (CRSF), allowing us to determine the magnetic field from the frequency/wavelength of the line(s).

> [!note] The Process of Emission
> - Accretion onto the NS from the donor star persists along the mag field lines and onto the magnetic poles of the NS
> - Produces continuum radiation spectrum *(see [[Question 63]])*, which then travels through the magnetic field with some probability of being scattered by cyclotron radiation
> - Leaves absorption features in the spectrum $\implies$ energy of said feature is proportional to the magnetic field strength
> 
> ![[XRB_cyclotronAbsorption.png|align:center|400]]
> $$E_{\lambda_{0}} = \frac{h c}{\lambda_{0}} \propto B$$

##### (ii) radio pulsars?

In a radio [[Neutron Star#Pulsar]], the magnetic field can be inferred from the exchange between magnetic dipole energy and the rotational energy. Meaning, if we can determine the period ($P$) and how it changes ($\dot{P}$), then we can directly infer how the strength of the magnetic field.

$$
\dot{E}_{\rm B} = \dot{E}_{\rm rot} \hWhere \dot{E}_{\rm B} = \frac{2}{3 c^{2}} \fpar{4 \pi}{\mu_{0}} |\ddot{m}|^{2} \hspace{1cm} \dot{E}_{\rm rot} = I \Omega \dot{\Omega}
$$

The magnetic moment is  $|m| \propto B R^{3}$ , such that $|\ddot{m}| \propto B R^{3} \Omega$ . Therefore, bringing them together...

$$
\begin{align}
	\dot{E}_{\rm B} \; &\propto \; \dot{E}_{\rm rot} \\
	|\ddot{m}|^{2} \; &\propto \; I \Omega \dot{\Omega} \\
	\left( B R^{3} \Omega \right)^{2} \; &\propto \; I \Omega \dot{\Omega} \\
	\left( \frac{B R^{3}}{P} \right)^{2} \; &\propto \; \left( M R^{2} \right) \left( P^{-1} \right) \left( \dot{P} P^{-2} \right) \\
	B^{2} \; &\propto \; \dot{P} P
\end{align}
$$
$$\boxed{\; B \propto ( \dot{P} P )^{1/2} \;}$$

> [!note] Additional Notes...
> 
> - For a more [[Neutron Star#^constant-bfield|explicit calculation]]...
> - This derivation gives rise to linear lines on the [[Neutron Star#P-Pdot Diagram]].
> - Another potentially helpful [link](https://www.cv.nrao.edu/~sransom/web/Ch6.html).

