#  Parallel_Sorting

# Task
Your task is to implement a parallel sorting algorithm such that each partition of the array is sorted in parallel. You will consider two different schemes for deciding whether to sort in parallel.
1.	A cutoff (defaults to, say, 1000) which you will update according to the first argument in the command line when running. It's your job to experiment and come up with a good value for this cutoff. If there are fewer elements to sort than the cutoff, then you should use the system sort instead.
2.	Recursion depth or the number of available threads. Using this determination, you might decide on an ideal number (t) of separate threads (stick to powers of 2) and arrange for that number of partitions to be parallelized (by preventing recursion after the depth of lg t is reached).
3.	An appropriate combination of these.

# RELATIONSHIP CONCLUSION:
Comparing the above graphs and data from the tables, we can conclude the following: 
• After changing the cutoff values and number of threads for different array sizes, the number of threads bigger than 8 does not improve the performance of the algorithm. Hence forking 8 threads is the best option. 
• Referring to the graphs above, we can see that the optimal performance is seen around ~25% of the array size. With this, we can conclude that this leads to least algorithm performance time.
