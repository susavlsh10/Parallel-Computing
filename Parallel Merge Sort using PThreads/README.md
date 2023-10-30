Parallel Merge Sort using pthreads

![Parallel Merge Sort](https://github.com/susavlsh10/Parallel-Computing/blob/main/images/MergeSort.png)


This project involves enhancing the performance of merge sort using an iterative variant of the merge sort algorithm. The aim is to parallelize the sorting process to improve efficiency. Unlike the traditional recursive merge sort, this project adopts a bottom-up approach, iteratively merging adjacent elements and achieving parallelism at different levels of the sorting process. Each thread is responsible for determining the location of its sublist elements in the merged list and placing them directly in that location, resulting in a faster sorting algorithm. This directory implements the parallel merge sort using posix pthreads.



To compile and execute the code, use the commands:

icc -o sort_list.exe sort_list.c

./sort_list.exe k q

where k and q are integer arguments that specify the number of elements in the list n = 2^𝑘, and the number of threads p = 2^𝑞. 

