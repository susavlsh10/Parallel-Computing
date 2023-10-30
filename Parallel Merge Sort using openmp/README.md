Parallel Merge Sort using openmp

![Parallel Merge Sort](https://github.com/susavlsh10/Parallel-Computing/blob/main/images/MergeSort.png)


To compile and execute the code, use the commands:

icc -qopenmp -o sort_list_openmp.exe sort_list_openmp.c
./sort_list_openmp.exe k q

where k and q are integer arguments that specify the number of elements in the list n = 2^𝑘, and the number of threads p = 2^𝑞.


The following graph shows the speedup vs q for different values of k.

![speedup vs q](https://github.com/susavlsh10/Parallel-Computing/blob/main/Parallel%20Merge%20Sort%20using%20openmp/Speedup.png)

The following graph shows the efficiency vs q for different value of k.

![efficiency vs q](https://github.com/susavlsh10/Parallel-Computing/blob/main/Parallel%20Merge%20Sort%20using%20openmp/Efficiency.png)

Analysis

The data illustrates the speedup ratios for parallel execution of merge sort using OpenMP, comparing it to sequential execution across various values of k and q. The speedup ratio, defined as single-thread time divided by multi-thread time, displays certain trends. For fixed k, the ratio generally rises with increasing q until it peaks, after which it declines. This suggests that adding more threads enhances performance up to a point, beyond which it introduces inefficiency. Similarly, for a constant q, the speedup ratio typically increases as k grows, emphasizing the benefit of parallelization for larger list sizes. 

The data depicts the efficiency of OpenMP parallel merge sort compared to sequential execution across various k and q values. Efficiency is the speedup ratio divided by the number of threads, indicating how well threads are utilized and the level of overhead incurred. For fixed k, efficiency typically decreases as q increases, indicating that more threads reduce individual thread performance and increase overhead. Conversely, for fixed q, efficiency generally rises with higher k, implying larger list sizes benefit from greater performance per thread and reduced overhead. The graph confirms these trends, showing efficiency declining as q increases and increasing with higher k or list size, aligning with expectations.





