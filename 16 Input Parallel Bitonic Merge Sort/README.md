# 16 Input Parallel Bitonic Merge Sort

This circuit performs a parallel bitonic merge sort on 16 inputs. The circuit sorts all 16 inputs in ascending order. This schematic was built entirely through basic hardware components such as registers, I/O pins, and multiplexers. Additionally, the data is collected and sorted within one clock cycle.

This type of parallel sort is especially important when considering GPU sorting procedures. GPUs mainly consist of SIMD (single instruction, multiple data) architecture which means that they are very proficient at performing instructions in parallel. Thus, the fastest possible parallel sort will be the fastest way to sort data on a GPU. The parallel bitonic merge sort is heavily used in GPU sorting for this reason and has a time complexity of O(log^2(n)).


Screenshot of the entire schematic
![image](https://user-images.githubusercontent.com/96373394/188299369-61f5e93f-8cfa-4134-9e55-e137bd91595b.png)

Screenshot of the left side of the schematic
![image](https://user-images.githubusercontent.com/96373394/188299719-a5d88d2c-f2fc-477a-95d9-aca3a3bccca1.png)

Screenshot of the right side of the schematic
![image](https://user-images.githubusercontent.com/96373394/188299818-c5b29ce6-5c7d-4319-b311-0b76b201d0e3.png)

Screenshot of the subcircuit used to find maximum and minimums
![image](https://user-images.githubusercontent.com/96373394/188299831-a0c3b373-0720-4382-a848-79741e3c9608.png)

Further Reading: 

https://en.wikipedia.org/wiki/Bitonic_sorter

https://developer.nvidia.com/gpugems/gpugems2/part-vi-simulation-and-numerical-algorithms/chapter-46-improved-gpu-sorting
                 
https://people.scs.carleton.ca/~dehne/teaching/4009/lectures/pdf/05c-Parallel_bitonic_sort.pdf
                 
