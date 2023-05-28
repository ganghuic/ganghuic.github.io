# Dissipative Particle Dynamics

## Derivation

### Fluctuation-Dissipation Theorem

In 1997, Groot and Warren conclude systematically the basic of choosing the parameter in dissipative particle dynamics.<sup><a href="#ref1">1</a></sup> Particles in canonical ensemble(NVT system) update position and velocity by colliding with each other. It needs to be rescaled for position and velocity in every integration steps. So it is easy to derive the following formula.


$$
\tag{1}\vec{p}_i'=\vec{p}_i + \sum_{j}\Omega _{ij}\vec{e}_{ij}
$$


In the above formula, $\vec{e}_{ij} = (\vec{r}_i-\vec{r}_j)/\left | \vec{r}_i-\vec{r}_j \right |$ is the unit vector with the direction of $\vec{r}_{ij}$ . $\Omega_{ij}$ means the momentum transferred from particle $j$ to particle $i$. 



1. <a name = "ref1" href = "http://physics.ujep.cz/~mlisal/pm-cm/dpd_FHmodel.pdf">Groot, R.D., & Warren, P.B. (1997). DISSIPATIVE PARTICLE DYNAMICS : BRIDGING THE GAP BETWEEN ATOMISTIC AND MESOSCOPIC SIMULATION. *Journal of Chemical Physics, 107*, 4423-4435.</a>













<!-- Google tag (gtag.js) --> <script async src="https://www.googletagmanager.com/gtag/js?id=G-HBS60FDTSC"></script> <script>  window.dataLayer = window.dataLayer || [];  function gtag(){dataLayer.push(arguments);}  gtag('js', new Date());   gtag('config', 'G-HBS60FDTSC'); </script>
