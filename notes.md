## Data Strcutures Overview

- Characteristics of Algorithms

    + **Unambiguous** − Algorithm should be clear and unambiguous. Each of its steps (or phases), and their input/outputs should be clear and must lead to only one meaning.
    + **Input** − An algorithm should have 0 or more well defined inputs.
    + **Output** − An algorithm should have 1 or more well defined outputs, and should match the desired output.
    + **Finiteness** − Algorithms must terminate after a finite number of steps.
    + **Feasibility** − Should be feasible with the available resources.
    + **Independent** − An algorithm should have step-by-step directions which should be independent of any programming code.

- Methods for analyzing algorithms:
    + **A priori analysis** − This is theoretical analysis of an algorithm. Efficiency of algorithm is measured by assuming that all other factors e.g. processor speed, are constant and have no effect on implementation.
    + **A posterior analysis** − This is empirical analysis of an algorithm. The selected algorithm is implemented using programming language. This is then executed on target computer machine. In this analysis, actual statistics like running time and space required, are collected.

- Algorithm Complexity: Time complexity and space factor

- Space Complexity (the amount of space required to execute the algorithm):
    + A fixed part that is a space required to store certain data and variables, that are independent of the size of the problem. For example simple variables & constant used, program size etc.
    + A variable part is a space required by variables, whose size depends on the size of the problem. For example dynamic memory allocation, recursion stack space etc.

- Time Complexity of an algorithm represents the amount of time required by the algorithm to run to completion. 

- Asymptotic analysis of an algorithm, refers to defining the mathematical boundation/framing of its run-time performance. Using asymptotic analysis, we can very well conclude the best case, average case and worst case scenario of an algorithm.

- Usually, time required by an algorithm falls under three types −
    + Best Case − Minimum time required for program execution.
    + Average Case − Average time required for program execution.
    + Worst Case − Maximum time required for program execution.

- Following are commonly used asymptotic notations used in calculating running time complexity of an algorithm.
    + **Ο Notation (Worst case)** - The Ο(n) is the formal way to express the upper bound of an algorithm's running time. It measures the worst case time complexity or longest amount of time an algorithm can possibly take to complete; `f(n) = O(g(n)) iff there exists c > 0 and n0 such that f(n) ≤ c.g(n) for all n, n ≥ n0.`
    
    + **Ω Notation (Best Case)** - The Ω(n) is the formal way to express the lower bound of an algorithm's running time. It measures the best case time complexity or best amount of time an algorithm can possibly take to complete; `f(n) = Ω(g(n)) iff there exists c > 0 and n0 such that f(n) ≥ c.g(n) for all n, n ≥ n0.`

    + **θ Notation (Average Case)**- The θ(n) is the formal way to express both the lower bound and upper bound of an algorithm's running time; `f(n) = θ(g(n)) iff g(n) is both an upper and lower bound on f(n) for all n , n > n0.`

- Greedy algorithms tries to find localized optimum solution which may eventually land in globally optimized solutions. But generally greedy algorithms do not provide globally optimized solutions.

- Greedy algorithms are different from divide and conquer algorithms in that the problem is divided into smaller sub-problems and them merged together to get final solution.

## Arrays

- Linked List is a sequence of links which contains items. Each link contains a connection to another link. Linked list the second most used data structure after array. Following are important terms to understand the concepts of Linked List.
    + Link − Each Link of a linked list can store a data called an element.
    + Next − Each Link of a linked list contain a link to next link called Next.
    + LinkedList − A LinkedList contains the connection link to the first Link called First.

- Following are the various flavours of linked list.
    + Simple Linked List − Item Navigation is forward only.
    + Doubly Linked List − Items can be navigated forward and backward way.
    + Circular Linked List − Last item contains link of the first element as next and and first element has link to last element as prev.

- Doubly Linked List is a variation of Linked list in which navigation is possible in both ways either forward and backward easily as compared to Single Linked List. Following are important terms to understand the concepts of doubly Linked List

- Circular Linked List is a variation of Linked list in which first element points to last element and last element points to first element. Both Singly Linked List and Doubly Linked List can be made into as circular linked list.

## Stacks:

- This feature makes it LIFO data structure. LIFO stands for Last-in-first-out. Here, the element which is placed (inserted or added) last, is accessed first. In stack terminology, insertion operation is called **PUSH** operation and removal operation is called **POP** operation; A stack can be implemented by means of Array, Structure, Pointer and Linked-List. Stack can either be a fixed size one or it may have a sense of dynamic resizing. Here, we are going to implement stack using arrays which makes it a fixed size stack implementation.

- **Notation** refers to the way an arithmetic expression is written.

- Three ways of writing notations:
    + **Infix Notation** - in between operands (e.g., `a-b+x`); An algorithm to process infix notation could be difficult and costly in terms of time and space consumption.
    + **Prefix (Polish) Notation** - In this notation, operator is prefixed to operands, i.e. operator is written ahead of operands. For example `+ab`. This is equivalent to its infix notation `a+b`. Prefix notation is also known as Polish Notation.
    + **Postfix (Reverse-Polish) Notation** - This notation style is known as Reversed Polish Notation. In this notation style, operator is postfixed to the operands i.e., operator is written after the operands. For example `ab+`. This is equivalent to its infix notation `a+b`.


- To parse any arithmetic expression and determine the order of evaluation of an expression, we need to take care of operator **precedence** and **associativity** also.

- Stacks are used to parse arithmetic expressions into prefix or postfix notation.

## Queue

- In contrast to Stack, queue is opened at both end. One end is always used to insert data (enqueue) and the other is used to remove data (dequeue). Queue follows First-In-First-Out methodology, i.e., the data item stored first will be accessed first.

- In queue, we always dequeue (or access) data, pointed by **front pointer** and while enqueing (or storing) data in queue we take help of **rear pointer**.

- In an Enqueue operation (using plain array structures), we are only accessing and changing **rear**; rear keeps incrementing as new items keep coming in so as to keep track of the last item.

- In a Dequeue operation (using plain array implementation), we are only accesing and changing **front**; front is incremented every time an item is accessed or deleted.

## Search Algorithms

- Linear search is a very simple search algorithm. In this type of search, a sequential search is made over all items one by one. Every items is checked and if a match founds then that particular item is returned otherwise search continues till the end of the data collection.

- Binary search is a fast search algorithm with run-time complexity of Ο(log n). This search algorithm works on the principle of divide and conquer. For this algorithm to work properly the data collection should be in sorted form; array must be sorted; find the middle and then compare if the that midpoint matches the searched item. Because it is dividing the search into two everytime the time complexity is logarithmic, given that the arrays is already sorted.

- Interpolation search - In contrast to binary and linear search, this type of search takes advantage of **probe position** capability; Runtime complexity of interpolation search algorithm is Ο(log (log n)) as compared to Ο(log n) of BST in favourable situations.

## Hash Tables

- Hash Table is a data structure which store data in associative manner. In hash table, data is stored in array format where each data values has its own unique index value. Access of data becomes very fast if we know the index of desired data; Thus, it becomes a data structure in which insertion and search operations are very fast irrespective of size of data. Hash Table uses array as a storage medium and uses hash technique to generate index where an element is to be inserted or to be located from.

- It may happen that the hashing technique used create already used index of the array. In such case, we can search the next empty location in the array by looking into the next cell until we found an empty cell. This technique is called linear probing.

## Sorting

- Sorting is important as it may lead to better search time; sorting is also helpful to arrange data in a more readable format

- Sorting algorithms may require some extra space for comparison and temporary storage of few data elements. These algorithms do not require any extra space and sorting is said to be happened in-place, or for example, within the array itself. This is called **in-place sorting**. **Bubble sort** is an example of in-place sorting.

- But in some sorting algorithms, the program requires space which more than or equal to the elements being sorted. Sorting which uses equal or more space are called **not-in-place sorting**. **Merge-sort** is an example of not-in-place sorting.

- If a sorting algorithm, after sorting the contents, does not change the sequence of similar content in which they appear, it is called **stable sorting**; If a sorting algorithm, after sorting the contents, changes the sequence of similar content in which they appear, it is called **unstable sorting**; Stability of an algorithm matters when we wish to maintain the sequence of original elements, like in a tuple for example.

- A sorting algorithm is said to be **adaptive**, if it takes advantage of already 'sorted' elements in the list that is to be sorted. That is, while sorting if the source list has some element already sorted, adaptive algorithms will take this in to account and will try not to re-order them; **A non-adaptive** algorithm is one which does not take into account the elements which are already sorted. They try to force every single element to be re-order to confirm their sortedness.

- **Increasing Order**: A sequence of values is said to be in increasing order, if the successive element is greater than the previous one. For example, 1, 3, 4, 6, 8, 9 are in increasing order, as every next element is greater than the previous.

- **Decreasing Order**: A sequence of values is said to be in decreasing order, if the successive element is less than the current one. For example, 9, 8, 6, 4, 3, 1 are in decreasing order, as every next element is less than the previous.

- **Non-Increasing Order**: A sequence of values is said to be in non-increasing order, if the successive element is less than or equal to its previous element in the sequence. This order occurs when the sequence contains duplicate values. For example, 9, 8, 6, 3, 3, 1 are in non-increasing order, as every next element is less than or equal to (in case of 3) but not greater than the any previous element.

- **Non-Decreasing Order**: A sequence of values is said to be in non-decreasing order, if the successive element is greater than or equal to its previous element in the sequence. This order occurs when the sequence contains duplicate values. For example, 1, 3, 3, 6, 8, 9 are in non-decreasing order, as every next element is greater than or equal to (in case of 3) but not less than the previous one.

- **Bubble sort** is a simple sorting algorithm (in-places sorting algorithm). This sorting algorithm is comparison based algorithm in which each pair of adjacent elements is compared and elements are swapped if they are not in order. This algorithm is not suitable for large data sets as its average and worst case complexity are of **O(n2)** where n are no. of items; a **swapped** value is used to indicate that a swap happened - this way it the algorithm knows that the array is already in order and no iteration is further required; also, items that are larger are settled into the end of the array, so they don't require to be checked in next iteration.

- **Insertion sort** is an in-place comparison based sorting algorithm. Here, a sub-list is maintained which is always sorted. For example, the lower part of an array is maintained to be sorted. A element which is to be 'insert'ed in this sorted sub-list, has to find its appropriate place and insert it there. Hence the name insertion sort; The array is searched sequentially and unsorted items are moved and inserted into sorted sub-list (in the same array). This algorithm is not suitable for large data sets as its average and worst case complexity are of **Ο(n2)** where n are no. of items; Observation: Very similar to bubble sort but instead it keeps a sublist which is also iterated and sorted.

- **Selection sort** is a simple sorting algorithm. This sorting algorithm is a in-place comparison based algorithm in which the list is divided into two parts, sorted part at left end and unsorted part at right end. Initially sorted part is empty and unsorted part is entire list; Smallest element is selected from the unsorted array and swapped with the leftmost element and that element becomes part of sorted array. This process continues moving unsorted array boundary by one element to the right; This algorithm is not suitable for large data sets as its average and worst case complexity are of O(n2) where n are no. of items.

- **Merge sort** is a (not in place) sorting technique based on divide and conquer technique. With worst-case time complexity being **Ο(n log n)**, it is one of the most respected algorithms; Merge sort first divides the array into equal halves and then combines them in a sorted manner.

- **Shell sort** is a highly efficient (not in place) sorting algorithm and is based on insertion sort algorithm. This algorithm avoids large shifts as in case of insertion sort if smaller value is very far right and have to move to far left; This algorithm uses insertion sort on widely spread elements first to sort them and then sorts the less widely spaced elements; This algorithm is quite efficient for medium sized data sets as its average and worst case complexity are of O(n) where n are no. of items; This spacing is termed as interval. This interval is calculated based on Knuth's formula as −
```C
h = h * 3 + 1

where −
   h is interval with initial value 1
```

- **Quick sort** is a highly efficient sorting algorithm and is based on partitioning of array of data into smaller arrays. A large array is partitioned into two arrays one of which holds values smaller than specified value say pivot based on which the partition is made and another array holds values greater than pivot value; The quick sort partitions an array and then calls itself recursively twice to sort the resulting two subarray. This algorithm is quite efficient for large sized data sets as its average and worst case complexity are of O(nlogn) where n are no. of items.

## Graph Data Structure

- A graph is a pictorial representation of a set of objects where some pairs of objects are connected by links. The interconnected objects are represented by points termed as **vertices**, and the links that connect the vertices are called **edges**; Formally, a graph is a pair of sets (V, E), where V is the set of vertices and E is the set of edges, connecting the pairs of vertices.

- Graphs can be represented with array of vertices and a two dimensional array of edges.

- **Vertex** − Each node of the graph is represented as a vertex. In example given below, labeled circle represents vertices. So A to G are vertices. We can represent them using an array as shown in image below. Here A can be identified by index 0. B can be identified using index 1 and so on.

- **Edge** − Edge represents a path between two vertices or a line between two vertices. In example given below, lines from A to B, B to C and so on represents edges. We can use a two dimensional array to represent array as shown in image below. Here AB can be represented as 1 at row 0, column 1, BC as 1 at row 1, column 2 and so on, keeping other combinations as 0.

- **Adjacency** − Two node or vertices are adjacent if they are connected to each other through an edge. In example given below, B is adjacent to A, C is adjacent to B and so on.

- **Path** − Path represents a sequence of edges between two vertices. In example given below, ABCD represents a path from A to D.

- **Depth First Search algorithm(DFS)** traverses a graph in a depthward motion and uses a stack to remember to get the next vertex to start a search when a dead end occurs in any iteration.

- **Breadth First Search algorithm(BFS)** traverses a graph in a breadthwards motion and uses a queue to remember to get the next vertex to start a search when a dead end occurs in any iteration.

## Tree

- Tree represents nodes connected by edges. We'll going to discuss binary tree or binary search tree specifically;

- Binary Tree is a special datastructure used for data storage purposes. A binary tree has a special condition that each node can have two children at maximum. A binary tree have benefits of both an ordered array and a linked list as search is as quick as in sorted array and insertion or deletion operation are as fast as in linked list.

- Binary Search tree exhibits a special behaviour. A node's left child must have value less than its parent's value and node's right child must have value greater than it's parent value.

- The basic operations that can be performed on binary search tree data structure, are following −
    + Insert − insert an element in a tree / create a tree.
    + Search − search an element in a tree.
    + Preorder Traversal − traverse a tree in a preorder manner.
    + Inorder Traversal − traverse a tree in an inorder manner.
    + Postorder Traversal − traverse a tree in a postorder manner.


- **Inorder Traversal** - In this traversal method, the left left-subtree is visited first, then root and then the right sub-tree. We should always remember that every node may represent a subtree itself; If a binary tree is traversed inorder, the output will produce sorted key values in ascending order.

- **Preorder Traversal** - In this traversal method, the root node is visited first, then left subtree and finally right sub-tree.

- **Postorder Traversal**In this traversal method, the root node is visited last, hence the name. First we traverse left subtree, then right subtree and finally root.

- A **binary search tree (BST)** is a tree in which all nodes follows the below mentioned properties −
    + The left sub-tree of a node has key less than or equal to its parent node's key.
    + The right sub-tree of a node has key greater than or equal to its parent node's key.
    + Thus, a binary search tree (BST) divides all its sub-trees into two segments; left sub-tree and right sub-tree and can be defined as −

`left_subtree (keys)  ≤  node (key)  ≤  right_subtree (keys)`

- What if the input to binary search tree comes in sorted (ascending (non-decreasing) or descending (non-increasing)) manner? Trees will disproportionate, meaning one side of the tree hold all the nodes; It is observed that BST's worst-case performance closes to linear search algorithms, that is Ο(n). In real time data we cannot predict data pattern and their frequencies. So a need arises to balance out existing BST.

- Named after their inventor Adelson, Velski & Landis, **AVL trees** are **height** balancing binary search tree. AVL tree checks the height of left and right sub-trees and assures that the difference is not more than 1. This difference is called **Balance Factor**; AVL tree permits difference (balance factor) to be only 1.
`BalanceFactor = height(left-sutree) − height(right-sutree)`

- To make itself balanced, an AVL tree may perform four kinds of rotations −
    + Left rotation
    + Right rotation
    + Left-Right rotation
    + Right-Left rotation

- First two rotations are single rotations and next two rotations are double rotations. Two have an unbalanced tree we at least need a tree of height 2. With this simple tree, let's understand them one by one.

- A **spanning tree** is a subset of Graph G, which has all the vertices covered with minimum possible number of edges. Hence, a spanning tree does not have cycles and it can not be disconnected; By this definition we can draw a conclusion that every connected & undirected Graph G has at least one spanning tree. A disconnected graph do not have any spanning tree, as it can not spanned to all its vertices.

- We found three spanning trees off one complete graph. A complete undirected graph can have maximum nn-2 number of spanning trees, where n is number of nodes. In addressed example, n is 3, hence 33−2 = 3 spanning trees are possible.

- We now understand that one graph can have more than one spanning trees. Below are few properties is spanning tree of given connected graph G −
    + A connected graph G can have more than one spanning tree.
    + All possible spanning trees of graph G, have same number of edges and vertices.
    + Spanning tree does not have any cycle (loops)
    + Removing one edge from spanning tree will make the graph disconnected i.e. spanning tree is minimally connected.
    + Adding one edge to a spanning tree will create a circuit or loop i.e. spanning tree is maximally acyclic.
    + Spanning tree has n-1 edges, where n is number of nodes (vertices)
    + From a complete graph, by removing maximum e-n+1 edges, we can construct a spanning tree.
    + A complete graph can have maximum nn-2 number of spanning trees.

- So we can conclude here that spanning trees are subset of a connected Graph G and disconnected Graphs do not have spanning tree.


- In a weighted graph, a **minimum spanning tree (MST)** is a spanning tree that has minimum weight that all other spanning trees of the same graph. In real world situations, this weight can be measured as distance, congestion, traffic load or any arbitrary value denoted to the edges.

## Heap

- Heap is a special case of balanced binary tree data structure where root-node key is compared with its children and arranged accordingly. If α has child node β then − `key(α) ≥ key(β)`

- As the value of parent is greater than that of child, this property generates **Max Heap**. Based on this criteria a heap can be of two types −
    + Min-Heap − where the value of root node is less than or equal to either of its children.
    + Max-Heap − where the value of root node is greater than or equal to either of its children.

## Recursion

- Some computer programming languages allows a module or function to call itself. This technique is known as **recursion**. In recursion, a function α either calls itself directly or calls a function β that in turn calls the original function α. The function α is called recursive function ; differs from the iteration functions (e.g., while and for);

- A recursive function can go infinite like a loop. To avoid infinite running of recursive function, there are two properties that a recursive function must have −
    + **Base criteria** − There must be at least one base criteria or condition, such that, when this condition is met the function stops calling itself recursively.
    + **Progressive approach** − The recursive calls should progress in such a way that each time a recursive call is made it comes closer to the base criteria.

- One may argue that why to use recursion as the same task can be done with iteration. The first reason is recursion makes a program more readable and because of today's enhance CPU systems, recursion is more efficient than iterations.

- **Time complexity**: In case of iterations, we take number of iterations to count the time complexity. Likewise, in case of recursion, assuming everything is constant, we try to figure out the number of time recursive call is being made. A call made to a function is Ο(1), hence the (n) number of time a recursive call is made makes the recursive function Ο(n).

- **Space complexity**: Space complexity is counted as what amount of extra space is required for a module to execute. In case of iterations, the compiler hardly requires any extra space. Compiler keeps updating the values of variables used in the iterations. But in case of recursion, the system needs to store activation record each time a recursive call is made. So it is considered that space complexity of recursive function may go higher than that of a function with iteration.
