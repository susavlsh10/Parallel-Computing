Parallel Merge Sort using openmp

![Parallel Merge Sort](https://github.com/susavlsh10/Parallel-Computing/blob/main/images/MergeSort.png)


To compile and execute the code, use the commands:

icc -qopenmp -o sort_list_openmp.exe sort_list_openmp.c
./sort_list_openmp.exe k q

where k and q are integer arguments that specify the number of elements in the list n = 2^𝑘, and the number of threads p = 2^𝑞.


The following graph shows the speedup vs q for different values of n.

![speedup vs q](https://github.com/susavlsh10/Parallel-Computing/blob/main/Parallel%20Merge%20Sort%20using%20openmp/Speedup.png)

The following graph shows the efficiency vs q for different value of n.

![efficiency vs q](https://github.com/susavlsh10/Parallel-Computing/blob/main/Parallel%20Merge%20Sort%20using%20openmp/Efficiency.png)
