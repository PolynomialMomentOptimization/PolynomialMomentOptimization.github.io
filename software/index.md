<div> </div>

# An overview of software for polynomial and moment optimization

## Polynomial Optimisation solvers
- [MomentTools](https://gitlab.inria.fr/AlgebraicGeometricModeling/MomentTools.jl) is an open source Julia package for solving polynomial optimization problems, via moment matrix relaxations. It provides tools to optimize vectors of moments sequences that satisfy positivity constraints or mass constraints, to extract minimizers from moment sequences. It uses a connection with SDP solvers such as CSDP, Mosek, SDPA, ... via the  [JuMP](https://jump.dev/JuMP.jl/stable/) interface. 
It is developed by Lorenzo Baldi and Bernard Mourrain (Inria).
- [MomentOpt](https://lanl-ansi.github.io/MomentOpt.jl/stable/)  is a Julia package to model Generalized Moment Problems  and to approximate solutions via convex relaxations of moment-SOS hierarchies. The main features of MomentOpt.jl are a highlevel syntax to define Generalized Moment Problems easily and different options to approximate solutions and switch between different formulations easily. It is developed by Tillmann Weisser, Benoît Legat, Chris Coey, Lea Kapelevich and  Juan Pablo Vielma.
- [TSSOS](https://github.com/wangjie212/TSSOS) is an open source Julia library developed by Jie Wang, V. Magron (LAAS CNRS) for large-scale polynomial optimization, based on the sparsity adapted moment-SOS hierarchies. Related modules can perform complex polynomial optimization, eigenvalue/trace optimization of noncommutative polynomials, compute joint spectral radii for stability analysis, approximate attractors and invariants of sparse dynamical systems.

These Julia packages use  SDP solvers via the interface package [JuMP.jl](https://jump.dev/JuMP.jl/stable/). A list of convex optimization solvers available in JuMP can be found [here]( https://jump.dev/JuMP.jl/stable/installation/#Supported-solvers).

* [POEM](http://www.iaa.tu-bs.de/AppliedAlgebra/POEM/) is a software for solving polynomial optimization problems developed at the Applied Algebra group at the [Institute for Analysis and Algebra](https://www.tu-braunschweig.de/iaa) at Technische Universität Braunschweig. It mainly uses sums of nonnegative circuit polynomials (SONC), a certificate for nonnegativity of polynomials independent of sums of  squares, which were developed by [Timo de Wolff](http://www.iaa.tu-bs.de/timodewolff/) and Sadik Iliman. SONC certificates are computed via geometric programs. POEM can also compute solutions via SAGE (sums of AM-GM exponentials) and SOS (sums of squares) certificates. POEM uses a variety of established solvers. It is written in Python.    




## Polynomial equation solvers

- [mpsolve](https://msolve.lip6.fr) is an open source C library for polynomial system solving with algebraic methods such as Groebner bases. In particular it can be used for solving polynomial optimization problems. It is developed by Jeremy Berthomieu (University of Sorbonne), Christian Eder (TU Kaiserslautern) and Mohab Safey El Din (University of Sorbonne).
