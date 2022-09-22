## 0x1D. C - Binary trees
# About 
- Binary Tree
- Binary Search 
- AVL Tree
- Max Binary Tree
- Tree Traversal 

# Requirements
- Compiled on Ubuntu 20.04 LTS using gcc
- Not allowed to use global variables
- Code should use the Betty style.

# File Descriptions
**Mandatory Tasks**
0. New node

Write a function that creates a binary tree node

-Prototype: binary_tree_t *binary_tree_node(binary_tree_t *parent, int value);
- Where parent is a pointer to the parent node of the node to create
- And value is the value to put in the new node
- When created, a node does not have any child
- Your function must return a pointer to the new node, or NULL on failure

1. Insert left mandatory
Write a function that inserts a node as the left-child of another node

- Prototype: binary_tree_t *binary_tree_insert_left(binary_tree_t *parent, int value);
- Where parent is a pointer to the node to insert the left-child in
- And value is the value to store in the new node
- Your function must return a pointer to the created node, or NULL on failure
- If parent already has a left-child, the new node must take its place, and the old left-child must be set as the left-child of the new node.
2. Insert right mandatory
Write a function that inserts a node as the right-child of another node

- Prototype: binary_tree_t *binary_tree_insert_right(binary_tree_t *parent, int value);
- Where parent is a pointer to the node to insert the right-child in
- And value is the value to store in the new node
- Your function must return a pointer to the created node, or NULL on failure
- If parent already has a right-child, the new node must take its place, and the old right-child must be set as the right-child of the new node.
3. Delete mandatory
Write a function that deletes an entire binary tree

- Prototype: void binary_tree_delete(binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to delete
4. Is leaf mandatory
Write a function that checks if a node is a leaf

- Prototype: int binary_tree_is_leaf(const binary_tree_t *node);
- Where node is a pointer to the node to check
- Your function must return 1 if node is a leaf, and 0 otherwise
- If node is NULL, return 0
5. Is root mandatory
Write a function that checks if a given node is a root

- Prototype: int binary_tree_is_root(const binary_tree_t *node);
- Where node is a pointer to the node to check
- Your function must return 1 if node is a root, and 0 otherwise
- If node is NULL, return 0
6. Pre-order traversal mandatory
Write a function that goes through a binary tree using pre-order traversal

- Prototype: void binary_tree_preorder(const binary_tree_t *tree, void (*func)(int));
- Where tree is a pointer to the root node of the tree to traverse
- And func is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
7. In-order traversal mandatory
Write a function that goes through a binary tree using in-order traversal

- Prototype: void binary_tree_inorder(const binary_tree_t *tree, void (*func)(int));
- Where tree is a pointer to the root node of the tree to traverse
- And func is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
8. Post-order traversal mandatory
Write a function that goes through a binary tree using post-order traversal

- Prototype: void binary_tree_postorder(const binary_tree_t *tree, void (*func)(int));
- Where tree is a pointer to the root node of the tree to traverse
- And func is a pointer to a function to call for each node. The value in the node must be passed as a parameter to this function.
9. Height mandatory
Write a function that measures the height of a binary tree

- Prototype: size_t binary_tree_height(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to measure the height of
- If tree is NULL, your function must return 0
10. Depth mandatory
Write a function that measures the depth of a node in a binary tree

- Prototype: size_t binary_tree_depth(const binary_tree_t *node);
- Where tree is a pointer to the node to measure the depth of
- If node is NULL, your function must return 0
11. Size mandatory
Write a function that measures the size of a binary tree

- Prototype: size_t binary_tree_size(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to measure the size of
12. Leaves mandatory
Write a function that counts the leaves in a binary tree

- Prototype: size_t binary_tree_leaves(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to count the leaves in
- A NULL pointer is not a leaf
13. Nodes mandatory
Write a function that counts the nodes with at least 1 child in a binary tree

- Prototype: size_t binary_tree_nodes(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to count the nodes in
- A NULL pointer is not a node
14. Balance factor mandatory
Write a function that measures the balance factor of a binary tree

- Prototype: int binary_tree_balance(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to measure the balance factor of
- If tree is NULL, return 0
15. Is full mandatory
Write a function that checks if a binary tree is full

- Prototype: int binary_tree_is_full(const binary_tree_t *tree);
- Where tree is a pointer to the root node of the tree to check
- If tree is NULL, your function must return 0
