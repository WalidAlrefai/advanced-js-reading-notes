# Stacks and Queues 

Stack A stack is a linear data structure in which elements can be inserted and deleted only from one side of
the list, called the top. A stack follows the LIFO (Last In First Out) principle, i.e., the element inserted
at the last is the first element to come out. The insertion of an element into stack is called push 
operation, and deletion of an element from the stack is called pop operation. In stack we always keep track 
of the last element present in the list with a pointer called top.

The diagrammatic representation of stack is given below:

![](./geek-stack-1.png)


Queue: A queue is a linear data structure in which elements can be inserted only from one side of the list 
called rear, and the elements can be deleted only from the other side called the front. The queue data 
structure follows the FIFO (First In First Out) principle, i.e. the element inserted at first in the list, is
the first element to be removed from the list. The insertion of an element in a queue is called an enqueue 
operation and the deletion of an element is called a dequeue operation. In queue we always maintain two 
pointers, one pointing to the element which was inserted at the first and still present in the list with the 
front pointer and the second pointer pointing to the element inserted at the last with the rear pointer.

![](./geek-queue-1.png)

## Difference between Stack and Queue Data Structures

|Stacks|Queues|
|-------------------|----------------|
|Stacks are based on the LIFO principle, i.e., the element inserted at the last, is the first element to come out of the list|Queues are based on the FIFO principle, i.e., the element inserted at the first, is the first element to come out of the list|

|Insertion and deletion in stacks takes place only from one end of the list called the top. |Insertion and deletion in queues takes place from the opposite ends of the list. The insertion takes place at the rear of the list and the deletion takes place from the front of the list.|
|-------------------|----------------|
|Insert operation is called push operation.|Insert operation is called enqueue operation.|
|-------------------|----------------|
|Delete operation is called pop operation|Delete operation is called dequeue operation.|
|In stacks we maintain only one pointer to access the list, called the top, which always points to the last element present in the list.|n queues we maintain two pointers to access the list. The front pointer always points to the first element inserted in the list and is still present, and the rear pointer always points to the last inserted element.|
|-------------------|-------------------|
|Stack is used in solving problems works on recursion.|Queue is used in solving problems having sequential processing.|
