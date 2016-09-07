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

- Linked List is a sequence of links which contains items. Each link contains a connection to another link. Linked list the second most used data structure after array. Following are important terms to understand the concepts of Linked List.
    + Link − Each Link of a linked list can store a data called an element.
    + Next − Each Link of a linked list contain a link to next link called Next.
    + LinkedList − A LinkedList contains the connection link to the first Link called First.

- Following are the various flavours of linked list.
    + Simple Linked List − Item Navigation is forward only.
    + Doubly Linked List − Items can be navigated forward and backward way.
    + Circular Linked List − Last item contains link of the first element as next and and first element has link to last element as prev.

- 
