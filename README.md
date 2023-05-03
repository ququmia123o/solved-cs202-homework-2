Download Link: https://assignmentchef.com/product/solved-cs202-homework-2
<br>
<h1>Question 1 –</h1>

You must draw the trees in this question by hand, and embed the scans or photographs of your drawings in your report. Make sure your drawings are clear, as ambiguities would make you lose points.

<ul>

 <li>[<em>5 points</em>] Insert 5, 12, 7, 1, 6, 3, 13, 2, 10, 11 into an empty binary search tree in the given order. Show the resulting BST after every insertion.</li>

 <li>[<em>5 points</em>] What are the preorder, inorder, and postorder traversals of the BST you have after (a)?</li>

 <li>[<em>5 points</em>] Delete 2, 7, 5, 6, 11 from the BST you have after (a) in the given order.</li>

</ul>

Show the resulting BST after every deletion.

<h1>Question 2</h1>

<ul>

 <li>[<em>21 points</em>] Implement a pointer-based Binary Search Tree whose keys are integers. Implement methods for insertion, deletion, retrieval, and inorder traversal. Traversal method must return an ordered array of keys and set the length parameter to the length of the array. (Note: The returned array must be dynamically allocated.) Put your code into the BSTNode.h, BSTNode.cpp, BST.h, BST.cpp files. Prototypes of the methods must be the following:

  <ul>

   <li>void BST::insertItem(int key); // 5 points</li>

   <li>void BST::deleteItem(int key); // 5 points</li>

   <li>BSTNode* BST::retrieveItem(int key); // 5 points</li>

   <li>int* BST::inorderTraversal(int&amp; length); // 6 points</li>

  </ul></li>

 <li>[<em>25 points</em>] Implement a method named containsSequence that takes a <em>sorted </em>array of integers as input, returns true if it is a sub-array of the inorder traversal of the BST, and false otherwise. Do not traverse all nodes, but only the nodes that are required to perform this check. Your method should print the key of the node when it enters to the node while traversing the tree, so that one can check which nodes are visited. Prototype of the method must be the following:

  <ul>

   <li>bool BST::containsSequence(int* seq, int length);</li>

  </ul></li>

</ul>

Figure 1: Example BST

For example, for the BST in Figure 1:

<ul>

 <li>containsSequence([1, 2, 3, 4, 5, 6], 6) must return true and must not traverse the subtree rooted at 13.</li>

 <li>containsSequence([10, 12, 13, 15], 4) must return false since the given sequence skips 14, and must not traverse the subtree rooted at 4.</li>

 <li>containsSequence([10, 11, 12], 3) must return false since 11 does not exists in the tree, and must not traverse the subtrees rooted at 4 and 15.</li>

</ul>

<ul>

 <li>[<em>12 points</em>] The level of a node is the number of nodes in the path from the node to the tree’s root node. The level of the root node is 1. Implement a method named countNodesDeeperThan that returns the number of nodes whose level is greater than or equal to a given number:

  <ul>

   <li>int BST::countNodesDeeperThan(int level);</li>

  </ul></li>

 <li>[<em>12 points</em>] Implement a method named maxBalancedHeight that returns what would be the height of the tree if we removed the minimum number of nodes required to make the tree height-balanced. For the BST in Figure 1, removing 2 would make the tree height-balanced, and the result of maxBalancedHeight would be 4. (Hint: Think recursively.) Prototype of the method must be the following:

  <ul>

   <li>int BST::maxBalancedHeight();</li>

  </ul></li>

 <li>[<em>0 points, mandatory</em>] Add a main function to the main.cpp file which calls the functions above with proper inputs (you will need to create some trees first), and displays their outputs. At the end, write a basic Makefile which compiles all your code and creates an executable file named hw2. <u>Please make sure that your </u>Makefile <u>works properly, otherwise you will not get any points from Question 2.</u></li>

</ul>

<h1>Question 3</h1>

In this question, you need to briefly explain your implementations in Question 2, analyze the asymptotic behavior of your implementations, and derive the resulting worst-case and average-case running time and space complexities. Your answer should be written in your report. You may, if you wish, write parts of your code or pseudo-code while explaining it.