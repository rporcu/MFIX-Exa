MFiX-Exa Introduction
=====================

MFiX-Exa comes with its own Projection-Method based solver for the
Navier-Stokes equations, as well as the SIMPLE solver used by MFiX-Classic.
AMReX is used to manage the simulation's data. Hence, AMReX is also responsible
for MPI and openMP parallelization. In the future, AMReX's adaptive mesh
refinement (AMR) will also be supported by MFiX-Exa.

The code for now lives at NETL; instructions for how to get access to the code
will be given below.

Key features of MFiX-Exa include:

-  C++ and Fortran interfaces

-  Projection-Method based solver of the Nativer-Stokes Equations

-  Support for cell-centered, face-centered, edge-centered, and nodal data

-  Support for solid particles

-  Parallelization via flat MPI, OpenMP, hybrid MPI/OpenMP, or MPI/MPI

-  Parallel I/O

-  Plotfile format supported by AmrVis, VisIt, ParaView, and yt.

-  Complex container walls implemented as embedded boundaries, with efficient
   particle/wall interactions.

Besides this documentation, there is documentation generated by Doxygen at
https://amrex-codes.github.io/MFIX-Exa/doxygen.

.. toctree::
   :maxdepth: 1
   :caption: Contents:

   BuildingMFiX
   TestingMFiX


Directory overview
------------------

.. table:: Overview of the MFiX-Exa directory structure

    +------------+-----------------------------------------------------+
    | File       | Description                                         |
    +============+=====================================================+
    | benchmarks | UC Benchmark cases (see benchmark/README.md)        |
    +------------+-----------------------------------------------------+
    | src        | Fortran source files                                |
    +------------+-----------------------------------------------------+
    | tests      | Regression tests (see tests/README.md)              |
    +------------+-----------------------------------------------------+
    | ThirdParty | External libraries sources                          |
    +------------+-----------------------------------------------------+
    | Tools      | CMake configuration files                           |
    +------------+-----------------------------------------------------+