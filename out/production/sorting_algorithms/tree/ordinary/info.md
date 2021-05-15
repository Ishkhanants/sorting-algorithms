Tree Sort

Tree sort is a sorting algorithm that is based on Binary Search Tree data structure. It first creates a binary search tree from the elements of the input list or array and then performs an in-order traversal on the created binary search tree to get the elements in sorted order.

Algorithm:

Step 1: Take the elements input in an array.

Step 2: Create a Binary search tree by inserting data items from the array into the
binary search tree.

Step 3: Perform in-order traversal on the tree to get the elements in sorted order.

Average Case Time Complexity : O(n log n) 

Adding one item to a Binary Search tree on average takes O(log n) time. Therefore, adding n items will take O(n log n) time

Worst Case Time Complexity : O(n2). The worst case time complexity of Tree Sort can be improved by using a self-balancing binary search tree like Red Black Tree, AVL Tree. Using self-balancing binary tree Tree Sort will take O(n log n) time to sort the array in worst case.

Auxiliary Space : O(n)