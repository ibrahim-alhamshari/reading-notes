### What is a Stack
**A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.**
- Push - Nodes or items that are put into the stack are pushed. And pushing a Node onto a stack will always be an O(1) operation.

- Peek - When you peek you will view the value of the top Node in the stack. When you attempt to peek an empty stack an exception will be raised. When conducting a peek, you will only be inspecting the top Node of the stack.

- Pop - Nodes or items that are removed from the stack are popped. When you attempt to pop an empty stack an exception will be raised. Popping a Node off a stack is the action of removing a Node from the top.


### What is a Queue
- Enqueue - Nodes or items that are `added` to the queue.
- Dequeue - Nodes or items that are `removed` from the queue. If called when the queue is empty an exception will be raised.
- Front - `first` Node of the queue.
- Rear - `last` Node of the queue.
- Peek - When you `peek` you will view the value of the `front` Node in the queue.

- First In First Out(FIFO): This means that the first item in the queue will be the first item out of the queue.

- Last In Last Out(LILO): This means that the last item in the queue will be the last item out of the queue.

![Queue_Visualization](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/images/Queue.PNG)

### Resources
- https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-10/resources/stacks_and_queues.html