+++
title = "Ferrite.jl Conference 2025"
hascode = false
hasmath = false
+++

# FerriteCon 2025
FerriteCon 2025 will take place at the [Technical University of Denmark (DTU)](https://www.dtu.dk/english/) 
outside Copenhagen, Denmark, on August 28th, 2025, supported by
[The Danish Center for Applied Mathematics and Mechanics, DCAMM](http://www.dcamm.dk).

## Ferrite.jl User & Developer Conference 2025
[Ferrite.jl](https://ferrite-fem.github.io/Ferrite.jl/stable/) is an open-source
finite element package written in the [Julia programming
language](https://julialang.org/). On Thursday the 28th of August 2025 we will host the fourth annual
Ferrite.jl user and developer conference at the Technical University of Denmark (DTU) in Lyngby, Denmark.

The conference aims to improve existing, and find new, technical and scientific
collaborations among Ferrite.jl users and developers, as well as to discuss
how the package can be further developed in the future. The conference will consist of both beginner-friendly 
and advanced presentations on Ferrite.jl and of current research using Ferrite.jl.

### Preliminary schedule
Click on the titles with grey background to expand the abstract. 

| Time        | Activity                                                                   |
|-------------|----------------------------------------------------------------------------|
| 09:00-09:25 | **Welcome coffee**
| 09:25-09:30 | **Opening and introduction**
| 09:30-10:15 | **_Keynote_** \\ **Differentiable programming for scientific computing with Enzyme and Julia**\\ *Valentin Churavy*, University of Augsburg
| 10:15-10:50 | **Introduction to Ferrite.jl** \\ *Kim Louisa Auth*, Technical University of Denmark \\ 
| 10:50-11:10 | Coffee break
| 11:10-11:30 | \collaps{**Current applications of Ferrite.jl at Institute of Continuum Mechanics (Leibniz University Hannover)**\\*Speaker: TBA*}{
    The research spectrum of IKM covers the modelling and numerically efficient solution of complex
    material behavior, including topology optimization and uncertainty quantification. The solution of
    the derived equations generally relies on the Finite Element Method but also requires significant
    adjustments and additions for innovative numerical solutions. This makes Ferrite.jl, as a FEM
    toolbox, of great use for us, as it allows for the required freedom to implement our methods.
    We present examples on uncertainty quantifications, topology optimization and coupled
    problems, showing the numerical implementation and results, which highlight the application of
    Ferrite.jl and discuss the package expansion possibilities.} \\
| 11:30-11:50 | \collaps{**Ensemble Kalman Filtering for Stochastic Phase Field Models of Brittle Fracture**\\ *Lucas Hermann*, TU Braunschweig}{
    Numerical models usually involve making assumptions about material parameters, initial conditions etc. Treating these parameters as random variables leads to randomness in the model outcome. I present how I quantify that uncertainty in a Ferrite.jl simulation of a phase field brittle fracture problem and I show how data can be used to decrease that uncertainty in order to get more reliable model outcomes.} \\
| 11:50-12:10 | \collaps{**Variational Minimization Formulation for Gradient-Extended Coupled Problems**\\ *Basavesh Yaraguntappa*, Universität Stuttgart}{
    In this work, we present a two-field canonical minimization formulation for phase-field approach to topology optimization.
    We further extend this to other problems like second-order poro-elasticity to model the hydro-mechanical behaviour of porous media.
    I would also like to share my experience on using Ferrite.jl for teaching from two perspectives. 
    As an instructor teaching courses in computational mechanics and also as an IT administrator at the institute.} \\
| 12.10-13.15 | **Lunch**
| 13:15-13.35 | \collaps{**Tensors.jl - Efficient tensor computations with support for automatic differentiation**\\ *Carlsson Kristoffer*, JuliaHub}{
    Abstract to be added} \\
| 13:35-13:55 | \collaps{**Ferrite + X**\\ *Fredrik Ekre*, JuliaHub}{
    Ferrite is often described as a FEM "toolbox" as opposed to a full fledged FEA platform. In this talk I will present how Ferrite seamlessly integrates with many other packages in the Julia ecosystem to enable more features. For example, BlockArrays.jl can be used for blocked global (or local) system matrices and enable block based solvers, OhMyThreads.jl can be used to enable multithreaded assembly and ForwardDiff.jl can be used to enable automatic differentiation. Hopefully this talk will demonstrate how easy it is to bring more functionality to Ferrite through other packages and inspire you to try out your own combinations of packages in order to tailor for your own Ferrite use case.} \\
| 13:55-14.15 | \collaps{**Ferrite now has true vector interpolations - what, why, and how?**\\ *Knut Andreas Meyer*, Chalmers University of Technology}{
    With newly added H(div) and H(curl) interpolations, Ferrite.jl can now tackle a broader range of problems — but this also brings extra complexity to `FEValues`. In this talk, I’ll go over what these interpolation types are, when you might need them, and how they’re implemented in Ferrite} \\
| 14:15-14:35 | \collaps{**A Tale of Two Multigrids: A Case Study on A- and P- Multigrid Methods in Vector Valued PDEs**\\ *Abdelrahman Fathy*, Ruhr-Universität Bochum}{
    Algebraic Multigrid (AMG) methods can be highly effective for solving vector-valued PDEs—such as linear elasticity—when properly tuned with suitable near null spaces. However, classical AMG struggles with higher-order finite element discretizations. In contrast, Polynomial Multigrid (pMG), a geometric multigrid variant, excels at coarsening high-order polynomial spaces down to linear order (p = 1). These two approaches can be effectively combined by applying AMG as the coarse solver within a pMG hierarchy, where AMG is often optimal for the resulting first-order problems. This hybrid strategy is realized in the new Julia package FerriteMultigrid.jl, which builds on Ferrite.jl for finite element infrastructure and AlgebraicMultigrid.jl for coarse-level solves. In this presentation, I will outline the theoretical foundations of this method using linear elasticity as a guiding example and demonstrate how the package helps in quickly developing efficient combined multigrid preconditioners.} \\
| 14.35-15.00 | **[Fika](https://en.wikipedia.org/wiki/Coffee_culture#Sweden)**
| 15:00-15.20 | \collaps{**Viscoplastic Modeling the Evolving Mechanical Properties of Shotcrete 3D Printing Material**\\ *Quoc Tuan La*, TU Braunschweig}{
    This work presents a viscoplastic material model for concrete used in shotcrete 3D printing, which is
an additive manufacturing method. Numerical examples at both material and structural levels are provided
to showcase the transient response of the material and the development of plastic failure within an
additively manufactured structure. The implementation is performed using `Ferrite.jl` as the Finite Element
framework. In addition, `FerriteInterfaceElements.jl` is utilized to simulate the interlayer
behavior.} \\
| 15:20-15.40 | \collaps{**Revisiting Adaptive Mesh Refinement that's not P4est**\\ *Abdulaziz	Mohamed*, Ruhr-Universität Bochum}{
    Update on Adaptive Mesh Refinement (AMR) presented in last year's FerriteCon. This AMR algorithm differs from other algorithms in that the finer elements are superpositioned with their parents rather than substituting them. In contrast to classical AMR techniques, this allows the enforcement of continuity without explicitly forming constraints, as would result in the classical approach due to e.g. hanging nodes. With this algorithm we cache local element contributions reducing the assembly overhead. This is especially beneficial for local timestepping using Discontinuous Galerking (DG) as the timestepping is done per element due to the mass matrix being block-diagonal thus no need to assemble the cached local matrices into a global one. The implementation follows the work of "Efficient multi-level hp-finite elements in arbitrary dimensions" (Kopp et al., 2022).} \\
| 15:40-16.00 | \collaps{**Order Matters - How to Boost Finite Element Simulations with Graph Sorting**\\ *Dennis Ogiermann*, Ruhr-Universität Bochum}{
Many finite element codes tend to be memory bound, which implies that relying on the good cache access patterns matters.
However, general purpose mesh generators like Gmsh tend to order the elements in a seemingly random way.
Even worse, the topology of a mesh is, in general, a graph.
When iterating over the elements, thinking about nodal ansatz functions for now, then it would be ideal to use the reuse nodal information of previous elements as good as possible, i.e. we want to iterate consecutively over neighboring elements.
In this light the question on how to order the elements can be framed as the quest for finding an ordering, such that the linear path induced by the element numbering minimizes some functional, which describes this neighborhood -- or formally, we want to solve a linear arrangement problem.
In this talk I will show you on some benchmarks how Gecko.jl can be used to solve this problem, thus speeding up your simulations.
} \\

| 16:15-17:30 | **Hackathon and open discussion**
| 18:00       | **Social Dinner**

You can also have a look at the program of previous editions of FerriteCon:
- [FerriteCon 2022 (Braunschweig, Germany)](/2022/)
- [FerriteCon 2023 (Bochum, Germany)](/2023/)
- [FerriteCon 2024 (Gothenburg, Sweden)](/2024/)

**Target audience for FerriteCon**

If you have used, contributed to, or are just curious about Ferrite.jl we
encourage you to participate. While the conference is free of charge, 
[registration](#registration_and_abstract_submission) is necessary.

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

## Registration and abstract submission
To register without a presentation, please register as soon as possible, but latest **15th of August (2025-08-15)**,
by sending an email with name and affiliation to [Kim Louisa Auth](mailto:kloau@dtu.dk).

To register as a speaker, please submit a title and a brief abstract (~100 words, 3-4 sentences) to
[Kim Louisa Auth](mailto:kloau@dtu.dk) by the ~~~<s>15th of July (2025-07-15)</s>~~~  **25th of July (2025-07-25)**.

## Contact
If you have any questions, please don't hesitate to ask by sending an email to
the organizers:

- Kim Louisa Auth [kloau@dtu.dk](mailto:kloau@dtu.dk)
- Knut Andreas Meyer [knut.andreas.meyer@chalmers.se](mailto:knut.andreas.meyer@chalmers.se)
