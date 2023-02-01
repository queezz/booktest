# Star formation
## Free fall
...
## Hydrostatic Equilibrium

An element of mater at a distance $r$ from the center of a spherical system will be in hydrostatic equilibrium if the pressure gradient at $r$ is 

$$
\newcommand{\d}{\mathop{}\!{\text{d}}}
\newcommand{\p}{\mathop{}\!{\partial}}
\frac{\d P}{\d r} = - \frac{Gm(r)\rho(r)}{r^2}.
$$ (pressure_gradient)

The whole system is in equilibrium if this equation is valid at all radii, $r$. To derive a simple relation between the average internal pressure and the gravitational potential energy of the system, we multiply Eq. {eq}`pressure_gradient` by $4\pi r^3$ and integrate from $r=0$ to $r=R$ to obtain

$$
\newcommand{\d}{\mathop{}\!{\text{d}}}
\newcommand{\p}{\mathop{}\!{\partial}}
\int_0^R 4\pi r^3\frac{\d P}{\d r}\d r = -\int_0^R \frac{Gm(r)\rho(r) 4\pi r^2}{r} \d r.
$$ (pressure_gravity_equilibrium)

Both sides of this equation have simple physical significance. The right-hand side is simply the gravitational potential energy of the system:

$$
\newcommand{\d}{\mathop{}\!{\text{d}}}
\newcommand{\p}{\mathop{}\!{\partial}}
E_{\text{GR}} = -\int^{m=M}_{m=0} \frac{Gm(r)}{r}\d m,
$$ (gravitational_energy_integral)
where $\text{d}m$ is the mass between $r$ and $r+\text{d}r$; i.e. $\rho(r)4\pi r^2\text{d}r$. The left-heand side can be integrated by parts to give

$$
\newcommand{\d}{\mathop{}\!{\text{d}}}
\newcommand{\p}{\mathop{}\!{\partial}}
\int_0^R 4\pi r^3\frac{\d P}{\d r}\d r = \left[ P(r)4\pi r^3\right]_0^{R} - 3 \int_0^R P(r)4\pi r^2\d r.
$$ (pressure_gradient_integral)

The first term is zero because the pressure on the outside surface at $r=R$ is zero. The second term is equal to $-3\langle P \rangle V$, where $V$ is the volume of the system and $\langle P \rangle$ is the volume averaged pressure. Hence, we conclude that the average pressure needed to support a system with gravitational energy $E_{\text{GR}}$ and volume $V$ is given by 

$$
\langle P \rangle = - \frac{1}{3}\frac{E_{\text{GR}}}{V}.
$$ (virial_theorem)

<!---
Star formation diagram
![](https://ipag.osug.fr/~mottef/img/MotteFig08.jpg)
--->
`````{admonition} Virial theorem
:class: tip
The average pressure is one third of the density of the stored gravitational energy.
`````

To derive the relation between the pressure and the internal energy density due to the translational motion of the particles we consider a gas of $N$ particles in a cubical box of volume $L^3$ with its edges oriented along the $x$, $y$, and $z$ axes. Initially we shall focus on a gas particle with velocity $\vec{v} = (v_x,v_y,v_z)$ and momentum $\vec{p} = (p_x,p_y,p_z)$. As this particle bounces around the box it strikes the sides at regular intervals. in particular, the rae at which it strikes one of the sides perpendicular to the z axis is $v_z/2L$, and in so doing it imparts a momentum $2p_z$ with each strike. Hence the rate of momentum transfer to unit area of the side is $p_zv_z/L^3$. We now consider all $N$ particles in the box. The pressure due to these particles on a side perpendicular to the $z$ axis is 

$$
P = \frac{N}{L^3}\langle p_zv_z\rangle,
$$ (pressure_in_a_box)
where the brackets denote an average over all the particles. If the gas is isotropic all directions of motion for the particles are equally likely and 

$$
\langle p_xv_x\rangle = \langle p_yv_y\rangle = \langle p_zv_z\rangle = \langle \vec{p} \cdot \vec{v}\rangle /3,
$$

where 

$$
\vec{p} \cdot \vec{v} = p_xv_x + p_yv_y+p_zv_z .
$$

...

- For a gas of non-relativistic particles of mass $m$, $\vec{p}\cdot\vec{v} = mv^2$ and the pressure becomes

$$
P = \frac{2}{3}n\langle \frac{1}{2}mv^2\rangle = \frac{2}{3} \text{ of the translational kinetic energy density}.
$$
- for a gas of ultra-relativistic particles $\vec{p}\cdot \vec{v} = pc$ and pressure becomes
  
  $$
  P = \frac{1}{3}n\langle pc \rangle = \frac{1}{3} \text{ of the translational kinetic energy density}.
  $$

  ## Equilibrium of a gas of non-relativistic particles
  ...