binary_trees
This is a partner project in which we are implimenting Binary trees,Data Structure and Algorithms,Tree Traversal,Binary Search Tree and Data structures. In this project, we learnt what is a binary tree, the diff between a binary tree and a binhary search tree,possibl gains in terms of time complexity compared to linked lists,the depth,the height and the size of a binary tree.the different traversal methods to go through a binary tree, a complete, a full, a perfect, and a balanced binary tree.

Header file Contains all the prototypes of the projects functions. Must push your header file All your header files should be include guarded.

Test files Has all the test files to test the projects functions. We did not push them to our repo.

Data structures Must include them in the header file.

Basic Binary Tree /**

struct binary_tree_s - Binary tree node
@n: Integer stored in the node
@parent: Pointer to the parent node
@left: Pointer to the left child node
@right: Pointer to the right child node */ struct binary_tree_s { int n; struct binary_tree_s *parent; struct binary_tree_s *left; struct binary_tree_s *right; };
typedef struct binary_tree_s binary_tree_t; Binary Search Tree typedef struct binary_tree_s bst_t; AVL Tree typedef struct binary_tree_s avl_t; Max Binary Heap typedef struct binary_tree_s heap_t;

Print function Functions to print binary trees in a pretty way

                       .----------------------(006)-------.
                  .--(001)-------.                   .--(008)--.
             .--(-02)       .--(003)-------.       (007)     (009)
   .-------(-06)          (002)       .--(005)
.--(-08)--. (004) (-09) (-07)

Tasks

New node
0-binary_tree_node.c: C function that creates a binary tree node with a given parent and value. Returns a pointer to the new node, or NULL on failure.

Insert left
1-binary_tree_insert: C function that inserts a node as the left-child of another. Returns a pointer to the new node, or NULL on failure. If the given parent already contains a left node, the new node takes its place and the old left-child becomes the left-child of the new node. 2. Insert right

2-binary_tree_insert_right.c: C function that inserts a node as the right-child of another. Returns a pointer to the new node, or NULL on failure. If the given parent already contains a right node, the new node takes its place and the old right-child becomes the right-child of the new node. 3. Delete

3-binary_tree_delete.c: C function that deletes an entire binary tree. 4. Is leaf

4-binary_tree_is_leaf.c: C function that checks if a given node is a leaf. Returns 1 if the node is a leaf, 0 otherwise. 5. Is root

5-binary_tree_is_root.c: C function that checks if a given node is a root. Returns 1 if the node is a root, 0 otherwise. 6. Pre-order traversal

6-binary_tree_preorder.c: C function that traverses a tree using pre-order traversal. 7. In-order traversal

7-binary_tree_inorder.c: C function that traverses a tree using in-order traversal. 8. Post-order traversal

8-binary_tree_postorder.c: C function that traverses a tree using post-order traversal. 9. Height

9-binary_tree_height.c: C function that returns the height of a binary tree. 10. Depth

10-binary_tree_depth.c: C function that returns the depth of a given node in a binary tree. 11. Size

11-binary_tree_size.c: C function that returns the size of a binary tree. 12. Leaves

12-binary_tree_leaves.c: C function that returns the number of leaves in a binary tree. 13. Nodes

13-binary_tree_nodes.c: C function that returns the number of nodes in a binary tree with at least one child. 14. Balance factor

14-binary_tree_balance.c: C function that returns the balance factor of a binary tree. 15. Is full

15-binary_tree_is_full.c: C function that checks if a binary tree is full. Returns 1 if a tree is full, 0 otherwise. 16. Is perfect

16-binary_tree_is_perfect.c: C function that checks if a binary tree is perfect. Returns 1 if a tree is perfect, 0 otherwise. 17. Sibling

17-binary_tree_sibling.c: C function that returns a pointer to the sibling of a given node in a binary tree. Returns NULL if no sibling is found. 18. Uncle

18-binary_tree_uncle.c: C function that returns a pointer to the uncle of a given node in a binary tree. Returns NULL if no uncle is found. 19. Lowest common ancestor

100-binary_trees_ancestor.c: C function that returns a pointer to the lowest common ancestor node of two given nodes in a binary tree. Returns NULL if no common ancestor is found. 20. Level-order traversal

101-binary_tree_levelorder.c: C function that traverses a binary tree using level-order traversal. 21. Is complete

102-binary_tree_is_complete.c: C function that checks if a binary tree is complete. Returns 1 if the tree is complete, 0 otherwise. 22. Rotate left

103-binary_tree_rotate_left.c: C function that performs a left-rotation on a binary tree. Returns a pointer to the new root node of the tree after rotation. 23. Rotate right

104-binary_tree_rotate_right.c: C function that performs a right-rotation on a binary tree. Returns a pointer to the new root node of the tree after rotation. 24. Is BST

110-binary_tree_is_bst.c: C function that checks if a binary tree is a valid binary search tree. Returns 1 if the tree is a valid BST, 0 otherwise. 25. BST - Insert

111-bst_insert.c: C function that inserts a value into a binary search tree. Returns a pointer to the new node, or NULL on failure. If the tree is NULL, the value becomes the root node. The value is ignored if it is already present in the tree. 26. BST - Array to BST

112-array_to_bst.c: C function that builds a binary search tree from an array. Returns a pointer to the root node of the created tree, or NULL on failure. 27. BST - Search

113-bst_search.c: C function that searches for a value in a binary search tree. If the value is matched in the BST, returns a pointer to the matched node. Otherwise, returns NULL. 28. BST - Remove

114-bst_remove.c: C function that removes a node from a binary search tree. Returns a pointer to the new root node of the tree after deletion. If the node to be deleted has two children, it is replaced with its first in-order successor. 29. Big O #BST

115-O: Text file containing the average time complexities of binary search tree operations (one answer per line): Inserting the value n. Removing the node with the value n. Searching for a node in a BST of size n. 30. Is AVL

120-binary_tree_is_avl.c: C function that checks if a binary tree is a valid AVL tree. If the tree is a valid AVL tree, returns 1. Otherwise, returns 0. 31. AVL - Insert

121-avl_insert.c: C function that inserts a value in an AVL tree. Returns a value to the inserted node, or NULL on failure. 32. AVL - Array to AVL

122-array_to_avl.c: C function that builds an AVL tree from an array. Returns a pointer to the root node of the created AVL tree, or NULL on failure. Ignores duplicate values. 35. Big O #AVL Tree

125-O: Text file containing the average time complexities of AVL tree opeartions (one answer per line): Inserting the value n. Removing the node with the value n. Searching for a node in an AVL tree of size n. 41. Big O #Binary Heap

135-O: Text file containing the average time complexities of binary heap opeartions (one answer per line): Inserting the value n. Extracting the root node. Searching for a node in a binary heap of size n.
