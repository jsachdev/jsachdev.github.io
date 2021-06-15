---
layout: archive
title: "Previous Research"
permalink: /previous/
author_profile: true
---

{% include base_path %}

## Lagrangian particle tracking in unstructured grids

Developed numerical framework for tracking particles through multi-element unstructured grids. The method implemented was based on the robust particle-localization algorithm by [Haselbacher et al.](https://doi.org/10.1016/j.jcp.2007.03.018). The implementation proved to be robust for a multi-element unstructured grid with grid-based domain decomposition. Moreover, this algorithm allowed far large particle movements and did not restrict the fluid time-step. This work was performed at Combustion Research and Flow Technology with the CRUNCH CFD code for turbomachinery applications and liquid sprays.

## Finite volume schemes for unsteady low Mach number flows

Preconditioning techniques used to alleviate numerical stiffness in steady low Mach number flows do not perform well in unsteady low Mach number regimes. The optimal preconditioning parameters for efficiency are detrimental to the spatial dissipation and result in poor accuracy. A unified flux formulation was investigated where the optimal scaling required for spatial accuracy was independent of the preconditioning required for convergence. Both upwind flux-difference and AUSM-type schemes were investigated and the use of unsteady preconditioning scaling was shown to be critical for preserving accuracy. In the flux-difference case, the formulation was based on a generalized blending of the steady and unsteady preconditioning terms. In the AUSM case, the formulation introduces two modifications to the standard AUSM+up scheme, designated as AUSM+up’ wherein the pressure dissipation is scaled using unsteady preconditioning and AUSM+u’p’ wherein both the pressure and velocity dissipation terms are scaled by the unsteady preconditioning. These flux formulations resulted in a framework valid over a broad range of flow conditions.

"Improved Flux Formulations for Unsteady Low Mach Number Flows"
Jai Sachdev, Ashvin Hosangadi and V. Sankaran
[AIAA 2012-3067](https://doi.org/10.2514/6.2012-3067)


## Eulerian formulations for disperse and dilute particle phase

Numerical methods for the solution of an Eulerian formulation of a disperse and dilute particle-phase of a gas-particle flow are capable of accurately representing expansion waves, which allow for regions of zero particles, but are problematic with compression waves. This limitation results in unphysical particle accumulation, particularly at boundaries, and excessive smearing of shear flows where the two streams have different particle concentrations. The cause of this issue was investigated by an investigation into the eigenstructure of the governing system of equations and a novel (and somewhat adhoc) multi-velocity formulation was described which can account for compression waves by splitting the particle-phase into distinct velocity families which are transported separately. Switching of the particle families at solid boundaries and due to momentum transfer with the gas-phase was conducted in a manner that enforces conservation of mass, momentum, and energy.

"Numerical Solution Scheme for Inert, Disperse, and Dilute Gas-Particle Flows"
J.S. Sachdev, C.P.T. Groth and J.J. Gottlieb
[Int. J. Maltier. Flow 33, 282 (2007)](10.1016/j.ijmultiphaseflow.2006.09.001)


## Automated mesh generation for arbitrarily embedded interfaces

"Application of Gaussian Moment Closure to Microscale Flows with Moving Embedded Boundaries"
J.G. McDonald, J.S. Sachdev & C.P.T. Groth, AIAA J. 52, 1839 (2014)

## Block-based adaptive mesh refinement



