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
**Idea of how it works:** Like Merge Sort, QuickSort is a Divide and Conquer algorithm. An array is divided into subarrays by selecting a pivot element (element selected from the array).
While dividing the array, the pivot element should be positioned in such a way that elements less than pivot are kept on the left side and elements greater than pivot are on the right side of the pivot.
The left and right subarrays are also divided using the same approach. This process continues until each subarray contains a single element.

**Complexity (worst case and best case):** The worst case occurs when the partition process always picks greatest or smallest element as pivot.  O(n^2)
The best case occurs when the partition process always picks the middle element as pivot. Following is recurrence for best case.  O(nLogn).

**Additional data, in-place, kind of algorithm:**

**Explain partitioning in quick sort:** Target of partitions is, given an array and an element x of array as pivot, put x at its correct position in sorted array and put all smaller elements (smaller than x) before x, and put all greater elements (greater than x) after x. All this should be done in linear time.

h.Quick Selecti.Idea of how it works (General Pattern). 

ii.Complexity of the algorithm (worst case and best case). 

iii.If it’s an in-place/requires additional data structure kind of algorithm.

## Stack

**General explanation of the data structure:** A stack is a linear data structure that follows the principle of Last In First Out (LIFO). This means the last element inserted inside the stack is removed first.

**Operations used on stack: Push, Pop, Empty(have to mention how they work/their concept):** We can check if the stack is empty or not by using "Empty?" operation. Push: Adds an item in the stack. If the stack is full, then it is said to be an Overflow condition.
op: Removes an item from the stack. The items are popped in the reversed order in which they are pushed. If the stack is empty, then it is said to be an Underflow condition
time complexity if O(1) for all operations

**Implementation of the stack handling the operations and empty case:**

## Queue

**General explanation of the data structure:** A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). A good example of a queue is any queue of consumers for a resource where the consumer that came first is served first. The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.

**Operations used on queue: Enqueue, Dequeue(have to mention how they work/their concept):** Enqueue is the operation of adding an element to the structure, which is added at the end of the structure (Rear). Dequeue is the operation of removing the first element, which is located in the Front. Time complexity if O(1) for all operations

**Implementation of the stack handling the operations and empty case:**


## Linked Lists

**General explanation of the data structure:** A linked list is a linear data structure, in which the elements are not stored at contiguous memory locations. The elements in a linked list are linked using pointers.

**Types of linked lists with their description:**
 * Singly Linked List: A singly linked list is a unidirectional linked list. So, you can only traverse it in one direction
 * Doubly Linked List: A doubly linked list is a bi-directional linked list. So, you can traverse it in both directions. Unlike singly linked lists, its nodes contain one extra pointer called the previous pointer.
 * Circular Linked List: A circular Linked list is a unidirectional linked list. So, you can traverse it in only one direction. But this type of linked list has its last node pointing to the head node
 * Circular Doubly Linked List: A circular doubly linked list is a mixture of a doubly linked list and a circular linked list. Like the doubly linked list, it has an extra pointer called the previous pointer, and similar to the circular linked list, its last node points at the head node. This type of linked list is the bi-directional list. So, you can traverse it in both directions.

**Operations used on linked lists: Search, Insertion, Delete (have to mention how they work/their concept and their complexities):**
 * Insertion at the beginning: Since there is no need to find the end of the list. If the list is empty, we make the new node as the head of the list. Otherwise, we we have to connect the new node to the current head of the list and make the new node, the head of the list.
 * Insertion at end: We will traverse the list until we find the last node. Then we insert the new node to the end of the list. Note that we have to consider special cases such as list being empty.
In case of a list being empty, we will return the updated head of the linked list because in this case, the inserted node is the first as well as the last node of the linked list.
 * Insertion after a given node: We are given the reference to a node, and the new node is inserted after the given node. The previous node is linked to the given node, and the given node is linked to the next node.
 * Deletion: Find the previous node of the node to be deleted. Change the next pointer of the previous node. Free the memory of the deleted node.
 * Search: To search any value in the linked list, we can traverse the linked list and compares the value present in the node.

**Implementation of the stack handling the operations and empty case:**

**Double Linked lists with sentinel: General idea -> with empty -> Search -> Insert -> Delete:**: Sentinel nodes do not store any data in them. They are usually placed at the head & tail of a linked list. 
1. They reduce complexity of the algorithm.
2. They increase operational speed.
3. They increase robustness of the data structure which use them.

	
## Binary Search Trees

**General explanation of the data structure:** Data structure where the date is organized in a binary search tree using pointers.

**Pointers used with it:** A binary tree is made of nodes, where each node contains a "left" pointer, a "right" pointer, and a data element. The "root" pointer points to the topmost node in the tree. The left and right pointers recursively point to smaller "subtrees" on either side. A null pointer represents a binary tree with no elements -- the empty tree. The formal recursive definition is: a binary tree is either empty (represented by a null pointer), or is made of a single node, where the left and right pointers (recursive definition ahead) each point to a binary tree.

**Its property:** The left subtree of a node contains only nodes with keys lesser than the node’s key.
The right subtree of a node contains only nodes with keys greater than the node’s key.
The left and right subtree each must also be a binary search tree.

**Traversals: General idea of how each traversal works with BST:**
 * In this traversal method, the left subtree is visited first, then the root and later the right sub-tree. We should always remember that every node may represent a subtree itself.

 * In this traversal method, the root node is visited first, then the left subtree and finally the right subtree.

 * In this traversal method, the root node is visited last, hence the name. First we traverse the left subtree, then the right subtree and finally the root node.


**Operations for BST: Search, Min, Max, Previous, Next, Insert, Delete (have to mention how they work/their concept and their complexities):**

* Search: The algorithm depends on the property of BST that if each left subtree has values below root and each right subtree has values above the root.
If the value is below the root, we can say for sure that the value is not in the right subtree; we need to only search in the left subtree and if the value is above the root, we can say for sure that the value is not in the left subtree; we need to only search in the right subtree.
O(n)

* Insert: Inserting a value in the correct position is similar to searching because we try to maintain the rule that the left subtree is lesser than root and the right subtree is larger than root.
We keep going to either right subtree or left subtree depending on the value and when we reach a point left or right subtree is null, we put the new node there. O(n)

 * Delete: There are three cases for deleting a node from a binary search tree. 
   * In the first case, the node to be deleted is the leaf node. In such a case, simply delete the node from the tree.
   * In the second case, the node to be deleted lies has a single child node. In such a case follow the steps below:
     * Replace that node with its child node:
     * Remove the child node from its original position.

   * In the third case, the node to be deleted has two children. In such a case follow the steps below:
     * Get the inorder successor of that node.
     * Replace the node with the inorder successor.
     * Remove the inorder successor from its original position.   O(n)

* Min: This is quite simple. Just traverse the node from root to left recursively until left is NULL. The node whose left is NULL is the node with minimum value. 
O(n) Worst case happens for left skewed trees.

* Max: Similarly we can get the maximum value by recursively traversing the right node of a binary search tree.
couldnt find next and previous

**Know the best and worst shapes for BST*:*

## Priority Queue

**General explanation of the data structure:**
Priority Queue is an abstract data type, which is similar to a queue, however, in the priority queue, every element has some priority. Every item has a priority associated with it. An element with high priority is dequeued before an element with low priority. If two elements have the same priority, they are served according to their order in the queue.

**Operations for priority queue: insertion, deletion(with complexities)**
 * Insertion: 	O(log n). When a new element is inserted in a priority queue, it moves to the empty slot from top to bottom and left to right. However, if the element is not in the correct place then it will be compared with the parent node. If the element is not in the correct order, the elements are swapped. The swapping process continues until all the elements are placed in the correct position.
 * Deletion: 	O(log n). As you know that in a max heap, the maximum element is the root node. And it will remove the element which has maximum priority first. Thus, you remove the root node from the queue. This removal creates an empty slot, which will be further filled with new insertion. Then, it compares the newly inserted element with all the elements inside the queue to maintain the heap invariant.

**Explain trick on how to delete the maximum element:** Assign priority according to value, then apply Delate according to descending order

## Hashing

**General:** Hashing is a technique or process of mapping keys, values into the hash table by using a hash function. It is done for faster access to elements. The efficiency of mapping depends on the efficiency of the hash function used. 

**Chaining**

 1. General explanation
Chaining is a technique used for avoiding collisions in hash tables.
A collision occurs when two keys are hashed to the same index in a hash table. Collisions are a problem because every slot in a hash table is supposed to store a single element.

 2. Operations used with it and their complexities
In the chaining approach, the hash table is an array of linked lists i.e., each index has its own linked list. All key-value pairs mapping to the same index will be stored in the linked list of that index. insertion in a hash table always occurs in O(1)


|ACTIVITY |	BEST CASE  COMPLEXITY |	AVERAGE CASE COMPLEXITY |	WORST CASE COMPLEXITY |
| --- | --- | --- | --- |
|Searching |	O(1) |	O(1) |	O(n) |
|Insertion |	O(1) |	O(1) |	O(n) |
|Deletion |	O(1) |	O(1) |	O(n) |
|Space Complexity |	O(m+n) |	O(m+n) |	O(m+n) |

 3. Division Method
The most common method is the division method, in which modular arithmetic is used in computing the slot. h(k) = M mod N

 4. Multiplication Method
Multiplicative hashing sets the hash index from the fractional part of multiplying k by a large real number. It's faster if this computation is done using fixed point rather than floating point, which is accomplished by computing (ka/2^q) mod m for appropriately chosen integer values of a, m, and q. So q determines the number of bits of precision in the fractional part of a.
	
**Opening Addressing:**

1. General explanation
In case of obtain an already used index of the array, we can search the next empty location in the array by looking into the next cell until we find an empty cell. This technique is called linear probing.

2. Operations: Insert, Search, Delete.

|ACTIVITY |	BEST CASE  COMPLEXITY |	AVERAGE CASE COMPLEXITY |	WORST CASE COMPLEXITY |
| --- | --- | --- | --- |
|Searching |	O(1) |	O(1) |	O(n) |
|Insertion |	O(1) |	O(1) |	O(n) |
|Deletion |	O(1) |	O(1) |	O(n) |
|Space Complexity |	O(n) |	O(n) |	O(n) |

**Linear Hashing:** Suppose the hash function is denoted by h(n). Then, for a value k, if the hash generated h(k) is occupied, linear probing suggests to look at the very next location i.e. h(k)+1. When this is occupied as well, we look at h(k)+2, h(k)+3, h(k)+4 and so on... 

**Quadratic Hashing:** Very similar to linear probing discussed above, this method of collision resolution searches for the next vacant space by taking steps in the order of i2 where i = 1, 2, 3...
So, the table is traversed in the order h(k)+1, h(k)+4, h(k)+9, h(k)+16 and so on.

**Double Hashing:** In this method, we use two hashing functions- h(n) for general hashing and and a new function h'(n) used specifically for resolving conflicts.
So, vacancies are searched in the order as h(k), h(k) + h'(k), h(k) + 2h'(k) and so on...
