Binary Insertion Sort

We can use binary search to reduce the number of comparisons in normal insertion sort. Binary Insertion Sort uses binary search to find the proper location to insert the selected item at each iteration.
In normal insertion sort, it takes O(n) comparisons (at nth iteration) in the worst case. We can reduce it to O(log n) by using binary search.

Time Complexity: The algorithm as a whole still has a running worst-case running time of O(n2) because of the series of swaps required for each insertion. 