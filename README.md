### C++ solver for the 2D wave equation through hetergenous media with MPI parallelization.
Primary author: Nicholas Geneva (ngeneva at nd.edu)
Co-authors: Govinda Anantha Padmanabha, Qing Lan

Dependiencies:
MPI (intel or ompi)
Boost

To compile in parallel: 
mpicxx *cpp -std=c++11 -lboost_system -lboost_filesystem  -D__MPI__

To run:
mpirun -np <num of procs> ./a.out

Simulation parameters can be modified in main.cpp lines 25-40
Source term can be modified line 58-62

To generate different permeability fields use perm_gen.m in perm_gen folder.
Requires matlab. Note that the perm field must match the simulation discretization!!!
