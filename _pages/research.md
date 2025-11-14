---
layout: archive
title: "Research Interests Past and Present"
permalink: /research/
author_profile: true
---

{% include base_path %}

## FUSION FM

Working toward an AI foundation model for magnetic confinement fusion devices. This is a part of a multi-lab collaboration for rapidly developing and deploying AI agents and other tools for accelerating fusion research and engineering. Data curation is paramount for any AI/ML project, including data from experiments and simluations. Towards this end, developmant of methods, procedures, and codes for extracting, transforming, and loading data with appropriate metadata and provenance to be AI-ready tools are being undertaken.

## T3D

[T3D](https://t3d.readthedocs.io/en/latest/index.html) (or Trinity3D) is a transport solver for modeling macro-scale profile evolution in fusion plasmas (tokamaks and stellarators).

- [J.S. Sachdev et al APS DPP PP12.00047](https://meetings.aps.org/Meeting/DPP24/Session/PP12.47)
- [N. Mandell et al APS DPP UO06.00011](https://meetings.aps.org/Meeting/DPP23/Session/UO06.11)
 

## NSTX-U Operational Software

Development of web-based tools for interacting with the NSTX and NSTX-U experiment logbook and viewing/plotting/analyzing experiment shot data. Web-based experimental logbook created using python and Flask and developed in collaboration with NSTX-U experimentalists. This utility offers a modern and much more effecient method for interacting with the experiment logbook. The physics viewer was created using python with Dash and Plotly to provide a quick but comprehensive look experiment shot data through a web-based application. 


## TRANSP

[TRANSP](https://transp.pppl.gov/) is a time-dependent 1.5D MHD equilibrium and plasma transport solver for modeling tokamak fusion devices. This software is used by hundreds of scientists at several research centers world-wide for interpreting experimental results, predictive analysis, experimental campaign planning, and rapid between shot analysis. The capabilities of the code has grown significantly over 40+ years of development, particularly with respect to the physics models. Maintaining and extending physics models was pursued in coordination with a major overhauling of the code base.

- [A.Y. Pankin et al, Computer Physics Communications 2024](https://www.sciencedirect.com/science/article/pii/S0010465525001134)
- [TRANSP: doi:10.11578/dc.20180627.4](https://www.osti.gov/biblio/1489900-transp)


## Best practices for scientific computing

Continuous testing, continuous deployment, automation, containerization, devops, ... for research software engineering.

- J.S. Sachdev NLIT 2024: A Survey of Sustainable Scientific Software Development Practices at PPPL
- [J.S. Sachdev et al SIAM CSE19 Minisymposterium: Software Productivity and Sustainability for CSE and Data Science](https://figshare.com/articles/poster/Modernizing_the_Scientific_Software_Approach_for_the_Fusion_Analysis_Code_TRANSP/7758305)


## Pellet ablation models

Implementation, testing, and application of pellet ablation models using TRANSP and PELLET (a pellet ablation code from ORNL/GA). Injection of pellets and shattered pellets are being studied as possible mechanisms for fueling of magnetic fusion devices as well as for control of disruptions and instabilities.

[R. Raman et al 2020 Nucl. Fusion 60 036014](https://iopscience.iop.org/article/10.1088/1741-4326/ab686f)


## Lagrangian particle tracking in unstructured grids

Developed numerical framework for tracking particles through multi-element unstructured grids. The method implemented was based on the robust particle-localization algorithm by [Haselbacher et al.](https://doi.org/10.1016/j.jcp.2007.03.018). The implementation proved to be robust for a multi-element unstructured grid with grid-based domain decomposition. Moreover, this algorithm allowed far large particle movements and did not restrict the fluid time-step. This work was performed at Combustion Research and Flow Technology with the CRUNCH CFD code for turbomachinery applications and liquid sprays.


## Finite volume schemes for unsteady low Mach number flows

Preconditioning techniques used to alleviate numerical stiffness in steady low Mach number flows do not perform well in unsteady low Mach number regimes. The optimal preconditioning parameters for efficiency are detrimental to the spatial dissipation and result in poor accuracy. A unified flux formulation was investigated where the optimal scaling required for spatial accuracy was independent of the preconditioning required for convergence. Both upwind flux-difference and AUSM-type schemes were investigated and the use of unsteady preconditioning scaling was shown to be critical for preserving accuracy. In the flux-difference case, the formulation was based on a generalized blending of the steady and unsteady preconditioning terms. In the AUSM case, the formulation introduces two modifications to the standard AUSM+up scheme, designated as AUSM+up’ wherein the pressure dissipation is scaled using unsteady preconditioning and AUSM+u’p’ wherein both the pressure and velocity dissipation terms are scaled by the unsteady preconditioning. These flux formulations resulted in a framework valid over a broad range of flow conditions.

[Jai Sachdev, Ashvin Hosangadi and V. Sankaran AIAA 2012-3067](https://doi.org/10.2514/6.2012-3067)


## CFD simulations of NASA rocket launch systems and components

CFD studies performed on failure modes and risk assessments of NASA rocket launch vehicle systems and components, such as: propellant tank common bulkhead failures, analysis of flame deflector spray nozzles in rocket engine test stands, and failure analysis of pyrotechnically actuated valves.

- [Jai Sachdev, Ashvin Hosangadi, Nateri Madavan and Scott Lawrence AIAA 2009-5150](https://doi.org/10.2514/6.2009-5150)
- [Jai Sachdev, Vineet Ahuja, Ashvin Hosangadi and Daniel Allgood AIAA 2010-6972](https://doi.org/10.2514/6.2010-6972)
- [Jai Sachdev, Ashvin Hosangadi, James Chenoweth, Regor Saulsberry and Stephen McDougle AIAA-2012-3799](https://doi.org/10.2514/6.2012-3799)

![image](https://github.com/jsachdev/jsachdev.github.io/assets/10472230/67ce8120-dabf-4982-8564-c24130526ab3)
![image](https://github.com/jsachdev/jsachdev.github.io/assets/10472230/0883b1fb-b885-4c2d-812f-36dbbd18a4c2)


## Eulerian formulations for disperse and dilute particle phase

Numerical methods for the solution of an Eulerian formulation of a disperse and dilute particle-phase of a gas-particle flow are capable of accurately representing expansion waves, which allow for regions of zero particles, but are problematic with compression waves. This limitation results in unphysical particle accumulation, particularly at boundaries, and excessive smearing of shear flows where the two streams have different particle concentrations. The cause of this issue was investigated by an investigation into the eigenstructure of the governing system of equations and a novel (and somewhat adhoc) multi-velocity formulation was described which can account for compression waves by splitting the particle-phase into distinct velocity families which are transported separately. Switching of the particle families at solid boundaries and due to momentum transfer with the gas-phase was conducted in a manner that enforces conservation of mass, momentum, and energy.

[J.S. Sachdev, C.P.T. Groth and J.J. Gottlieb Int. J. Multiphase Flow 33, 282 (2007)](10.1016/j.ijmultiphaseflow.2006.09.001)

![jets_010](https://user-images.githubusercontent.com/10472230/122473243-927ef980-cf8f-11eb-8bf8-d3aa479a45b9.jpg)

Contours of the particle concentration for crossing particle jets into a quiescent gas. Results for a single-velocity formulation on the left and a multi-velocity formulation on the right. The multi-velocity formulation shows the expected behavior for a disperse and dilute particle-phase.


## Mesh adaptation and refinement

Development of a block-based adaptive mesh refinement (AMR) scheme for multi-block body-fitted structured meshes with automatic solution-directed mesh adaptation according to physics-based refinement criteria. Efficient and scalable parallel implementation achieved on distributed memory multi-processor architectures by evenly allotting the blocks to the available processors. In addition, mesh adjustment scheme was devised in which a body-fitted multi-block mesh is locally adjusted to embedded boundaries that are not aligned with the mesh. This scheme allowed for quick and robust parallel mesh generation involving complex embedded boundaries. The viability of this scheme was demonstrated for stationary and moving embedded boundaries. These algorithms were applied to problems involving microscale flows and multi-phase core flows in solid propellant rocket motor flows.

- [J.G. McDonald, J.S. Sachdev, and C.P.T. Groth AIAA J. 52, 1839 (2014)](https://arc.aiaa.org/doi/10.2514/1.J052576)
- [J.S. Sachdev and C.P.T. Groth Commun. Comput. Phys. 2 (2007), pp. 1095-1124](https://global-sci.org/index.php/cicp/article/view/5492)
- [J. Sachdev, C. Groth, and J. Gottlieb AIAA 2005-5334](https://doi.org/10.2514/6.2005-5334)
- [J. Sachdev, C. Groth, and J. Gottlieb Int. J. Comput. Fluid Dyn.](https://www.tandfonline.com/doi/abs/10.1080/10618560410001729135)

![image](https://user-images.githubusercontent.com/10472230/122476398-1935d580-cf94-11eb-9d8b-e84f1c4190c9.png)
![image](https://user-images.githubusercontent.com/10472230/122476435-2b177880-cf94-11eb-8a96-0a565482cf15.png)

Block-based adaptive mesh refinement of a supersonic flow over a bump with $$M_\infty = 2$$. Block boundaries shown in figures with each block containing 32 by 32 cells.

![naca0012](https://user-images.githubusercontent.com/10472230/122145966-2df35b80-ce24-11eb-8acf-54b8511e819d.gif)

## Solid Propellant Rocket Motors

Numerical schemes applied to internal solid propellant rocket motor flows.

- [J. Sachdev, C. Groth, and J. Gottlieb AIAA 2005-5334](https://doi.org/10.2514/6.2005-5334)
- [J. Sachdev, C. Groth, and J. Gottlieb Int. J. Comput. Fluid Dyn.](https://www.tandfonline.com/doi/abs/10.1080/10618560410001729135)
