
This repository contains a script that employs the parallel quicksort algorithm on a hypercube using MPI. At the outset, an unsorted list of elements is evenly distributed across multiple processes. As the algorithm progresses, the sorted list is efficiently distributed among processors based on their ranks, ensuring that each processor maintains a sorted list.
