Given an unsorted array, sort the given array. You are allowed to do only following operation on array.

flip(arr, i): Reverse array from 0 to i

Unlike a traditional sorting algorithm, which attempts to sort with the fewest comparisons possible, the goal is to sort the sequence in as few reversals as possible.

The idea is to do something similar to Selection Sort. We one by one place maximum element at the end and reduce the size of current array by one.
Following are the detailed steps. Let given array be arr[] and size of array be n.

Start from current size equal to n and reduce current size by one while it’s greater than 1. Let the current size be curr_size. Do following for every curr_size

Find index of the maximum element in arr[0..curr_szie-1]. Let the index be ‘mi’

Call flip(arr, mi)

Call flip(arr, curr_size-1)

