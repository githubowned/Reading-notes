# Stacks and Queues:

## What is a Stack:
- A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.
A stack is a linear data structure in which elements can be inserted and deleted only from one side of the list, called the top.
<br/>

 ## Common terminology for a stack :
- Push : Nodes or items that are put into the stack are pushed. Push O(1)
- Pop : Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised. Pop O(1)
- Top: This is the top of the stack.
- Peek: When you peek you will view the value of the top Node in the stack. When you attempt to peek an - empty stack an exception will be raised. Peek O(1)
- IsEmpty: returns true when stack is empty otherwise returns false. IsEmpty O(1)
<br/>

## Stacks follow these concepts:
- FILO(First In Last Out) : This means that the first item added in the stack will be the last item popped out of the stack.
- LIFO(Last In First Out) : This means that the last item added to the stack will be the first item popped out of the stack.
 <br/>

 ## What is a Queue?
- A queue is a linear data structure in which elements can be inserted only from one side of the list called rear, and the elements can be deleted only from the other side called the front.
<br/>

 ## Common terminology for a queue :
- Enqueue: Nodes or items that are added to the queue. Enqueue O(1)

- Dequeue :Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised. Dequeue O(1)

- Front : This is the front/first Node of the queue.

- Rear : This is the rear/last Node of the queue.

- Peek : When you peek you will view the value of the front Node in the queue. If called when the queue is empty an exception will be raised. Peek O(1)

- IsEmpty : returns true when queue is empty otherwise returns false. IsEmpty O(1)
<br/>


## Queues follow these concepts:

- FIFO (First In First Out) : This means that the first item in the queue will be the first item out of the queue.

- LILO (Last In Last Out) : This means that the last item in the queue will be the last item out of the queue.

<br/>

#References:
[Stacks and Queues](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html)
