+++
title = "Ferrite.jl Conference"
hascode = false
hasmath = false
+++

# Ferrite.jl User & Developer Conference

[Ferrite.jl](https://github.com/Ferrite-FEM/Ferrite.jl) is an open-source
finite element package written in the [Julia programming
language](https://julialang.org/). On the 26th of September 2022 we will host a
Ferrite.jl user and developer conference at TU Braunschweig.

The conference aims to improve existing, and find new, scientific
collaborations among Ferrite.jl users and developers, as well as to discuss
how the package can be further developed in the future.

The [program](#program) of the conference will consist of presentations of current research
using Ferrite.jl, followed by a hackathon where participants can discuss and
solve current challenges with the library.

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
 - Describe what you would like to use Ferrite.jl for, and the reasons why you
   are currently using something else.
 - Present ideas for future Ferrite.jl improvements and describe how you would
   like to incorporate it (perhaps describe prior art from other software
   packages)

If you have another topic you would like to discuss, please feel free to do so,
as long as you can relate it to Ferrite.jl!


## Time and location

The conference will be held at at [TU
Braunschweig](https://www.tu-braunschweig.de/en/) at the [Institute
of Applied Mechanics](https://www.tu-braunschweig.de/en/iam) 
(Pockelsstraße 3, 38106 Braunschweig, Germany)
on September 26th, starting at 9:30. 

## Program

| Time        | Activity                                                                   |
|-------------|----------------------------------------------------------------------------|
| 09:30-10:00 | **Welcome coffee**
| 10:00-10:05 | **Opening and information about the day**
| 10:05-10:30 | **Introduction to Ferrite.jl**, *Fredrik Ekre*\\In this talk I will give an overview of Ferrite.jl. I will discuss current capabilities and features and also discuss some of the currently missing pieces.\\ Presentation: [Introduction to Ferrite.jl](/assets/IntroductionFerrite.pdf)
| 10:30-10:55 | **Cohesive elements -- a showcase for mixed grids and customized interpolations**, *Kim Louisa Auth*\\The talk shows how to define cohesive elements by subtyping the interpolation and using a custom `Values` object (well integrated into Ferrite since [Ferrite.jl#404](https://github.com/Ferrite-FEM/Ferrite.jl/pull/404)). The capabilities of Ferrite in terms of mixed grids are discussed on the example of using 2D triangular bulk elements together with quadrilateral cohesive elements. Rounding up, a very brief overview of my research project, that uses cohesive elements in a multi-physics framework with a concentration field living solely on the cohesive zones (i.e. a subdomain), is given. \\ Code: [FerriteCon2022.jl](https://github.com/kimauth/FerriteCon2022.jl) and [FerriteCohesiveZones.jl](https://github.com/kimauth/FerriteCohesiveZones.jl)
| 10:55-11:20 | **FerriteViz.jl: Friendship ended with ParaView, now Makie.jl is my best friend**, *Maximilian Köhler*\\Makie.jl offers the unique possibility to construct publication-quality plots as vector graphics by means of the CairoMakie backend, while at the same time being able to facilitate the GPU by the GLMakie or WGLMakie backend. The latter is especially suited for notebook environments that offer a great possibility for teaching. In this talk, I will show you how Dennis Ogiermann and me automated a lot of annoying steps for you and bundled the code in a package called FerriteViz.jl. \\ Code: [ferritecon22](https://github.com/koehlerson/ferritecon22) and [FerriteViz.jl](https://github.com/Ferrite-FEM/FerriteViz.jl)
| 11:20-11:45 | **Using Ferrite.jl for multiscale bone simulations**, *Mischa Blaszczyk, Klaus Hackl*\\We present our computer program -- written in the Julia programming language, mainly using the Ferrite.jl package -- which we used to perform FE² bone simulations for our research. We discuss our reasons for choosing Julia and Ferrite, which aspects of the package we are using and show some implementation details regarding e.g. meshing, coupled problems, periodic boundary conditions and parallel computing. Finally, we discuss features the framework is still lacking and formulate our wishes for the future. \\ Code: [bone\_fe2\_c](https://github.com/blaszm/bone_fe2_c) \\ Presentation: [Using Ferrite.jl for multiscale bone simulations](/assets/blaszm.pdf)
| 11:45-13:15 | **Lunch break**
| 13:15-13:40 | **Usecases of Ferrite.jl**, *Hendrik Geisler, Dustin R. Jantos, Miriam Kick*\\In this talk, we present several complex applications of Ferrite.jl in material modeling and optimization. Hereby, we motivate the use of Ferrite.jl in advanced FEM research. The examples include uncertainty quantification, topology optimization and damage modeling. We discuss implementation details as handling nonlocal evolution equations and implementing various material models. At the end, we show some extensions, e.g. for handling complex boundary conditions.
| 13:40-14:05 | **Isogeometric analysis with Ferrite.jl and IGA.jl**, *Elias Börjesson*\\Isogeometric analysis is a computational approach similar to the Finite Element Method, where the shape functions used for the discretisation of the geometry are higher order continuous spline functions. The higher order continuity offer some interesting advantages, for example closer connection with CAD, and faster convergence per degree of freedom. In this presentation, I will showcase the Package IGA.jl, which is a toolbox build on top of Ferrite, for creating efficient and flexible IGA simulations. \\Code: [IGA.jl](https://github.com/lijas/IGA.jl)
| 14:05-14:30 | **A brief history of Ferrite.jl**, *Kristoffer Carlsson*\\Did you know what in the end became Ferrite started out as a Python library called "lolFem"?. In this presentation I will go through the different stages of evolution Ferrite went through before it became what it is today. \\Code: [lolFem](https://github.com/KristofferC/lolFem) → [FEM.jl](https://github.com/KristofferC/FEM.jl) → [Ferrite.jl](https://github.com/Ferrite-FEM/Ferrite.jl) 
| 14:30-15:00 | [**Fika**](https://en.wikipedia.org/wiki/Fika_(Sweden))
| 15:00-17:00 | [**Hackathon**](https://en.wikipedia.org/wiki/Hackathon)
| 17:00       | **Leaving for ["after work"](https://sv.wikipedia.org/wiki/Afterwork)**

Coffee and snacks for the morning and afternoon will be provided (for free). 

The after work will be at [Le Feu](https://www.lefeu.de/le-feu-flammkuchen-braunschweig/) where we can order drinks and food. 

For organizational reasons, if you do *not* intend to participate in the evening, please let us
know!

## Presentations

For those of you who are contributing with a presentation: We have allocated 20+5 minutes
per presentation. Make sure you can connect an HDMI-cable to your computer.


## Registration and abstract submission

The conference is free of charge, but registration is necessary. To register,
please send an email to Fredrik Ekre
([f.ekre@tu-braunschweig.de](mailto:f.ekre@tu-braunschweig.de)) at the latest
the **9th of September (2022-09-09)** (extended deadline for participation). 

## Contact

If you have any questions, please don't hesitate to ask by sending an email to
the organizers:

- Fredrik Ekre [f.ekre@tu-braunschweig.de](mailto:f.ekre@tu-braunschweig.de)
- Knut Andreas Meyer [k.a.meyer@tu-braunschweig.de](mailto:k.a.meyer@tu-braunschweig.de)
