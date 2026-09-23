+++
title = "Ferrite.jl Conference 2026"
hascode = false
hasmath = false
+++

# FerriteCon 2026
FerriteCon 2026 will take place at the [Technische Universität Braunschweig](https://www.tu-braunschweig.de/en/) (TU Braunschweig) in Braunschweig, Germany, on 24 September 2026.

## Ferrite.jl User & Developer Conference 2026
[Ferrite.jl](https://ferrite-fem.github.io/Ferrite.jl/stable/) is an open-source finite element package written in the [Julia programming
language](https://julialang.org/). On Thursday the 24th of September 2026, we will host the fifth annual Ferrite.jl user and developer conference at TU Braunschweig.

The conference aims to improve existing and find new, technical and scientific collaborations among Ferrite.jl users and developers, as well as to discuss how the package can be further developed in the future. The conference will consist of both beginner-friendly and advanced presentations on Ferrite.jl and of current research using Ferrite.jl.

## Schedule
The conference will take place at the [Institute for Applied Mechanics (Pockelsstraße 3, 38106 Braunschweig), Room 0017 (ground floor)](https://maps.app.goo.gl/owZjbXpcSwwAZmbU8).

Click on the titles with grey background to expand the abstract.

| Time          | Activity                                                            |
|---------------|---------------------------------------------------------------------|
| 09:00 – 09:25 | **Welcome coffee** |
| 09:25 – 09:30 | **Opening and introduction** |
| 09:30 – 10:15 | **Introduction to Ferrite.jl**\\ *Knut Andreas Meyer*, Chalmers University of Technology |
| 10:15 – 11:00 | \collaps{**_Keynote_**\\**Makie goes full GPU**\\*Simon Danisch*, Author of Makie}{In this talk we present Mantle, Makie's new unified GPU platform, which allows to run graphics, hardware-accelerated ray tracing, and compute on all platforms (macOS, Windows, Linux, all GPU vendors). Mantle will be used for the upcoming new Makie backend, introducing better real-time rendering and ray tracing, with the option to use Julia for arbitrary pre- and post-processing of data, including FEM meshes.} |
| 11:00 – 11:15 | Coffee break |
| 11:15 – 11:35 | \collaps{**Upgrading a decade-old Ferrite code to modern Ferrite**\\ *Kristoffer Carlsson*, JuliaHub}{About ten years ago I wrote the finite element code behind two papers on gradient-extended crystal plasticity (Carlsson et al., *Comput. Mech.* 2017; *Int. J. Numer. Methods Eng.* 2019) in Ferrite (which was then still called JuAFEM). At the time, the package covered only the most basic FE utilities: fields could not live on a subset of the mesh, there was no constraint handling, and surrounding tooling like mesh readers and interface elements did not exist. Many of the things I needed for the papers had to be written by hand, and I often had to use Ferrite's internals.

Ferrite has since gotten a significant amount of development, and many of the gaps it had back then are now filled. This talk walks through porting the old code to the current Ferrite release: what could be deleted, what was replaced by built-in functionality, and what still needs a workaround. The question we'll answer is whether Ferrite has reached "feature nirvana", where a full research code like this can be written in "pure" Ferrite without any hacks or workarounds.

References:\
K. Carlsson, K. Runesson, F. Larsson, M. Ekh. A comparison of the primal and semi-dual variational formats of gradient-extended crystal inelasticity. *Comput. Mech.* 60, 531–548 (2017). https://doi.org/10.1007/s00466-017-1419-y\
K. Carlsson, M. Ekh, F. Larsson, K. Runesson. A comparison of computational formats of gradient-extended crystal viscoplasticity in the context of selective homogenization. *Int. J. Numer. Methods Eng.* 119, 281–304 (2019). https://doi.org/10.1002/nme.6050} |
| 11:35 – 11:55 | \collaps{**Ferrite.jl since 1.0: two years of non-breaking growth**\\*Fredrik Ekre*, JuliaHub}{Ferrite.jl 1.0 was released two years ago with the promise of a stable API. This talk gives an overview of what has been added to Ferrite and its companion packages since then without breaking that promise, and an outlook on what is currently being worked on.} |
| 11:55 – 12:15 | \collaps{**High-Order Accuracy Meets High Performance: Spectral Elements in Ferrite.jl**\\*Shadi Affan*, RPTU Kaiserslautern-Landau}{This talk presents a native implementation of the two-dimensional spectral element method (SEM) for linear elasticity in Ferrite.jl, extending the existing workflow with Gauss-Lobatto-Legendre quadrature, high-order interpolation, and dedicated spectral elements. The implementation is fully integrated into Ferrite.jl and validated using benchmark problems with analytical reference solutions. Two performance optimizations – a cross-pattern assembly scheme and static condensation – exploit characteristic properties of SEM to significantly reduce assembly and solution times while preserving numerical accuracy. The results demonstrate that Ferrite.jl provides an efficient and flexible framework for high-order finite element methods and future extensions toward three-dimensional and shell formulations.} |
| 12:15 – 13:15 | **Lunch** |
| 13:15 – 13:35 | \collaps{🌐 **Isogeometric Analysis in Julia: FerriteIGA.jl and the Ferrite Ecosystem**\\*Sreeram Shankar*, University of Texas}{Isogeometric Analysis (IGA) modifies the finite element approximation space with spline-based basis functions, providing high smoothness basis and the potential for synergy between geometric representation (CAD) and the numerical discretization of mechanical problems. These properties make IGA particularly attractive for high-order approximations, structural mechanics, and problems requiring elevated smoothness, while introducing mathematical and computational structures that differ from those encountered in conventional finite element implementations. This talk introduces the mathematical foundations of IGA through its relationship to classical finite elements, emphasizing the role of the spline approximation space, its differences from the classical method, and specific mathematical properties of IGA. From this perspective, I will present FerriteIGA.jl and discuss ongoing development of the package along with the potential for future expansion and broader integration within the Ferrite ecosystem, bringing enhanced IGA capabilities to the Julia scientific computing community.} |
| 13:35 – 13:55 | \collaps{🌐 **From Ferrite Codes to Clinical Digital Twins**\\*Amin Alibakhshi*, University of A Coruña}{The collaboration between clinicians and mechanical researchers is growing as efforts to computerize disease progression and improve treatment continue to expand. Computational biomechanics and scientific programming are the main pillars of this field. This work demonstrates the potential of the Ferrite package for applications in biomechanics and the development of Clinical Digital Twins in three illustrative applications: breast deformation, benign prostate growth, and bone implants.} |
| 13:55 – 14:15 | \collaps{🌐 **FerriteShells.jl: A general shell assembler for Ferrite.jl**\\*Marin Lauber* and *Viola Bini*, Delft University of Technology}{Shells are both natural and engineered structures that exhibit rich mechanical responses;from bending to membrane-dominated regimes with the associated buckling and wrinkling.Their modeling is therefore an important, and yet complex, field of engineering. We presenta companion library for the Ferrite ecosystem that provides specialized shell assemblyprocedures that enables modeling thick and thin non-linear shells. Our formulationleverages Ferrite’s existing infrastructure and the type dispatch of the Julia programminglanguage to implement Kirchhoff–Love and Reissner–Mindlin shells. With various linear andnon-linear shell examples, we demonstrate that the library is robust and requires onlyminimal changes to the standard Ferrite setup to model shells.} |
| 14:15 – 14:30 | Coffee break |
| 14:30 – 14:50 | \collaps{**Benchmarking Sparse Direct and Preconditioned Iterative Solvers for Elliptic PDEs**\\*Marieke Osewold*, Weierstrass Institute}{Discretizations of elliptic PDEs lead to large sparse linear systems whose solution can dominate the computational cost. This talk benchmarks sparse direct solvers accessed through LinearSolve.jl against iterative methods from Krylov.jl with incomplete LU and algebraic multigrid preconditioners for symmetric and nonsymmetric problems. Building on Cartesian-grid model problems from my master’s thesis, the benchmarks will be extended to finite element matrices relevant to Ferrite.jl applications.} |
| 14:50 – 15:10 | \collaps{**Unmatching Periodic Boundary Data: How We Handle It**\\*Patrick Jaap*, Weierstrass Institute}{This talk addresses the following task: given a very complex grid, periodic boundary conditions must be imposed on the solution.This task is straightforward as long as the periodic interfaces align properly.To address mismatched interfaces, we initially attempted a straightforward brute-force interpolation strategy.However, this approach led to several performance bottlenecks.Therefore, we developed an efficient, thread-parallel lookup algorithm capable of handling a large number of DOFs across the periodic interfaces.We will present the details of this approach, along with two strategies for incorporating the assembled data into the global system matrix.Although this method was implemented within our PDE library ExtendableFEM.jl, its underlying concept is purely algebraic and can be readily adapted for Ferrite.jl.We also present analytical results to quantify the accuracy loss introduced by the interpolation for three-dimensional elasticity problem.} |
| 15:10 – 15:30 | \collaps{**Modelling of cast aluminium and ductile phase field modelling**\\*Mélanie Fournier* and *Jacob Gunnarsson*, Chalmers University of Technology}{We are working on problems involving damage modelling and homogenization of multiphase cast aluminium and pearlite with multiple fields. In this talk, we highlight how we use Ferrite.jl and other packages such as FerriteAssembly.jl, MaterialModelsBase.jl and MechanicalMaterialModels.jl for that purpose.} |
| 15:30 – 15:50 | \collaps{**An application of optimal boundary control in Ferrite.jl**\\*Phil Kreutzheide*, Chalmers University of Technology}{When we model systems with PDEs, we are generally interested in some output quantity. More specifically, we are interested in how that output quantity depends on some input quantity whose value we want to determine. A naive approach is to repeatedly solve the PDE for a chosen set of input parameters and study the output data until we are satisfied with the result. For problems involving nonlinear PDEs or large parameter ranges, however, this quickly becomes prohibitive. Optimal control of PDEs removes the guesswork by posing an optimization problem instead. As in "conventional" optimization, optimal control consists of an objective that measures the deviation from a desired state, subject to some constraints – in this case, a system of PDEs. In this talk, I will go through an application of optimal boundary control of incompressible Navier–Stokes, and its solution via a direct approach.} |
| 15:50 – 17:00 | Hackathon & open discussion |
| 19:00 | **Social dinner**\\ *The registration for the dinner has passed.* Note that the dinner will be at your own expense. |

You can also have a look at the program of previous editions of FerriteCon:
- [FerriteCon 2022 (Braunschweig, Germany)](/2022/)
- [FerriteCon 2023 (Bochum, Germany)](/2023/)
- [FerriteCon 2024 (Gothenburg, Sweden)](/2024/)
- [FerriteCon 2025 (Lyngby, Denmark)](/2025/)

## Webex meeting information
The conference is live-streamed via Webex, which can be accessed [here](https://tu-braunschweig.webex.com/tu-braunschweig-en/j.php?MTID=m7523c849931045f794abf26a3f57ea03). Otherwise, the meeting room can be accessed using the information below:

Meeting number:
2782 639 8610

Meeting password:
afKW2Yv65tx

## Speaker information
Regular talks are 15 minutes + 5 minutes for questions. We will live-stream the conference via Webex and record the talks, in order to upload them on the [JuliaLang YouTube channel](https://www.youtube.com/c/TheJuliaLanguage). If you do not consent to this, please contact the organizers, and we will exclude your talk from the uploaded videos.

You can present from your own laptop — in that case, please make sure you can share your slides in a Webex meeting so that the recording includes them. The room is equipped with video/audio equipment, and we will be available in the conference room from 8:30 on the day so you can test your connection.

## Public transport
If you need to use public transport in Braunschweig, you can buy single tickets from the driver or  more conveniently via the [Meine BSVG](https://www.bsvg.net/) or [VRB Fahrinfo & Tickets](https://www.vrb-online.de/en/service/app) apps. In addition, [Fairtiq](https://fairtiq.com/en/vrb), a check-in / check-out app, is also available. For trains to Braunschweig, please use [Deutsche Bahn (DB Navigator)](https://www.bahn.de/) for schedules and tickets.

## Conference topics
*Please note that the abstract registration deadline has passed.*

If you have experience with Ferrite.jl we encourage you to contribute to the conference by giving a presentation. Here are some suggested topics that would fit well:

* Present your research and how you use Ferrite.jl (take this opportunity to discuss implementation aspects which are normally not discussed much on regular scientific conferences!)
* Present interesting synergies between Ferrite.jl and the rest of the Julia package ecosystem
* Present how you use Ferrite.jl for teaching or for student projects
* Describe what you would like to use Ferrite.jl for, and the reasons why you are currently using something else.
* Present ideas for future Ferrite.jl improvements and describe how you would like to incorporate it (perhaps describe prior art from other software packages)

If you have another topic you would like to discuss, please feel free to do so, as long as you can relate it to Ferrite.jl!

<!-- The conference and meetup is free of charge, but registration is necessary. To register as a speaker, please send an email containing a title and a brief abstract (~100 words, 3-4 sentences) to Quoc Tuan La ([quoc-tuan.la@tu-braunschweig.de](mailto:quoc-tuan.la@tu-braunschweig.de)) at the latest the **28th of August (2026-08-28)**. If you want to attend without presenting, please register as soon as possible, but latest the **18th of September (2026-09-18)**. -->

## Registration
*Please note that the participant registration deadline has passed.*

Registration is open until **18th of September (2026-09-18)**. To register as a participant, please send an email to Mischa Blaszczyk ([mischa.blaszczyk@tu-braunschweig.de](mailto:mischa.blaszczyk@tu-braunschweig.de)).

There will also be a social dinner at your own expense. If you are interested in attending, please indicate this in your email, along with any dietary requirements.


## Contact
If you have any questions, please don't hesitate to ask by sending an email to
the organizers:

* Quoc Tuan La ([quoc-tuan.la@tu-braunschweig.de](mailto:quoc-tuan.la@tu-braunschweig.de))
* Mischa Blaszczyk ([mischa.blaszczyk@tu-braunschweig.de](mailto:mischa.blaszczyk@tu-braunschweig.de))
