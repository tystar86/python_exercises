#1. 
>Write a function for binary search. 
* Binary Search : In computer science, a binary search or half-interval search algorithm finds the position of a target value within a sorted array. The binary search algorithm can be classified as a dichotomies divide-and-conquer search algorithm and executes in logarithmic time.

**Test Data :**
```
binary_search([1,2,3,5,8], 6) -> False
binary_search([1,2,3,5,8], 5) -> True
```

#2. 
>Write a function for sequential search.
Sequential Search : In computer science, linear search or sequential search is a method for finding a particular value in a list that checks each element in sequence until the desired element is found or the list is exhausted. The list need not be ordered.

**Test Data :**
```
Sequential_Search([11,23,58,31,56,77,43,12,65,19],31) -> (True, 3) 
```

#3. 
>Write a function for binary search for an ordered list.

**Test Data :**
```
Ordered_binary_Search([0, 1, 3, 8, 14, 18, 19, 34, 52], 3) -> True
Ordered_binary_Search([0, 1, 3, 8, 14, 18, 19, 34, 52], 17) -> False 
```

#4. 
>Write a function to sort a list of elements using the bubble sort algorithm.

**Note:** According to Wikipedia "Bubble sort, sometimes referred to as sinking sort, is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares each pair of adjacent items and swaps them if they are in the wrong order. The pass through the list is repeated until no swaps are needed, which indicates that the list is sorted. The algorithm, which is a comparison sort, is named for the way smaller elements "bubble" to the top of the list. Although the algorithm is simple, it is too slow and impractical for most problems even when compared to insertion sort. It can be practical if the input is usually in sort order but may occasionally have some out-of-order elements nearly in position."
* Sample Data: ```[14,46,43,27,57,41,45,21,70]```
* Expected Result: ```[14, 21, 27, 41, 43, 45, 46, 57, 70]```

#5. 
>Write a function to sort a list of elements using the selection sort algorithm.

**Note:** The selection sort improves on the bubble sort by making only one exchange for every pass through the list. 
* Sample Data: ```[14,46,43,27,57,41,45,21,70]```
* Expected Result: ```[14, 21, 27, 41, 43, 45, 46, 57, 70]```

#6. 
>Write a function to sort a list of elements using the insertion sort algorithm.

**Note:** According to Wikipedia "Insertion sort is a simple sorting algorithm that builds the final sorted array (or list) one item at a time. It is much less efficient on large lists than more advanced algorithms such as quicksort, heapsort, or merge sort."
* Sample Data: ```[14,46,43,27,57,41,45,21,70]```
* Expected Result : ```[14, 21, 27, 41, 43, 45, 46, 57, 70]```

#7. 
>Write a function to sort a list of elements using shell sort algorithm.

**Note:** According to Wikipedia "Shell sort or Shell's method, is an in-place comparison sort. It can be seen as either a generalization of sorting by exchange (bubble sort) or sorting by insertion (insertion sort). The method starts by sorting pairs of elements far apart from each other, then progressively reducing the gap between elements to be compared. Starting with far apart elements can move some out-of-place elements into position faster than a simple nearest neighbor exchange."

#8. 
>Write a function to sort a list of elements using the merge sort algorithm.

**Note:** According to Wikipedia "Merge sort (also commonly spelled mergesort) is an O(n log n) comparison-based sorting algorithm. Most implementations produce a stable sort, which means that the implementation preserves the input order of equal elements in the sorted output."

#9. 
>Write a function to sort a list of elements using the quick sort algorithm. 

**Note:** According to Wikipedia "Quicksort is a comparison sort, meaning that it can sort items of any type for which a "less-than" relation (formally, a total order) is defined. Inefficient implementations it is not a stable sort, meaning that the relative order of equal sort items is not preserved. Quicksort can operate in-place on an array, requiring small additional amounts of memory to perform the sorting."

#10. 
>Write a function for counting sort. 

**Note:** According to Wikipedia "In computer science, counting sort is an algorithm for sorting a collection of objects according to keys that are small integers; that is, it is an integer sorting algorithm. It operates by counting the number of objects that have each distinct key value, and using arithmetic on those counts to determine the positions of each key value in the output sequence. Its running time is linear in the number of items and the difference between the maximum and minimum key values, so it is only suitable for direct use in situations where the variation in keys is not significantly greater than the number of items. However, it is often used as a subroutine in another sorting algorithm, radix sort, that can handle larger keys more efficiently".
