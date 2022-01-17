a.Sorting definition in general.

In computer science, a sorting algorithm is an algorithm that puts elements of a list into an order, most frequenfly by numerical or lexicographical order, and either ascending or descending. 

b.Bubble Sort

	i.Idea of how it works.
Bubble Sort is the simplest sorting algorithm that works by repeatedly swapping the adjacent elements if they are in wrong order.
	ii.Complexity of the algorithm (worst case).
O(n*n). Worst case occurs when array is reverse sorted. Minimum time (Order of n) when elements are already sorted.
	iii.If it’s an in-place/requires additional data structure kind of algorithm. 
Auxiliary Space: O(1), Sorting In Place, Stable

c.Insertion Sort

	i.Idea of how it works.
The array is virtually split into a sorted and an unsorted part. Values from the unsorted part are picked and placed at the correct position in the sorted part.
	ii.Complexity of the algorithm (worst case). 
O(n^2). Worst case occurs when array is reverse sorted. Minimum time (Order of n) when elements are already sorted.
	iii.If it’s an in-place/requires additional data structure kind of algorithm. 
Auxiliary Space: O(1), Sorting In Place, Stable
	
d.Selection Sort

	i.Idea of how it works.
The array is virtually split into a sorted and an unsorted part. The selection sort algorithm sorts an array by repeatedly finding the minimum element (considering ascending order) from unsorted part and putting it at the beginning. 
	ii.Complexity of the algorithm (worst case)
O(n2) as there are two nested loops.
	iii.If it’s an in-place/requires additional data structure kind of algorithm. 
In Place : Yes, it does not require extra space. Auxiliary Space: O(1) 
	
e.Merge Sort
	i.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
	iv.Merge and its complexityv.Brief explanation of why/how sentinel is used.
	vi.No explanation of how to get to the complexity is needed
f.Heap Sort
	i.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
	iv.How is max selection sort related to heap sort. Brief explanation of how it works
	v.Preprocessing related in heap sort
	vi.Resorting heap property
	vii.Tree property related to building a heap.
	viii.What is heapify? What is its complexity?
	ix.Why is heap sort an asymptotically sorting algorithm?
g.Quick Sort
	i.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case and best case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
	iv.Explain partitioning in quick sort.
	h.Quick Selecti.Idea of how it works (General Pattern). 
	ii.Complexity of the algorithm (worst case and best case). 
	iii.If it’s an in-place/requires additional data structure kind of algorithm.
i.Stack
	i.Generl explanation of the data structure.
	ii.Operations used on stack: Push, Pop, Empty(have to mention how they work/their concept)
	iii.Implementation of the stack handling the operations and empty case
j.Queue
	i.General explanation of the data structure.
	ii.Operations used on queue: Enqueue, Dequeue(have to mention how they work/their concept)
	iii.Implementation of the stack handling the operations and empty case
k.Linked Lists
	i.General explanation of the data structure.
	ii.Types of linked lists with their description
	iii.Operations used on linked lists: Search, Insertion, Delete (have to mention how they work/their concept and their complexities)
	iv.Implementation of the stack handling the operations and empty case
	v.Double Linked lists with sentinel: General idea -> with empty -> Search -> Insert -> Delete
l.Binary Search Trees
	i.General explanation of the data structure.
	ii.Pointers used with it
	iii.Its property
	iv.Traversals: General idea of how each traversal works with BST (no need for mentioning example if concept of each is properly explained)
	v.Operations for BST: Search, Min, Max, Previous, Next, Insert, Delete (have to mention how they work/their concept and their complexities)
	vi.Know the best and worst shapes for BST
m.Priority Queue
	i.General explanation of the data structure.
	ii.Operations for priority queue: insertion, deletion(with complexities)
	iii.Explain trick on how to delete the maximum element
n.Hashing
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
