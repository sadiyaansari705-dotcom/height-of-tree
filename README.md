Find Height of a Binary Tree in C

This project demonstrates how to calculate the height of a Binary Tree using recursion in C.

🧾 Program Description

The program:

Defines a Node structure containing:

data

left pointer

right pointer

Dynamically creates a binary tree using malloc().

Uses a recursive function height() to compute the height of the tree.

Prints the height of the tree.

🌳 Example Tree Used
        1
       / \
      2   3
     / \
    4   5
📏 What is Height of a Binary Tree?

The height of a binary tree is the number of edges on the longest path from the root node to a leaf node.

In this program:

If root == NULL, the function returns -1

Height is calculated in terms of edges

For the above tree:

Height of Tree = 2
🧠 How the Height Function Works
int height(struct Node* root)

If the node is NULL, return -1.

Recursively find height of left subtree.

Recursively find height of right subtree.

Return:

1 + max(leftHeight, rightHeight)
🧠 Concepts Used

Binary Tree

Recursion

Divide and Conquer Approach

Dynamic Memory Allocation (malloc)

Pointers and Structures in C

⏱ Time and Space Complexity

Time Complexity: O(n)

Space Complexity: O(h) (recursive stack height)

Where:

n = number of nodes

h = height of tree

🚀 How to Run
🔹 Compile the Program
gcc main.c -o output
🔹 Run the Program
./output

(For Windows)

output.exe
📂 Project Structure
📁 binary-tree-height
 ├── main.c
 └── README.md
⚠️ Notes

Height is calculated in terms of edges.

If you want height in terms of number of nodes, change:

return -1;

to:

return 0;
🔧 Possible Improvements

Take user input to create tree dynamically.

Add level-order traversal display.

Free allocated memory.

Add functions for diameter and depth calculation.

👨‍💻 Author


B.Tech Student

If you want, I can also provide:

⭐ Version calculating height in terms of nodes

⭐ Complete binary tree operations program

⭐ Comparison between height and depth

⭐ Short lab submission version
