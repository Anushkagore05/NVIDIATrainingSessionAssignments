Searching and Sorting — Complexity Notes

1. Bubble Sort

Best case: O(n) — When the array is already sorted and we use a swap flag.

Average case: O(n²) — When the elements are in random order.

Worst case: O(n²) — When the array is sorted in reverse order.

Space: O(1) — It uses only a few extra variables.

Stable: Yes — Equal elements do not change their relative order.

In-place: Yes — Sorting is done in the same array.

Why: It compares adjacent elements and swaps them if they are in the wrong order.

2. Insertion Sort

Best case: O(n) — When the array is already sorted.

Average case: O(n²) — When the elements are in random order.

Worst case: O(n²) — When the array is sorted in reverse order.

Space: O(1) — It uses only a few extra variables.

Stable: Yes — Equal elements keep their relative order.

In-place: Yes — It sorts the same array.

Why: It takes one element at a time and inserts it into its correct position in the sorted part.

3. Selection Sort

Best case: O(n²) — Even if the array is already sorted, it checks the remaining elements.

Average case: O(n²) — It searches for the minimum element in every pass.

Worst case: O(n²) — It still checks all remaining elements in every pass.

Space: O(1) — It uses only a few extra variables.

Stable: No — Swapping elements can change the relative order of equal elements.

In-place: Yes — It sorts the same array.

Why: It selects the smallest element from the unsorted part and puts it in the correct position.

4. Merge Sort

Best case: O(n log n) — The array is divided and merged at every level.

Average case: O(n log n) — It divides the array into smaller parts and merges them.

Worst case: O(n log n) — The number of levels and work at each level remain similar.

Space: O(n) — It needs temporary arrays and O(log n) recursion stack space.

Stable: Yes — If equal elements are taken from the left half first.

In-place: No — The usual array implementation requires extra memory.

Why: It divides the array into halves, sorts them and merges the sorted halves.

5. Quick Sort

Best case: O(n log n) — When the pivot divides the array into nearly equal parts.

Average case: O(n log n) — When the pivot usually creates reasonably balanced partitions.

Worst case: O(n²) — When the pivot repeatedly gives highly unbalanced partitions, such as one element and the rest.

Space: O(log n) on average for the recursion stack; O(n) in the worst case. Partitioning itself uses O(1) extra space.

Stable: No — Swapping elements during partitioning can change the relative order of equal elements.

In-place: Yes — The usual partitioning algorithm sorts within the same array, apart from recursion stack space.

Why: It chooses a pivot, partitions the array around it and sorts the two parts recursively.

Quick Sort: O, Ω and Θ

O(n²): Worst-case upper bound when partitions are highly unbalanced.

Ω(n log n): Best-case lower bound when partitions are balanced.

Θ(n log n): Tight bound for balanced partitions and the usual average-case growth.

6. Linear Search

Best case: O(1) — The element is at the first position.

Average case: O(n) — The element is usually found after checking several elements.

Worst case: O(n) — The element is at the last position or is not present.

Space: O(1) — It uses only a few extra variables.

Stable: Not applicable — Stability is generally used for sorting algorithms.

In-place: Yes — It does not modify the array and uses constant extra space.

Why: It checks each element one by one until the target is found.

7. Binary Search

Best case: O(1) — The target is the middle element.

Average case: O(log n) — The search space is reduced by half after each comparison.

Worst case: O(log n) — It keeps dividing the search space until the element is found or the range becomes empty.

Space: O(1) for iterative binary search; O(log n) for recursive binary search because of the recursion stack.

Stable: Not applicable — Stability is generally used for sorting algorithms.

In-place: Yes — The iterative version uses constant extra space and does not modify the array.

Why: It compares the target with the middle element and eliminates half of the search space each time.
