## Linked List

- Linked List - A data structure that contains nodes that links/points to the next node in the list.
- Node - Nodes are the individual items/links that live in a linked list. Each node contains the data for each link.

![Linked list](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/images/LinkedList1.PNG)

- There are two types of Linked List - Singly and Doubly. 
- Each node contains a property called `Next`. This property contains the reference to the next node.

- Here is the Pseudo code for an *`Add`* method on a Linked list with an O(1):
  - `ALGORITHM Add(newValue)`
  - `// INPUT <-- Value to add`
  - `// OUTPUT <-- No output`

  - `newNode <-- NEW Node`
  - `newNode.Value <-- newValue`
  - `newNode.Next <-- Head`
  - `Head <-- newNode`

> Printing out all of the nodes in a Linked List:
> we are creating a while loop to check and make sure we are not at the end of a linked list.
- ALGORITHM Print()
- // INPUT <-- None
- // OUTPUT <-- string to console

  - Current <-- Head

  - WHILE Current is not equal to NULL
  -  OUTPUT <-- "{Current.Value} --> "
   - Current <-- Current.Next

  - OUTPUT <-- "NULL"

### Resources
- https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html
- https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d
- https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996