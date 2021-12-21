<div> </div>

# An overview of software for polynomial and moment optimization

## Julia packages
- [MomentTools.jl](https://gitlab.inria.fr/AlgebraicGeometricModeling/MomentTools.jl) is an open source Julia package for solving polynomial optimization problems, via moment matrix relaxations. It provides tools to optimize vectors of moments sequences that sastisfy positivity constraints or mass constraints,to extract minimizers from moment sequences. It uses a connection with SDP solvers such as CSDP, Mosek, SDPA, ... via the JuMP interface. 
It is developed by L. Baldi and B. Mourrain.

- [MomentOpt](https://lanl-ansi.github.io/MomentOpt.jl/stable/)
...

- [TSSOS](https://github.com/wangjie212/TSSOS) 
is an open source Julia library developed by LAAS CNRS (Jie Wang, V. Magron) for large-scale polynomial optimization, based on the sparsity adapted moment-SOS hierarchies. Related modules can perform complex polynomial optimization, eigenvalue/trace optimization of noncommutative polynomials, compute joint spectral radii for stability analysis, approximate attractors and invariants of sparse dynamical systems.


## Polynomial equation solvers

- [mpsolve](https://msolve.lip6.fr) is an open source C library developed by University of Sorbonne and TU Kaiserslautern for polynomial system solving with algebraic methods such as Groebner bases, in particular it can also be used for solving polynomial optimization problems
