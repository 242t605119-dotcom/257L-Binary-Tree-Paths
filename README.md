# Binary Tree Paths

**LeetCode Problem:** 257
**Language:** Python

## Problem

Given the root of a binary tree, return all root-to-leaf paths.

A leaf node is a node that does not have a left or right child.

Each path should be represented as a string using `->` between the node values.

For example:

```text
Input:
    1
   / \
  2   3
   \
    5

Output:
["1->2->5", "1->3"]
```

## Approach

The solution uses Depth-First Search (DFS) to explore the binary tree.

A path is maintained while moving from the root toward each leaf.

When a leaf node is reached, the complete path is added to the result.

For every non-leaf node, DFS continues through both the left and right children.

## Example

For the tree:

```text
    1
   / \
  2   3
   \
    5
```

The root-to-leaf paths are:

```text
1 -> 2 -> 5
1 -> 3
```

Therefore, the result is:

```text
["1->2->5", "1->3"]
```

## Complexity

* Time: O(n)
* Space: O(h)

Here, `n` is the number of nodes and `h` is the height of the tree.

## Key Learning

This problem helped me practice:

* Binary Trees
* Depth-First Search
* Recursion
* Root-to-leaf traversal
* Building paths during tree traversal

## Conclusion

DFS provides a simple way to explore every root-to-leaf path. Whenever a leaf node is reached, the current path is stored as one valid answer.

**Author: T. Nandhini**
