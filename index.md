+++
title = "Ferrite.jl Conference 2023"
hascode = false
hasmath = false
+++

# Ferrite.jl User & Developer Conference 2023

[Ferrite.jl](https://github.com/Ferrite-FEM/Ferrite.jl) is an open-source
finite element package written in the [Julia programming
language](https://julialang.org/). On the 6th of October 2023 we will host another
Ferrite.jl user and developer conference at Ruhr University Bochum.

The conference aims to improve existing, and find new, scientific
collaborations among Ferrite.jl users and developers, as well as to discuss
how the package can be further developed in the future.

The [program](#program) of the conference will consist of presentations of current research
using Ferrite.jl, followed by a hackathon where participants can discuss and
solve current challenges with the library.

The program will be similar to the one from last year, please have a look at
[Ferrite.jl User & Developer Conference 2022](2022/).

## Target audience

If you have used, contributed to, or are just curious about Ferrite.jl we
encourage you to participate.

If you have experience with Ferrite.jl we also encourage you to contribute to
the conference by giving a presentation. Here are some suggested topics that
would fit well:

 - Present your research and how you use Ferrite.jl (take this opportunity to
   discuss implementation aspects which are normally not discussed much on
   regular scientific conferences!)
 - Present interesting synergies between Ferrite.jl and the rest of the Julia
   package ecosystem
 - Present how you use Ferrite.jl for teaching or for student projects
 - Describe what you would like to use Ferrite.jl for, and the reasons why you
   are currently using something else.
 - Present ideas for future Ferrite.jl improvements and describe how you would
   like to incorporate it (perhaps describe prior art from other software
   packages)

If you have another topic you would like to discuss, please feel free to do so,
as long as you can relate it to Ferrite.jl!


## Time and location

The conference will be held at at [Ruhr University Bochum]
(https://www.ruhr-uni-bochum.de/en) at the [Chair of Continuum Mechanics]
(http://www.lkm.rub.de/)
(Universitätsstraße 150, 44801 Bochum, Germany)
on October 6th, starting at 9:30.
All presentations will be held in the building IC, floor 03, in the rooms 604 & 606 (IC 03/604 and IC 03/606).
Please note that the floor 03 is a basement floor and a different floor than floor number 3.
A plan for the campus as a PDF can be found [here](https://www.ruhr-uni-bochum.de/anreise/download/campusplan.pdf).

If you would like to attend online via Zoom, please [follow this link](https://ruhr-uni-bochum.zoom.us/j/61775211575?pwd=UTBhVHdwN1hCQ3NSOXAzaTNIMjJ1UT09)

## Program

A preliminary program is given below, more details will follow after registration.

| Time        | Activity                                                                   |
|-------------|----------------------------------------------------------------------------|
| 09:30-10:00 | **Welcome coffee**
| 10:00-10:05 | **Opening and introduction**
| 10:05-11:00 | **Keynote (online)\\ Julia for scientific high-performance computing: opportunities and challenges**\\ *[Michael Schlottke-Lakemper](https://lakemper.eu/)*\\ The Julia programming language aims to provide a modern approach to scientific computing and was designed with high-performance computing (HPC) in mind. As a consequence, a growing number of research groups are considering Julia as their language of choice for creating the next generation of computational fluid dynamics or structure mechanics codes. In this talk, we will thus discuss benefits of using Julia for such classical HPC workloads, and examine where challenges remain. For some practical insights, we will take a closer look at [Trixi.jl](https://github.com/trixi-framework/Trixi.jl), a numerical simulation framework for hyperbolic conservation laws that has been shown to scale efficiently to more than 50,000 MPI ranks, and share some of the lessons learned during its development.
| 11:00-11:25 | **One year of Ferrite.jl development**, *Fredrik Ekre*\\I will present the progress in Ferrite.jl since last years conference. I will give an overview of the new features that are available and discuss some of the internal and external changes to the code base.\\Presentation: [One year of Ferrite development.pdf](/assets/2023/One_year_of_Ferrite_development.pdf)
| 11:25-11:50 | **Recent applications of Ferrite.jl at the IKM**, *Dustin Jantos, et al.*\\A main research topic at the IKM (Institute of Continuum Mechanics, Leibniz University Hannover) is the modelling and simulation of complex material behavior. For this purpose, we make use of Ferrite.jl as the FEM toolbox. In this talk, we present examples including uncertainty quantifications, topology optimization and damage modeling. We show numerical implementations and results. In doing so, we present applications and point out expansion possibilities of Ferrite.jl. \\Presentation: [Recent_applications_of_Ferrite_at_the_iKM.pdf](/_assets/2023/Recent_applications_of_Ferrite_at_the_iKM.pdf)
| 11:50-13:00 | **Lunch break**
| 13:00-13:25 | **Immersed Methods with Ferrite**, *Elias Börjesson*\\In this presentation, I will discuss my implementation of immersed methods in Ferrite.jl. The core idea of immersed methods is to use simple un-fitted (voxel-like) meshes to discretize the unknown fields, while the geometry is captured with specially generated quadrature rules. The benefit of immersed methods is that the discretization (or meshing) procedure can be made automatic, even for very complex geometries. As an application, I will show how I have used immersed methods for modelling of meso-scale structures of fibre composites.
| 13:25-13:50 | **Discontinuous Galerkin Methods Infrastructure: A GSoC Project**, *Abdulaziz Hamid*\\Presenting the process of developing infrastructure for discontinuous Galerkin (DG) methods as part of the Google Summer of Code (GSoC) program. The project focused on implementing and optimizing methods to resolve the interface integral terms, which then addresses other issues such as syncing the quadrature points on both sides of the interface and adding cross-element coupling to sparsity patterns. Future work includes having a unified method to work with mixed grids and interfacing DG with AMR.\\Presentation: [Discontinuous_Galerkin_Methods_Infrastructure_GSoC.pdf](/assets/2023/Discontinuous_Galerkin_Methods_Infrastructure_GSoC.pdf)
| 13:50-14:15 | **Raising MixedDofHandler – about full support for mixed grids**, *Kim Louisa Auth*\\Did you know Ferrite has supported mixed (or hybrid) grids with several different cell types ever since 2019? This feature has been slightly hidden in the code base as `MixedDofHandler` since then. Over time, it matured and got battle tested in cohesive element research. During the past year, it went through a redesign, got a major performance-boost and a shiny new syntax. Grown up like this, it went out to conquer the (Ferrite-) world and became the standard `DofHandler` in April 2023. But chances are you didn’t even notice this since the change was non-breaking for old-`DofHandler` users!\\In this talk I will present the new syntax for constructing problems on mixed grids and with several subdomains. An example for using Ferrite on a grid consisting of both triangular and quadrilateral elements will be shown, including advice on how to write performant code for the global assembly procedure. Additionally, there will be a (short) discussion of some of the design decisions for the new `SubDofHandler` and the underlying internals. In connection with the talk, a new tutorial and a new how-to guide on mixed grids are planned.
| 14:15-14:40 | **How simple should using Ferrite get?**, *Knut Andreas Meyer*\\At FerriteCon2022, discussions on how to reduce boilerplate user code took place. One year later, the packages [`FerriteAssembly.jl`](https://knutam.github.io/FerriteAssembly.jl/), [`FESolvers.jl`](https://knutam.github.io/FESolvers.jl/), and [`FerriteProblems.jl`](https://knutam.github.io/FerriteProblems.jl/), aim to do just that. While these packages offer several advantages for both new and experienced users, the convenience also reduces flexibility. The talk will first introduce the ecosystem built on top of Ferrite.jl with some examples from research codes, showing how simple it can get. Thereafter, the focus shifts to the limitations and challenges of using such packages before concluding with a discussion on when to use, and not to use, such packages.\\Presentation: [How simple should using Ferrite.jl get?](/assets/2023/Meyer_FerriteCon2023.pdf)
| 14:40-15:00 | **Coffee and snacks**
| 15:00-15:25 | **Julia implementation of P4est datastructures tailored for Ferrite.jl**, *Maximilian Köhler*\\ In this talk I will briefly introduce the concepts of linear quad/octree adaptivity and how it can be realized in Julia without C dependencies. I will go through the main operations and how the status of the implementation is with respect to basic grid operations. The implementation uses the very optimized and stripped down datastructure proposals of [p4est](https://ins.uni-bonn.de/media/public/publication-media/BursteddeWilcoxGhattas11.pdf?pk=583). There, a second coordinate system with an a priori fixed length is used. This allows to build a lazy forest datastructure that requires less communication and is ready for scalability. However, the talk is limited to the sequential case. \\ Presentation: [P4est Datastructures for Ferrite.jl](https://github.com/koehlerson/FerriteCon23/blob/main/slides.pdf)
| 15:25-15:50 | **PDE based control using Ferrite**, *Krishna Bhogaonker*\\PDE based control is a broad topics with applications across industry and academic research. The JuliaSimControl package consolidates a number of PDE based control methods into a single library. However, the package is still relatively new and presently is only tested with the MethodOfLines.jl package which supports finite differences for PDE based control. I would like to demonstrate a prototype for using JuliaSimControl with Ferrite, thus enabling Ferrite users to work on PDE based control problems.
| 15:50-16:10 | **Thunderbolt.jl - A Fast and Modular Cardiac Multiphysics Simulation Framework on top of Ferrite.jl**, *Dennis Ogiermann*\\Computational cardiology has gained wide attention over the last decade as a candidate to gain a better understanding of the heart function during healthy and diseases conditions, as well as being a tool to improve clinical care through personalized simulations. However, existing simulation frameworks focus either on limited model classes or do not come with an easily hackable solver backend. To overcome this issue I developed [Thunderbolt.jl](https://github.com/termi-official/Thunderbolt.jl), a framework provides an easy to use and modular modeling frontend in tandem with a fully modular solver backend. One great challenge in cardiac multiphysics is to develop energy efficient approaches. Hence the framework is restrited to shared memory environments utilizing CPU and GPU in tandem for the simulations. In this presentation I will give an overview on the architecture of the framework and the next steps.
| 16:10-16:15 | **Progress Report: Ferrite's HPC Layer**, *Dennis Ogiermann*\\In this presentation I will summarize the recent advances and open issues of the HPC layer development. Two major advances took place since the FerriteCon 2022. First, the distributed memory assembly infrastructure has been moved into its own package [FerriteDistributed.jl](https://github.com/Ferrite-FEM/FerriteDistributed.jl/). This package contains helpers, grids and dof handlers to manage distributed assembly in different distributed sparse matrix formats. Second, there is an ongoing development of an infrastructure for GPU-based methods, which gained lots of attention over the recent years due to superior performance is several use-cases.
| 16:15-18:30 | [**Hackathon**](https://en.wikipedia.org/wiki/Hackathon)
| 19:15       | **Dinner at [Hans im Glück](https://hansimglueck-burgergrill.de/en/burger-restaurant/bochum-kortumstrasse/)**

Coffee and snacks for the morning and afternoon will be provided (for free).

The dinner will be at some restaurant where we can order drinks and food.
More information to come.

## Presentations

In the spirit of last year we allocate 20+5 minutes per presentation.
All presenters have to use their own laptop and share their slides via Zoom.
So, please keep your Laptop's Zoom installation up to date.
All presentations will be recorded and uploaded to YouTube.
If you don't feel comfortable with this, please send a short notice, such that we can delete the recording.


## Registration and abstract submission

The conference is free of charge, but registration is necessary. To register,
please send an email to Maximilian Köhler
([maximilian.koehler@ruhr-uni-bochum.de](mailto:maximilian.koehler@ruhr-uni-bochum.de)) at the latest
the **31th of August (2023-08-31)**. If you also want to contribute with a presentation, include a title and a brief abstract (~100 words, 3-4 sentences).

## Contact

If you have any questions, please don't hesitate to ask by sending an email to
the organizers:

- Maximilian Köhler [maximilian.koehler@ruhr-uni-bochum.de](mailto:maximilian.koehler@ruhr-uni-bochum.de)
- Fredrik Ekre [f.ekre@tu-braunschweig.de](mailto:f.ekre@tu-braunschweig.de)
