# Read: Stacks & Queues Summary :
### What is a Stack ?
* Stack is a linear data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous. It follows a particular order in which the operations are performed.The order may be **LIFO(Last In First Out)** or **FILO(First In Last Out)**.
### Common terminology for a stack is
1. **Push**: Nodes or items that are put into the stack are pushed
2. **Pop** : Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised.
3. **Top** : This is the top of the stack.
4. **Peek**: When you peek you will view the value of the **top Node** in the stack. When you attempt to peek an empty stack an exception will be raised.
5. **IsEmpty** : returns true when stack is empty otherwise returns false.

### Stack Visualization :
* The topmost item is denoted as the **top**. When you push something to the stack, it becomes the new top. When you pop something from the stack, you pop the current top and set the next top as **top.next**.
* When adding a Node, you **push** it into the stack by assigning it as the new top, with its next property equal to the original top.
  - **Note**:Pushing a Node onto a stack will always be an O(1) operation. This is because it takes the same amount of time no matter how many Nodes (n) you have in the stack.
*  Popping a Node off a stack is the action of removing a Node from the top. When conducting a pop, the top Node will be re-assigned to the Node that lives below and the top Node is returned to the user.
* When conducting a peek, you will only be inspecting the top Node of the stack.

### What is a Queue ?
* A Queue is a linear structure which follows a particular order in which the operations are performed. The order is First In First Out (FIFO). 
* The difference between stacks and queues is in removing. In a stack we remove the item the most recently added; in a queue, we remove the item the least recently added.
### Common terminology for a queue is
1. **Enqueue** : Nodes or items that are **added** to the queue.
2. **Dequeue** :  Nodes or items that are **removed** from the queue. If called when the queue is empty an exception will be raised.
3. **Front** : This is the front/first Node of the queue.
4. **Rear** : This is the rear/last Node of the queue.
5. **Peek** : When you peek you will view the value of the **front Node** in the queue. If called when the queue is empty an exception will be raised.
6. **IsEmpty** : returns true when queue is empty otherwise returns false.

### Queue Visualization
* When you add an item to a queue, you use the **enqueue** action. This is done with an O(1) operation in time because it does not matter how many other items live in the queue (n).
* When you remove an item from a queue, you use the **dequeue** action. This is done with an O(1) operation in time because it doesn’t matter how many other items are in the queue, you are always just removing the **front Node** of the queue.
* When conducting a **peek**, you will only be inspecting the front Node of the queue.




