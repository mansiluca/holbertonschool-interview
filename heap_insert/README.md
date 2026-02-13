# Heap Insert

## Description

This project involves implementing a function to insert a value into a Max Binary Heap.

## Data Structures

The project uses the following data structures for the binary tree:

```c
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
typedef struct binary_tree_s heap_t;
```

## Requirements

*   Allowed editors: `vi`, `vim`, `emacs`
*   All your files will be compiled on Ubuntu 14.04 LTS using `gcc 4.8.4`
*   Compiler flags: `-Wall -Werror -Wextra -pedantic`
*   Your code should use the `Betty` style.

## Tasks

### 0. Heap - Insert

Write a function that inserts a value into a Max Binary Heap:

*   **Prototype:** `heap_t *heap_insert(heap_t **root, int value);`
*   `root` is a double pointer to the root node of the Heap.
*   `value` is the value to store in the node to be inserted.
*   Your function must return a pointer to the inserted node, or `NULL` on failure.
*   If the address stored in `root` is `NULL`, the created node must become the root node.
*   You have to respect a **Max Heap** ordering.
*   You are allowed to swap values between nodes to maintain the property.

**Repo:**
*   GitHub repository: `holbertonschool-interview`
*   Directory: `heap_insert`
*   File: `0-binary_tree_node.c`, `1-heap_insert.c`