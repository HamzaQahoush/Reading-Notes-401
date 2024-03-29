
## What is a Linked List? 
* **A Linked List** is a sequence of **Nodes** that are connected/linked to each other. The most defining feature of a Linked List is that *each Node references the next Node in the link*.
* There are two types of Linked List - **Singly** and **Doubly**.
  -  **Singly** :  Singly refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the Next node in a linked list.
  - **Doubly** - Doubly refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous node.
  ![image](https://miro.medium.com/max/875/1*AeMDLFUjR0w0J4n8CP4H6g.jpeg)
* **Node** - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.
* **Next** - Each node contains a property called Next. This property contains the reference to the next node.
* **Head** - The Head is a reference of type Node to ***the first node in a linked list***.
* **Current**- The Current is a reference of type Node to the node that is currently being looked at. When traversing, you create a new Current variable at the Head to guarantee you are starting from the beginning of the linked list.
* * ![image](https://miro.medium.com/max/875/1*K0_eV07tJtKQSVGKfP18bw.jpeg)
* The **Next** property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.  The best way to approach a traversal is through the use of **a while() loop**. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash.
* ***Traversal Example***:
* Let’s put a use case on our traversal. We want to check whether or not our LinkedList Includes a specific value.
```
The pseudo-code for an Includes is as so:

ALGORITHM Includes (value)
// INPUT <-- integer value
// OUTPUT <-- boolean

  Current <-- Head

  WHILE Current is not NULL
    IF Current.Value is equal to value
      return TRUE

    Current <-- Current.Next

  return FALSE
```
- **The Big O** of time for Includes would be O(n). This is because, at its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

- **The Big O** of space for Includes would be O(1). This is because there is no additional space being used than what is already given to us with the linked list input.
![image](https://miro.medium.com/max/875/1*Jy5tjwrMdtpGl2ceq4f94A.jpeg)
* When constructing your code, a few things to keep in mind>> When making your Node class, consider requiring a value to be passed in to require that each node has a value.
# array vs .linked list 
![image](https://miro.medium.com/max/875/1*cUehR5S18XSoVLaPNfNzlA.jpeg)
