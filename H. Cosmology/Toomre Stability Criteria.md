---
banner: "![[cosmology.png]]"
banner_y: 0.46
aliases:
---
The **Toomre Stability Criterion** is a full stability criterion for a galactic stellar disk.

$$Q = \frac{\sigma}{\sigma_{\rm crit}} 
\begin{cases}
>1 &\hspace{0.5cm} \text{stable} \\
<1 &\hspace{0.5cm} \text{unstable}
\end{cases}$$
...where $\sigma$ is the disk velocity dispersion and $\sigma_{\rm crit}$ is the critical value derived from bringing together the stability criteria for large scales and small scales.

On the **large scale**, galactic disks are stabilized by *rotational motion*. If we were to introduce a radial perturbation to some star on the disk (initiating epicyclic motion), the we can use Newtonian mechanics to balance the centripetal and gravitational forces. Keeping mass and angular momentum conserved, we find that the system remains stable if:

$$R_{\rm rot} > \frac{2 \pi G \Sigma}{3 \Omega^{2}} \hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}
G &= \text{gravitational constant} \\
\Sigma &= \text{surface density of stellar disk to $R$} \\
\Omega &= \text{rotational frequency}
\end{aligned}$$


On the **smaller scale**, stability is achieved through *random motion* if...

$$R < \lambda_{J} 
\hspace{1cm} \text{where} \hspace{1cm}
\begin{aligned}[t]
 \lambda_{J} \equiv \frac{\pi v_{s}^{2}}{G \rho_{0}} = \frac{\pi \sigma^{2}}{G \rho_{0}} &\equiv \text{Jeans Length} \\
 v_{s} &= \text{sound speed} \\
 \sigma &= \text{velocity dispersion} \\
 \rho_{0} &= \text{background density}
\end{aligned}$$


Combining the two stability criteria with the epicyclic frequency ($\kappa = \sqrt{2} \, \Omega$), we can derive the critical velocity dispersion for Toomre's Full Stability Criterion.

$$\begin{align}
\lambda_{J} \ge R_{\rm rot} 
\hspace{1cm} \Rightarrow \hspace{1cm} 
\begin{aligned}[t]
\frac{\pi \sigma^{2}}{G \rho_{0}} &\ge \frac{2 \pi G \Sigma}{3 \Omega^{2}} \\
\frac{\pi \sigma^{2}}{8 G \Sigma} &\ge \frac{2 \pi G \Sigma}{3 \Omega^{2}} \\
\sigma^{2} &\ge \frac{16 G^{2} \Sigma^{2}}{3 \Omega^{2}} \\
\sigma &\ge \frac{4 G \Sigma}{\sqrt{3} \, \Omega} \\
\sigma &\ge \sqrt{32}{3} \, \left(\frac{G \Sigma}{\kappa}\right) \approx 3.26 \, \left(\frac{G \Sigma}{\kappa}\right)
\end{aligned}
\end{align}$$

$$\sigma_{\rm crit} \equiv \sqrt{32}{3} \, \left(\frac{G \Sigma}{\kappa}\right) \approx 3.26 \, \left(\frac{G \Sigma}{\kappa}\right) 
\hspace{1cm} \Rightarrow \hspace{1cm}
\sigma \ge \sigma_{\rm crit} \hspace{1cm} \Rightarrow \hspace{1cm} \boxed{Q = \frac{\sigma}{\sigma_{\rm crit}}}$$
