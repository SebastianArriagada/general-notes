## Sorting definition in general.

In computer science, a sorting algorithm is an algorithm that puts elements of a list into an order, most frequenfly by numerical or lexicographical order, and either ascending or descending. 

## Bubble Sort

**Idea of how it works:** Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in wrong order.

**Complexity (worst case):** O(n^2) Worst case occurs when array is reverse sorted. Minimum time O(n) when elements are already sorted.

**Additional data, in-place, kind of algorithm:** O(1), sorting In Place, stable.

## Insertion Sort

**Idea of how it works:** The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.

**Complexity (worst case):** O(n^2) Worst case occurs when array is reverse sorted. Minimum time O(n) when elements are already sorted.

**Additional data, in-place, kind of algorithm:** O(1), sorting in place, stable.
	
## Selection Sort

**Idea of how it works:** The array is virtually split into a sorted and an unsorted part. The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning. 

**Complexity (worst case):** O(n2) as there are two nested loops.

**Additional data, in-place, kind of algorithm:** O(1), in place (it does not require extra space), unestable
	
## Merge Sort

**Idea of how it works:** It divides the input array into two halves, calls itself for the two halves, till the size of each halve becomes 1. The merge() function is used for merging two halves. The merge(arr, l, m, r) is a key process that assumes that arr[l..m] and arr[m+1..r] are sorted and merges the two sorted sub-arrays into one.

**Complexity (worst case):** θ(nLogn) in all 3 cases (worst, average and best).

**Additional data, in-place, kind of algorithm:**  O(n), no in place, Divide and Conquer (It is the best Sorting technique used for sorting Linked Lists)

**Merge and its complexity:** O(n). Marge grow linear with the growth of number of sub-array

**Brief explanation of why/how sentinel is used:** The use of sentinels in merge sort prevents us from needing to check to see if we have reached the end of either of the arrays being sorted. Merge sort can be performed without a sentinel, but adds an additional check for every iteration of the comparison loop.

	
## Heap Sort

**Idea of how it works:**
1. Build a max heap from the input data. 
2. At this point, the largest item is stored at the root of the heap. Replace it with the last item of the heap followed by reducing the size of heap by 1. Finally, heapify the root of the tree. 
3. Repeat step 2 while the size of the heap is greater than 1.

**Complexity (worst case):** O(nLog n)

**Additional data, in-place, kind of algorithm:** no additional space needed, sort in-place, Comparison-base with Binary Heap data structure, no stable

**How is max selection sort related to heap sort. Brief explanation of how it works:** It is similar to selection sort where we first find the minimum element and place the minimum element at the beginning. We repeat the same process for the remaining elements.

**Preprocessing related in heap sort:** Is constructed a Binary Tree and apply the heapify 

**Resorting heap property:** Check the key stored in each node is either greater than or equal (≥) or less than or equal (≤) to the keys in the node's children, according to some total order.
	
**Tree property related to building a heap:** A Binary Heap is a Complete Binary Tree where items are stored in a special order such that the value in a parent node is greater(or smaller) than the values in its two children nod

**What is heapify? What is its complexity?** Heapify is the process of converting a binary tree into a Heap data structure. A binary tree being a tree data structure where each node has at most two child nodes. A Heap must be a complete binary tree, that is each level of the tree is completely filled, except possibly the bottom level. At this level, it is filled from left to right. Complexity O(nLog n)

**Why is heap sort an asymptotically sorting algorithm?** This mean that the algorithm require the same time for the worst and better case
	
## Quick Sort
	i.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case and best case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
	iv.Explain partitioning in quick sort.
	h.Quick Selecti.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case and best case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
## Stack
	i.Generl explanation of the data structure.
	ii.Operations used on stack: Push, Pop, Empty(have to mention how they work/their concept)
	iii.Implementation of the stack handling the operations and empty case
## Queue
	i.General explanation of the data structure.
	ii.Operations used on queue: Enqueue, Dequeue(have to mention how they work/their concept)
	iii.Implementation of the stack handling the operations and empty case
## Linked Lists
	i.General explanation of the data structure.
	ii.Types of linked lists with their description
	iii.Operations used on linked lists: Search, Insertion, Delete (have to mention how they work/their concept and their complexities)
	iv.Implementation of the stack handling the operations and empty case
	v.Double Linked lists with sentinel: General idea -> with empty -> Search -> Insert -> Delete
## Binary Search Trees
	i.General explanation of the data structure.
	ii.Pointers used with it
	iii.Its property
	iv.Traversals: General idea of how each traversal works with BST (no need for mentioning example if concept of each is properly explained)
	v.Operations for BST: Search, Min, Max, Previous, Next, Insert, Delete (have to mention how they work/their concept and their complexities)
	vi.Know the best and worst shapes for BST
## Priority Queue
	i.General explanation of the data structure.
	ii.Operations for priority queue: insertion, deletion(with complexities)
	iii.Explain trick on how to delete the maximum element
## Hashing
	i.General explanation
	ii.Chaining
		1.General explanation
		2.Operations used with it and their complexities
		3.Division Method
		4.Multiplication Method
	iii.Opening Addressing:
		1.General explanation
		2.Operations: Insert, Search, Delete.
	iv.Linear Hashing:  General Explanation
	v.Quadratic Hashing:  General Explanation
	vi.Double Hashing:  General Explanation
