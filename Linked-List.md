# Linked List # 

## Linear Data Structures ## 

One of the characteristics of a *linked list* is that it is a *linear data structure*. This means "that there is a sequence and an order to how they are constructed and traversed." - [Linked List pt. 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d). On the flip-side, with *non-linear data structures* 
you do not traverse through the data sequentially. 

      Linear Structure                    Non-Linear Structure
      
      [] -> [] -> [] -> [] ...                   [ ]
                                                |   |
                                               []   []
                                              |       |
                                             []   ->  []
                                             
## Memory Management ## 

Arrays are an example of a linear data structure but it is different than a Linked List which also is a linear structure. The difference is the memory use within our machines. An array that might have 7 values need 7 bytes, and our machines would need to find 7 bytes of memory that was free to use in one place. With a linked list, you do not need 7 bytes all in one place. Unlike an array where the memory needs to be allocated in one location, a *linked list* can have memory scattered throughout. "The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures." - [Linked List pt. 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d). 

## Parts Of a Linked List ## 

*Linked Lists* "is made up of a series of nodes, which are the elements of the list." - [Linked List pt. 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d). 

The starting point of a *linked list* is the first node and is referred to as the head. At the end of a *link list* is not a node, but rather a node that will point to null or empty. All *linked lists* start with a head because that is the starting point, and without it, there would be no entry starting point. Another point worth mentioning is "A node only knows about what data it contains, and who its neighbor is." - [Linked List pt. 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d). Furthermore, nodes do not know where the starting point is nor the end - and only knows its neighbor or the next node. This is what enables a *linked list* to have memory scattered throughout instead of in a single location like an array; because eah node in a *linked list* has the reference or address to the next node. 

## Lists For All Shapes And Sizes ## 

* _singly linked lists_ - The simplest type of *linked list* can only go in one direction - from the *Head* to null. 
* _doubly linked lists_ - This type of *linked list* - nodes can reference to the previous node rather than just the next node. You would use this so when you do not want to start from the *head* every single time. 
* _circular linked list_ - This type of *linked list* does not have the ending node point to null, and rather has another node that will point to the beginning of the *linked list* after the last node. 

## Big O notation ## 

"Big O Notation is a way of evaluating the performance of an algorithm." - [Linked List pt. 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996). 
A way to think about Big O is the amount of time that a function takes to run based on the amount of elements that is passed into that function or N. Big O, might not be very important when your dealing with maybe 10 values in an array - but it starts getting more important when your dealing with "ten thousand? Or a million? Or tens of millions?" - [Linked List pt. 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996). To break down what "O" even is "O" can be referred to as just "O" or *order*. Then there is "N" which is the size of the input. However, when dealing with *Linked Lists* two BigO equations that need to be remembered is `O(1)` and `O(n)`. If you think about a graph, imagine a straight horizontal line - that is O(1) which is constant or constant time. 
If you think about the same graph but a line that has a constant rise and run - or linear meaning, that it will have a constant growth of n - that is O(n) or linear. 
Another BigO equation is O(n^2). This is an exponential growth in terms of within a graph (so as time continues run, the n or the rise will curve upwards exponentially. 

## Growing A Linked List ## 

All you really need to do to grow your *linked list* is change the pointers for the nodes. Some example steps you might take for a *singly linked list* to grow might be to: 

1. First, we find the head node of the linked list.
2. Next, we’ll make our new node, and set its pointer to the current first node of the list.
3. Lastly, we rearrange our head node’s pointer to point at our new node.

[Linked List pt.2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996). 

"Inserting an element at the beginning of a linked list is particularly nice and efficient because it takes the same amount of time, no matter how long our list is, which is to say it has a space time complexity that is constant, or O(1)." - [Linked List pt. 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996). 

Inserting an element at the end of a *linked list* follows, practically the same steps. 

1. Find the node we want to change the pointer of (in this case, the last node)
2. Create the new node we want to insert and set its pointer (in this case, to null)
3. Direct the preceding node’s pointer to our new node

[Linked Lists pt. 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996). 

But beware, before you can insert an element after the end of the *linked list* you will have to find it which means you will have to traverse through the *linked list*. 

## To List Or Not To List ## 

A good thing to note when considering if you want to use a *linked list* is: 
"a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element." - [Linked List pt. 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996).
Thus, keep in mind that an array might be the better option if you find yourself needing to constantly traverse, iterate, or need quick index-level access.

![Array Vs. Linked List](https://miro.medium.com/max/700/1*cUehR5S18XSoVLaPNfNzlA.jpeg)

