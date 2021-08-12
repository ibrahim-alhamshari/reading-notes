## Trees

- Node - A Tree node is a component which may contain it’s own values, and references to other nodes
- Root - The root is the node at the beginning of the tree
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf

![Sample Tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG)

-  Traversing a tree allows us to search for a node, print out the contents of a tree. We have two categories of traversals trees:
1. `Depth First`: is where we prioritize going through the depth (height) of the tree first.We have three methods for depth first traversal:
- Pre-order: root >> left >> right
- In-order: left >> root >> right
- Post-order: left >> right >> root

2. `Breadth First`: iterates through the tree by going through each level of the tree node-by-node. And it uses a queue (instead of the call stack via recursion) to traverse the width/breadth of the tree.

- **Binary Tree**
- Trees can have any number of children per node, but `Binary Trees` restrict the number of children to two (hence our left and right children).
![Binary Tree](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree2.PNG)

- **K-ary Trees**
- If Nodes are able have more than 2 child nodes, we call the tree that contains them a `K-ary Tree`. In this type of tree we use K to refer to the maximum number of children that each Node is able to have.

![K-ary Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/KaryTree1.png)

## What is Recursion? 
The process in which a function calls itself directly or indirectly is called `recursion` and the corresponding function is called as `recursive function`.

#### Why Stack Overflow error occurs in recursion? 
- If the base case is not reached or not defined, then it will arise the stack overflow problem.

**Here is a `recursive tree` for input 5 which shows a picture of how a big problem can be solved into smaller ones.**

![recursive tree](https://media.geeksforgeeks.org/wp-content/uploads/20191107235734/fib1.jpg)

## Resources
- https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html
- https://www.geeksforgeeks.org/recursion/