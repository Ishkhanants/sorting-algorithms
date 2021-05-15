Given a list of items, sort them in increasing order.

Examples:

Input : ip[] = {10, 5, 30, 40, 2, 4, 9}

Output : op[] = {2, 4, 5, 9, 10, 30, 40}

Input : ip[] = {1, 10, 7}

Output : op[] = {1, 7, 10}

Strand Sort is a sorting algorithm that works in O(n) time if list is already sorted and works in O(n*n) in worst case.

Below are simple steps used in the algorithm.

Let ip[] be input list and op[] be output list.

Create an empty sublist and move first item of ip[] to it.

Traverse remaining items of ip. For every item x, check if x is greater than last inserted item to sublist. If yes, remove x from ip and add at the end of sublist. If no, ignore x (Keep it it in ip)

Merge sublist into op (output list)

Recur for remaining items in ip and current items in op.

Let ip[] = {10, 5, 30, 40, 2, 4, 9}

Initialize : op[] = {}

sublist[] = {}

Move first item of ip to sublist.

sublist[] = {10}

Traverse remaining items of ip and

if current element is greater than

last item of sublist, move this item

from ip to sublist. Now

sublist[] = {10, 30, 40}

ip[] = {5, 2, 4, 9}

Merge sublist into op.

op = {10, 30, 40}

Next recursive call:

Move first item of ip to sublist.

sublist[] = {5}

Traverse remaining items of ip and move

elements greater than last inserted.

ip[] = {2, 4}

sublist[] = {5, 9}

Merge sublist into op.

op = {5, 9, 10, 30, 40}

Last Recursive Call:

{2, 4} are first moved to sublist and

then merged into op.

op = {2, 4, 5, 9, 10, 30, 40}

