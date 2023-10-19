# Singly Linked List
>It is the most commonly used data structure used to store similar types of data. NO MIXING.

>The elements of a linked list are not stores in adjacent memory locations like arrays.

>A linked list is a linear collection of data elements called nodes, where the linear order is implemented by means of pointers.

>A linear structure where an array is a random access structure. 

>Each linked list containts a head and a tail. Tail is generally null.
# Nodes
>Contain a data partition and a next pointer.

# Properties of a linked list
>The nodes in a linked list are not stores contiguously in the memory.
>
>You don't have to shift any element in the list when inserting or deleting elements, unlike arrays. Inserting a new node is considered constant (O(n)) because we are just updating pointers.
>>>In arrays, we need to shift every element in order to add an element to the front or in the middle.
>
>Memory for each node can be allocated dynamically whenever the need arises.
>
>The size of a linked list can grow or shrink dynamically during run-time.

# Why use a Linked List over an Array




# Operations
## Creation
>This operation is used to create a linked list
## Insertion and Deletion
>At/From the beginning of a linked list
>At/From the end of the linked list
>At/From the specified position in a linked list
## Traversing
>Traversing may be either forward or backward
## Searching
>Finding an element in a linked list
## Concatenation
>the process of appending second list to the end of the first

# Dynamic Memory Allocation
Creating and maintining data structures requires dynamic memory allocation - the ability for a program to obtain more memory space at execution time to hold new nodes, and to release space no longer needed.

## Functions essential to memory allocation
Make sure to typecast the void pointer to the correct type.
The allocated memory is not initialized.
### malloc
>Takes an argument that is the number of bytes to be allocated and returns a void pointer to the allocated memory.

##### Example usage
>newPtr = (node*)malloc(sizeof(struct node));
### free
>Deallocates memory - i.e. the memory is returned to the system so that it can be reallocated.
##### Example usage
>free(newPtr);
### sizeof()

[[Linked List Example Code]]

