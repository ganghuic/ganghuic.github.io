# Dissipative Particle Dynamics

*Note of reading Multi-scale Theoretical Simulation Methods and Applications for Polymeric Systems.*

## Derivation

### Fluctuation-Dissipation Theorem

In 1997, Groot and Warren conclude systematically the basic of choosing the parameter in dissipative particle dynamics.<sup><a href="#ref1">1</a></sup> Particles in canonical ensemble(NVT system) update position and velocity by colliding with each other. It needs to be rescaled for position and velocity in every integration steps. So it is easy to derive the following formula.


$$
\tag{SA-1-1}\vec{p}_i'=\vec{p}_i + \sum_{j}\Omega _{ij}\vec{e}_{ij}
$$

In the above formula, $\vec{e}_{ij} = (\vec{r}_i-\vec{r}_j)/\left | \vec{r}_i-\vec{r}_j \right |$ is the unit vector with the direction of $\vec{r}_{ij}$ . $\Omega_{ij}$ means the momentum transferred from particle $j$ to particle $i$. After a integration step, the new position of particle is $\vec{r}_i'$.


$$
\tag{SA-1-2}\vec{r}_i' = \vec{r}_i + \frac{\delta t}{m_i}\vec{p}'
$$


In order to guarantee the conservation of momentum, $\Omega_{ij}$ must satisfy the symmetry:$\Omega_{ij} = \Omega{ji}$. That means that the momentum of particle $j$ to particle $i$ and the momentum of particle $i$ to particle $j$ are numerically equal, which ensure the system obeys Galileo invariance. Over the process of the entire simulation, we assume that the mass of every particle is 1(dimensionless  number), so formula(SA-1-1) and formula(SA-1-2) will be equivalent to the following formula.


$$
\tag{SA-1-3} \vec{v}_i' = \vec{v}_i + \sum_{j}\Omega_{ij}\vec{e}_{ij}
$$

$$
\tag{SA-1-4} \vec{r}_i' = \vec{r}_i + \delta t\vec{v}_i'
$$


$\Omega_{ij}$ presents the velocity of particle $j$ to particle $i$. Differentiate the above formula by time, we can derive the following equation.


$$
\tag{SA-1-5} \vec{F}_i' = \vec{F}_i + f_{ij} \vec{e}_{ij}
$$


It indicated that the force acting on particle $i$ has changed, and it attributed the collisions between particles.



 





1. <a name = "ref1" href = "http://physics.ujep.cz/~mlisal/pm-cm/dpd_FHmodel.pdf">Groot, R.D., & Warren, P.B. (1997). DISSIPATIVE PARTICLE DYNAMICS : BRIDGING THE GAP BETWEEN ATOMISTIC AND MESOSCOPIC SIMULATION. *Journal of Chemical Physics, 107*, 4423-4435.</a>













<!-- Google tag (gtag.js) --> <script async src="https://www.googletagmanager.com/gtag/js?id=G-HBS60FDTSC"></script> <script>  window.dataLayer = window.dataLayer || [];  function gtag(){dataLayer.push(arguments);}  gtag('js', new Date());   gtag('config', 'G-HBS60FDTSC'); </script>
