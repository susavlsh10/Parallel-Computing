
This repository contains a script that employs the parallel quicksort algorithm on a hypercube using MPI. At the outset, an unsorted list of elements is evenly distributed across multiple processes. As the algorithm progresses, the sorted list is efficiently distributed among processors based on their ranks, ensuring that each processor maintains a sorted list.

Compile the code using the following command.

mpiicpc -o qsort_hypercube.exe qsort_hypercube.cpp

To execute the program, use

mpirun –np &lt;p&gt; ./qsort_hypercube.exe &lt;n&gt;n &lt;type&gt;

where p is the number of MPI processes, n is the size of the local list of each MPI process, and type is the method used to initialize the local list.
