Permutation Sort

BogoSort also known as permutation sort, stupid sort, slow sort, shotgun sort or monkey sort is a particularly ineffective algorithm based on generate and test paradigm. The algorithm successively generates permutations of its input until it finds one that is sorted.(Wiki)
For example, if bogosort is used to sort a deck of cards, it would consist of checking if the deck were in order, and if it were not, one would throw the deck into the air, pick the cards up at random, and repeat the process until the deck is sorted.

PseudoCode:

while not Sorted(list) do

shuffle (list)

done

Example:

Let us consider an example array ( 3 2 5 1 0 4 )

4 5 0 3 2 1 (1st shuffling)

4 1 3 2 5 0 (2ndshuffling)

1 0 3 2 5 4 (3rd shuffling)

3 1 0 2 4 5 (4th shuffling)

1 4 5 0 3 2 (5th shuffling)

.
.
.

0 1 2 3 4 5 (nth shuffling)—— Sorted Array

Here, n is unknown because algorithm doesn’t known in which step the resultant permutation will come out to be sorted.

Time Complexity:

Worst Case : O(∞) (since this algorithm has no upper bound)

Average Case: O(n*n!)

Best Case : O(n)(when array given is already sorted)

Auxiliary Space : O(1)