Sleep Sort – The King of Laziness / Sorting while Sleeping

Difficulty Level : Medium

In this algorithm we create different threads for each of the elements in the input array and then each thread sleeps for an amount of time which is proportional to the value of corresponding array element.

Hence, the thread having the least amount of sleeping time wakes up first and the number gets printed and then the second least element and so on. The largest element wakes up after a long time and then the element gets printed at the last. Thus the output is a sorted one.

All this multithreading process happens in background and at the core of the OS. We do not get to know anything about what’s happening in the background, hence this is a “mysterious” sorting algorithm.

Example : Let’s assume (for convenience) we have a computer that’s so slow it takes 3 seconds to work through each element:

INPUT: 8 2 9

3s: sleep 8

6s: sleep 2

8s: "2" (2 wakes up so print it)

9s: sleep 9

11s: "8" (8 wakes up so print it)

18s: "9" (9 wakes up so print it)

OUTPUT: 2 8 9

Implementation

To implement sleep sort, we need multithreading functions, such as _beginthread() and WaitForMultipleObjects(). Hence we need to include windows.h to use these functions. This won’t compile on Online IDE. We must run it in your PC (Note this code is for WINDOWS and not for LINUX).

To perform a sleep sort we need to create threads for each of the value in the input array. We do this using the function _beginthread().

In each of the threads we assign two instructions:

1) Sleep : Sleep this thread till arr[i] milliseconds (where arr[i] is the array element which this thread is associated to). We do this using Sleep() function. The Sleep(n) function suspends the activity associated with this thread till ‘n’ milliseconds. Hence if we write Sleep(1000), then it means that the thread will sleep for 1 second (1000 milliseconds = 1 second)

2) Print : When the thread ‘wakes’ up after the sleep then print the array element – arr[i] which this thread is associated to.

After creating the threads, we process these threads. We do this using WaitForMultipleObjects().

