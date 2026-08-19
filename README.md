# Awesome Scientific Computing with stars

[<img src="https://nschloe.github.io/awesome-scientific-computing/sunglasses.svg" align="right" width="30%">](#readme)

> Useful resources for scientific computing and numerical analysis.

Scientific computing and numerical analysis are research fields that aim to provide
methods for solving large-scale problems from various areas of science with the help of
computers. Typical problems are ordinary and partial differential equations (ODEs,
PDEs), their discretizations, and the solution of linear algebra problems arising from
them.

## Contents

* [Basic linear algebra](#basic-linear-algebra)
* [Multi-purpose toolkits](#multi-purpose-toolkits)
* [Finite Elements](#finite-elements)
* [Meshing](#meshing)
* [Data formats](#data-formats)
* [Sparse linear solvers](#sparse-linear-solvers)
* [Visualization](#visualization)
* [Other libraries and tools](#other-libraries-and-tools)
* [Community](#community)

## Basic linear algebra

* [OpenBLAS](https://www.openblas.net) - Optimized BLAS library based on GotoBLAS2.
  (C and Assembly, BSD, [GitHub](https://github.com/OpenMathLib/OpenBLAS) ⭐ 7,559 | 🐛 114 | 🌐 C | 📅 2026-08-18)
* [BLIS](https://github.com/flame/blis) ⭐ 2,672 | 🐛 129 | 🌐 C | 📅 2026-07-10 - High-performance BLAS-like dense linear algebra libraries.
  (C, BSD, GitHub)
* [BLAS](https://netlib.org/blas/) - Standard building blocks for performing basic vector and matrix operations.
  (Fortran, public domain, [GitHub](https://github.com/Reference-LAPACK/lapack/tree/master/BLAS) ⭐ 1,888 | 🐛 139 | 🌐 Fortran | 📅 2026-08-06)
* [LAPACK](https://netlib.org/lapack/) - Routines for solving systems of linear equations, linear least-squares, eigenvalue problems, etc.
  (Fortran, BSD, [GitHub](https://github.com/Reference-LAPACK/lapack) ⭐ 1,888 | 🐛 139 | 🌐 Fortran | 📅 2026-08-06)
* [Ginkgo](https://ginkgo-project.github.io/) - High-performance manycore linear algebra library, focus on sparse systems.
  (C++, BSD, [GitHub](https://github.com/ginkgo-project/ginkgo) ⭐ 618 | 🐛 214 | 🌐 C++ | 📅 2026-08-19)
* [Eigen](https://libeigen.gitlab.io/) - C++ template library for linear algebra.
  (C++, MPL 2, [GitLab](https://gitlab.com/libeigen/eigen))
* [blaze](https://bitbucket.org/blaze-lib/blaze) - High-performance C++ math library for dense and sparse arithmetic.
  (C++, BSD, Bitbucket)

## Multi-purpose toolkits

* [NumPy](https://numpy.org/) - Fundamental package needed for scientific computing with Python.
  (Python, BSD, [GitHub](https://github.com/numpy/numpy) ⭐ 32,558 | 🐛 2,334 | 🌐 Python | 📅 2026-08-19)
* [SciPy](https://scipy.org) - Python modules for statistics, optimization, integration, linear algebra, etc.
  (Python, mostly BSD, [GitHub](https://github.com/scipy/scipy/) ⭐ 14,935 | 🐛 1,846 | 🌐 Python | 📅 2026-08-19)
* [DifferentialEquations.jl](https://docs.sciml.ai/DiffEqDocs/stable/) - Toolbox for solving different types of differential equations numerically. (Julia, MIT, [GitHub](https://github.com/SciML/DifferentialEquations.jl) ⭐ 3,145 | 🐛 126 | 🌐 Julia | 📅 2026-08-17)
* [PETSc](https://petsc.org/release/) - Parallel solution of scientific applications modeled by PDEs.
  (C, 2-clause BSD, [GitLab](https://gitlab.com/petsc/petsc))
* [DUNE Numerics](https://www.dune-project.org) - Toolbox for solving PDEs with grid-based methods.
  (C++, GPL 2, [GitLab](https://gitlab.dune-project.org/core/))

## Finite Elements

* [MOOSE](https://mooseframework.inl.gov/) - Multiphysics Object Oriented Simulation Environment.
  (C++, LGPL 2.1, [GitHub](https://github.com/idaholab/moose) ⭐ 2,331 | 🐛 2,811 | 🌐 C++ | 📅 2026-08-19)
* [MFEM](https://mfem.org) - Free, lightweight, scalable C++ library for finite element methods.
  (C++, BSD-3-Clause, [GitHub](https://github.com/mfem/mfem) ⭐ 2,220 | 🐛 222 | 🌐 C++ | 📅 2026-08-19)
* [deal.II](https://dealii.org) - Software library supporting the creation of finite element codes.
  (C++, LGPL 2.1, [GitHub](https://github.com/dealii/dealii) ⭐ 1,710 | 🐛 636 | 🌐 C++ | 📅 2026-08-19)
* [SfePy](https://sfepy.org) - Simple Finite Elements in Python.
  (Python, BSD, [GitHub](https://github.com/sfepy/sfepy) ⭐ 838 | 🐛 79 | 🌐 Python | 📅 2026-08-14)
* [libMesh](https://libmesh.github.io) - Framework for the numerical simulation of PDEs using unstructured discretizations.
  (C++, LGPL 2.1, [GitHub](https://github.com/libMesh/libmesh) ⭐ 757 | 🐛 334 | 🌐 C | 📅 2026-08-18)
* [Firedrake](https://www.firedrakeproject.org) - Automated system for the solution of PDEs using the finite element method.
  (Python, LGPL 3, [GitHub](https://github.com/firedrakeproject/firedrake) ⭐ 669 | 🐛 449 | 🌐 Python | 📅 2026-08-18)
* [scikit-fem](https://github.com/kinnala/scikit-fem) ⭐ 644 | 🐛 11 | 🌐 Python | 📅 2026-08-19 - Simple finite element assemblers.
  (Python, BSD/GPL, GitHub)
* [Netgen/NGSolve](https://ngsolve.org) - High performance multiphysics finite element software.
  (C++, LGPL 2.1, [GitHub](https://github.com/NGSolve/netgen) ⭐ 386 | 🐛 116 | 🌐 C++ | 📅 2026-08-06)
* [libceed](https://libceed.readthedocs.io/en/latest/index.html) - Code for Efficient Extensible Discretizations.
  (C, 2-clause BSD, [GitHub](https://github.com/CEED/libCEED) ⭐ 264 | 🐛 49 | 🌐 C | 📅 2026-08-19)
* [FEniCS](https://fenicsproject.org) - Computing platform for solving PDEs in Python and C++.
  (C++/Python, LGPL 3, [GitHub](https://github.com/FEniCS)/[Bitbucket](https://bitbucket.org/fenics-project/))
* [FreeFEM](https://freefem.org) - High level multiphysics-multimesh finite element language.
  (C++, LGPL, [GitHub](https://github.com/FreeFem))

## Meshing

### Triangular and tetrahedral meshing

* [CGAL](https://www.cgal.org) - Algorithms for computational geometry.
  (C++, mixed LGPL/GPL, [GitHub](https://github.com/CGAL/cgal) ⭐ 6,011 | 🐛 682 | 🌐 C++ | 📅 2026-08-17)
* [trimesh](https://trimesh.org) - Loading and using triangular meshes with an emphasis on watertight surfaces.
  (Python, MIT, [GitHub](https://github.com/mikedh/trimesh) ⭐ 3,651 | 🐛 480 | 🌐 Python | 📅 2026-08-18)
* [pygmsh](https://github.com/nschloe/pygmsh) ⭐ 967 | 🐛 60 | 🌐 Python | 📅 2023-10-04 - Python interface for Gmsh.
  (Python, GPL 3, GitHub)
* [TetWild](https://arxiv.org/abs/1908.03581) - Generate tetrahedral meshes for triangular surface meshes.
  (C++, GPL 3, [GitHub](https://github.com/Yixin-Hu/TetWild) ⭐ 721 | 🐛 31 | 🌐 C++ | 📅 2023-04-27)
* [pygalmesh](https://github.com/meshpro/pygalmesh) ⭐ 667 | 🐛 33 | 🌐 C++ | 📅 2024-07-22 - Python interface for CGAL's 3D meshing capabilities.
  (Python, GPL 3, GitHub)
* [fTetWild](https://arxiv.org/abs/1908.03581) - Same as TetWild, but faster.
  (C++, MPL 2, [GitHub](https://github.com/wildmeshing/fTetWild) ⭐ 594 | 🐛 37 | 🌐 C++ | 📅 2026-05-05)
* [MeshPy](https://mathema.tician.de/software/meshpy/) - Quality triangular and tetrahedral mesh generation.
  (Python, MIT, [GitHub](https://github.com/inducer/meshpy) ⭐ 586 | 🐛 18 | 🌐 C++ | 📅 2026-08-10)
* [TriWild](https://cims.nyu.edu/gcl/papers/2019-TriWild.pdf) - Robust triangulation with curve constraints.
  (C++, MPL 2, [GitHub](https://github.com/wildmeshing/TriWild) ⭐ 265 | 🐛 6 | 🌐 C++ | 📅 2025-12-22)
* [dmsh](https://github.com/meshpro/dmsh) ⭐ 222 | 🐛 4 | 📅 2026-05-18 - Simple generator for unstructured triangular meshes, inspired by distmesh.
  (Python, proprietary, GitHub)
* [SeismicMesh](https://github.com/krober10nd/SeismicMesh) ⚠️ Archived - Parallel 2D/3D triangle/tetrahedral mesh generation with sliver removal.
  (Python and C++, GPL 3, GitHub)
* [Gmsh](https://gmsh.info) - Three-dimensional finite element mesh generator with pre- and post-processing facilities.
  (C++, GPL, [GitLab](https://gitlab.onelab.info/gmsh/gmsh))
* [TetGen](https://www.wias-berlin.de/software/index.jsp?id=TetGen) - Quality tetrahedral mesh generator and 3D Delaunay triangulator.
  (C++, AGPLv3)
* [Triangle](https://www.cs.cmu.edu/~quake/triangle.html) - Two-dimensional quality mesh generator and Delaunay triangulator.
  (C, *nonfree software*)
* [distmesh](https://persson.berkeley.edu/distmesh/) - Simple generator for unstructured triangular and tetrahedral meshes.
  (MATLAB, GPL 3)

### Quadrilateral and hexahedral meshing

* [QuadriFlow](https://stanford.edu/~jingweih/papers/quadriflow/) - Scalable and robust quadrangulation from triangulation.
  (C++, BSD, [GitHub](https://github.com/hjwdzh/QuadriFlow) ⭐ 859 | 🐛 9 | 🌐 C++ | 📅 2019-12-07)

### Mesh tools

* [meshio](https://github.com/nschloe/meshio) ⭐ 2,320 | 🐛 250 | 🌐 Python | 📅 2024-07-23 - I/O for various mesh formats, file conversion.
  (Python, MIT, GitHub)
* [pmp-library](https://www.pmp-library.org/) - Polygon mesh processing library.
  (C++, MIT with Employer Disclaimer, [GitHub](https://github.com/pmp-library/pmp-library/) ⭐ 1,500 | 🐛 17 | 🌐 C++ | 📅 2026-08-03)
* [optimesh](https://github.com/meshpro/optimesh) ⭐ 635 | 🐛 3 | 📅 2026-05-18 - Triangular mesh smoothing.
  (Python, proprietary, GitHub)
* [Mmg](https://www.mmgtools.org/) - Robust, open-source & multidisciplinary software for remeshing.
  (C, LGPL 3, [GitHub](https://github.com/MmgTools/mmg) ⭐ 483 | 🐛 45 | 🌐 C | 📅 2026-05-11)
* [meshplex](https://github.com/meshpro/meshplex) ⭐ 110 | 🐛 8 | 📅 2026-05-18 - Fast tools for simplex meshes.
  (Python, proprietary, GitHub)
* [MOAB](https://sigma.mcs.anl.gov/moab-library/) - Representing and evaluating mesh data.
  (C++, mostly LGPL 3, [Bitbucket](https://bitbucket.org/fathomteam/moab/))

## Data formats

* [Zarr](https://zarr.readthedocs.io/en/stable/) - Format for the storage of chunked, compressed, N-dimensional arrays.
  (Python, MIT, [GitHub](https://github.com/zarr-developers/zarr-python) ⭐ 2,040 | 🐛 501 | 🌐 Python | 📅 2026-08-17)
* [HDF5](https://www.hdfgroup.org/solutions/hdf5/) - Data model, library, and file format for storing and managing data.
  (C/Fortran, BSD, [GitHub](https://github.com/HDFGroup/hdf5) ⭐ 976 | 🐛 341 | 🌐 C | 📅 2026-08-19)
* [NetCDF](https://www.unidata.ucar.edu/software/netcdf) - Software libraries and data formats for array-oriented scientific data.
  (C/C++/Fortran/Java/Python, [custom open-source
  license](https://www.unidata.ucar.edu/software/netcdf/licensing),
  [GitHub](https://github.com/Unidata/netcdf-c/) ⭐ 601 | 🐛 295 | 🌐 C | 📅 2026-08-18)
* [XDMF](https://xdmf.org/) - eXtensible Data Model and Format for data from High Performance Computing codes.
  (C++, [GitLab](https://gitlab.kitware.com/xdmf/xdmf))

## Sparse linear solvers

* [hypre](https://computing.llnl.gov/projects/hypre-scalable-linear-solvers-multigrid-methods) - Library of high-performance preconditioners and solvers.
  (C, Apache 2.0/MIT, [GitHub](https://github.com/hypre-space/hypre) ⭐ 852 | 🐛 179 | 🌐 C | 📅 2026-08-18)
* [PyAMG](https://pyamg.readthedocs.io/en/latest/) - Algebraic Multigrid Solvers in Python.
  (Python, MIT, [GitHub](https://github.com/pyamg/pyamg) ⭐ 652 | 🐛 40 | 🌐 Python | 📅 2026-03-30)
* [SuperLU](https://portal.nersc.gov/project/sparse/superlu/) - Direct solution of large, sparse, nonsymmetric systems of linear equations.
  (C, mostly BSD, [GitHub](https://github.com/xiaoyeli/superlu) ⭐ 332 | 🐛 26 | 🌐 C | 📅 2026-08-16)

## Visualization

* [F3D](https://f3d.app/) - Cross-platform, fast, and minimalist 3D viewer with scientific visualization tools.
  (C++, BSD, [GitHub](https://github.com/f3d-app/f3d) ⭐ 4,634 | 🐛 339 | 🌐 C++ | 📅 2026-08-19)
* [PyVista](https://docs.pyvista.org/) - 3D plotting and mesh analysis through a streamlined interface for VTK.
  (Python, MIT, [GitHub](https://github.com/pyvista/pyvista) ⭐ 3,774 | 🐛 597 | 🌐 Python | 📅 2026-08-19)
* [vedo](https://vedo.embl.es) - Library for scientific analysis and visualization of 3D objects based on VTK.
  (Python, MIT, [GitHub](https://github.com/marcomusy/vedo) ⭐ 2,262 | 🐛 171 | 🌐 Python | 📅 2026-08-04)
* [Polyscope](https://polyscope.run/) - Viewer and user interface for 3D geometry processing.
  (C++, MIT, [GitHub](https://github.com/nmwsharp/polyscope) ⭐ 2,196 | 🐛 127 | 🌐 C++ | 📅 2026-05-20)
* [Mayavi](https://docs.enthought.com/mayavi/mayavi/) - 3D scientific data visualization and plotting in Python.
  (Python, BSD, [GitHub](https://github.com/enthought/mayavi) ⭐ 1,407 | 🐛 455 | 🌐 Python | 📅 2026-08-15)
* [yt](https://yt-project.org/) - Toolkit for analysis and visualization of volumetric data.
  (Python, BSD, [GitHub](https://github.com/yt-project/yt) ⭐ 558 | 🐛 483 | 🌐 Python | 📅 2026-08-05)
* [TTK](https://topology-tool-kit.github.io/) - Topological data analysis and visualization.
  (C++/Python, BSD, [GitHub](https://github.com/topology-tool-kit/ttk) ⭐ 478 | 🐛 23 | 🌐 C++ | 📅 2026-08-17)
* [morphologica](https://github.com/ABRG-Models/morphologica) ⚠️ Archived - Header-only, modern OpenGL code to visualize numerical simulations at runtime. (C++, Apache 2.0, GitHub)
* [ParaView](https://www.paraview.org) - Multi-platform data analysis and visualization application based on VTK.
  (C++, BSD, [GitLab](https://gitlab.kitware.com/paraview/paraview))
* [VTK](https://vtk.org/) - Process images and create 3D computer graphics.
  (C++, BSD, [GitLab](https://gitlab.kitware.com/vtk/vtk))

## Other libraries and tools

* [cvxpy](https://www.cvxpy.org/) - Modeling language for convex optimization problems.
  (Python, Apache 2.0, [GitHub](https://github.com/cvxpy/cvxpy) ⭐ 6,305 | 🐛 194 | 🌐 C++ | 📅 2026-08-18)
* [FFTW](http://www.fftw.org) - Discrete Fourier transforms in one or more dimensions, of arbitrary input size, real and complex.
  (C, GPL2, [GitHub](https://github.com/FFTW/fftw3) ⭐ 3,098 | 🐛 183 | 🌐 C | 📅 2026-06-10)
* [PyWavelets](https://pywavelets.readthedocs.io/en/latest/) - Wavelet transforms in Python.
  (Python, MIT, [GitHub](https://github.com/PyWavelets/pywt) ⭐ 2,397 | 🐛 81 | 🌐 Python | 📅 2026-08-17)
* [OpenFOAM](https://www.openfoam.com) - Free, open source CFD (computational fluid dynamics) software.
  (C++, GPL 3, [GitHub](https://github.com/OpenFOAM/OpenFOAM-dev) ⭐ 2,200 | 🐛 7 | 🌐 C++ | 📅 2026-08-19)
* [pyGAM](https://pygam.readthedocs.io/en/latest/) - Generalized Additive Models in Python.
  (Python, Apache 2.0, [GitHub](https://github.com/dswah/pyGAM) ⭐ 1,011 | 🐛 232 | 🌐 Python | 📅 2026-04-21)
* [Qhull](http://www.qhull.org) - Convex hull, Delaunay triangulation, Voronoi diagram, halfspace intersection about a point, etc.
  (C/C++, [custom open source license](http://www.qhull.org/COPYING.txt),
  [GitHub](https://github.com/qhull/qhull/) ⭐ 824 | 🐛 30 | 🌐 C | 📅 2025-09-07)
* [quadpy](https://github.com/sigma-py/quadpy) ⭐ 785 | 🐛 31 | 📅 2026-05-18 - Numerical integration (quadrature, cubature) in Python.
  (Python, proprietary, GitHub)
* [Dedalus](https://dedalus-project.org/) - Solve partial differential equations with spectral methods.
  (Python, GPL 3, [GitHub](https://github.com/DedalusProject/dedalus) ⭐ 703 | 🐛 64 | 🌐 Python | 📅 2026-07-21)
* [Chebfun](https://www.chebfun.org/) - Computing with functions to about 15-digit accuracy.
  (MATLAB, BSD, [GitHub](https://github.com/chebfun/chebfun) ⭐ 677 | 🐛 174 | 🌐 MATLAB | 📅 2026-06-23)
* [FiPy](https://www.ctcms.nist.gov/fipy/) - Finite-volume PDE solver.
  (Python, [custom open-source
  license](https://www.nist.gov/open/copyright-fair-use-and-licensing-statements-srd-data-software-and-technical-series-publications),
  [GitHub](https://github.com/usnistgov/fipy) ⭐ 636 | 🐛 178 | 🌐 Python | 📅 2026-06-18)
* [PyGMO](https://esa.github.io/pygmo/) - Massively parallel optimization.
  (Python/C++, MPL 2, [GitHub](https://github.com/esa/pygmo2) ⭐ 534 | 🐛 39 | 🌐 C++ | 📅 2026-04-17)
* [pyMOR](https://pymor.org/) - Model Order Reduction with Python.
  (Python, 2-clause BSD, [GitHub](https://github.com/pymor/pymor/) ⭐ 346 | 🐛 130 | 🌐 Python | 📅 2026-08-19)
* [shenfun](https://shenfun.readthedocs.io/en/latest/) - High-performance Python library for the spectral Galerkin method.
  (Python, BSD-2, [GitHub](https://github.com/spectralDNS/shenfun) ⭐ 232 | 🐛 31 | 🌐 Python | 📅 2026-07-20)
* [orthopy](https://github.com/sigma-py/orthopy) ⭐ 192 | 🐛 8 | 📅 2026-05-18 - Compute orthogonal polynomials efficiently.
  (Python, proprietary, GitHub)
* [NFFT](https://www-user.tu-chemnitz.de/~potts/nfft/) - Nonequispaced fast Fourier transform.
  (C/MATLAB, GPL 2, [GitHub](https://github.com/NFFT/nfft) ⭐ 187 | 🐛 19 | 🌐 C | 📅 2026-08-12)
* [HPDDM](https://github.com/hpddm/hpddm) ⭐ 154 | 🐛 1 | 🌐 C++ | 📅 2026-07-31 - High-performance unified framework for domain decomposition methods.
  (C++, LGPL 3, GitHub)
* [PyDMD](https://github.com/mathLab/PyDMD) ⭐ 127 | 🐛 0 | 🌐 Python | 📅 2025-03-06 - Dynamic Mode Decomposition (DMD) in Python.
  (Python, MIT, GitHub)
* [accupy](https://github.com/sigma-py/accupy) ⭐ 107 | 🐛 2 | 🌐 Python | 📅 2021-09-06 - Accurate sums and dot products for Python.
  (Python, GPL 3, GitHub)
* [GSL](https://www.gnu.org/software/gsl/) - Random number generators, special functions, and least-squares fitting etc.
  (C/C++, GPL 3, [Savannah](https://savannah.gnu.org/projects/gsl))
* [SLEPc](https://slepc.upv.es) - Scalable Library for Eigenvalue Problem Computations.
  (C, 2-clause BSD, [GitLab](https://gitlab.com/slepc/slepc))
* [preCICE](https://precice.org/) - Coupling library for partitioned multi-physics simulations (FSI, CHT, and more).
  (C++, LGPL 3, [GitHub](https://github.com/precice/))

## Community

* [SciComp StackExchange](https://scicomp.stackexchange.com/) - Computational Science on the StackExchange network.
* [Wolfgang Bangerth's video class](https://www.math.colostate.edu/~bangerth/videos.html) - MATH 676: Finite element methods in scientific computing.
* [Nick Higham's blog](https://nhigham.com/) - Mostly on MATLAB, general computing advice.
* [Nick Trefethen's Video Lectures](https://people.maths.ox.ac.uk/trefethen/videos.html) - 36 video lectures on approximation theory/practice and scientific computing.
* [John D. Cook's blog](https://www.johndcook.com/blog/) - Feats of scientific computing.
* [Jack Dongarra's software list](https://netlib.org/utk/people/JackDongarra/la-sw.html) - List of freely available software for the solution of linear algebra problems.
* [NA Digest](https://netlib.org/na-digest-html/) - Collection of articles on topics related to numerical analysis and those who practice it.
* [Gabriel Peyré on Bluesky](https://bsky.app/profile/gabrielpeyre.bsky.social) - One post a day on computational mathematics.
* [Discord: Numerical Software](https://discord.com/invite/hnTJ5MRX2Y) - Discord messaging server on numerical software.

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-19._
