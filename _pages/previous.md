---
layout: archive
title: "Previous Research"
permalink: /previous/
author_profile: true
---

{% include base_path %}

Under construction.

* Lagrangian particle tracking in unstructured grids
* Finite volume schemes for unsteady low Mach number flows
* Eulerian formulations for disperse and dilute particle phase
* Automated mesh generation for arbitrarily embedded interfaces
* Block-based adapative mesh refinement



solves the compressible Navier-Stokes equations expressed in differential form as

$$ \mathcal{R}(U) = \frac{\partial U}{\partial t} + \nabla \cdot \bar{F}^{c}(U) - \nabla \cdot \bar{F}^{v}(U,\nabla U) - S = 0 $$

where the conservative variables are the working variables and given by

$$ U = \left{ \rho, \rho \bar{v}, \rho E \right}^T $$

$$S$$ is a generic source term, and the convective and viscous fluxes are

$$ \bar{F}^{c} = \left{ \begin{array}{c} \rho \bar{v} \ \rho \bar{v} \otimes \bar{v} + \bar{\bar{I}} p \ \rho E \bar{v} + p \bar{v} \end{array} \right} $$

and

$$ \bar{F}^{v} = \left{ \begin{array}{c} \cdot \ \bar{\bar{\tau}} \ \bar{\bar{\tau}} \cdot \bar{v} + \kappa \nabla T \end{array} \right} $$

where $$\rho$$ is the fluid density, $$\bar{v}=\left\lbrace u, v, w \right\rbrace^\mathsf{T}$$ $$\in$$ $$\mathbb{R}^3$$ is the flow speed in Cartesian system of reference, $$E$$ is the total energy per unit mass, $$p$$ is the static pressure, $$\bar{\bar{\tau}}$$ is the viscous stress tensor, $$T$$ is the temperature, $$\kappa$$ is the thermal conductivity, and $$\mu$$ is the viscosity. The viscous stress tensor can be expressed in vector notation as

$$ \bar{\bar{\tau}}= \mu \left( \nabla \bar{v} + \nabla \bar{v}^{T} \right) - \mu \frac{2}{3} \bar{\bar I} \left( \nabla \cdot \bar{v} \right) $$

Assuming a perfect gas with a ratio of specific heats $$\gamma$$ and specific gas constant $$R$$, one can close the system by determining pressure from $$p = (\gamma-1) \rho \left[ E - 0.5(\bar{v} \cdot \bar{v} ) \right]$$ and temperature from the ideal gas equation of state $$T = p/(\rho R)$$. Conductivity can be a constant, or we assume a constant Prandtl number $$Pr$$ such that the conductivity varies with viscosity as $$\kappa = \mu c_p / Pr$$.
