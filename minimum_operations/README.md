# Minimum Operations

This project contains a Python script that calculates the fewest number of operations needed to result in exactly `n` `H` characters in a file.

## Requirements

*   Allowed editors: `vi`, `vim`, `emacs`
*   All files will be interpreted/compiled on Ubuntu 20.04 LTS using `python3` (version 3.4.3)
*   All files should end with a new line
*   The first line of all files should be exactly `#!/usr/bin/python3`
*   A `README.md` file, at the root of the folder of the project, is mandatory
*   Your code should use the PEP 8 style (version 1.7.x)
*   All modules and functions must be documented

## Task

### 0. Minimum Operations

In a text file, there is a single character `H`. Your text editor can execute only two operations in this file: `Copy All` and `Paste`. Given a number `n`, write a method that calculates the fewest number of operations needed to result in exactly `n` `H` characters in the file.

*   Prototype: `def minOperations(n)`
*   Returns an integer
*   If `n` is impossible to achieve, return `0`

#### Example:

`n = 9`

`H` => `Copy All` => `Paste` => `HH` => `Paste` => `HHH` => `Copy All` => `Paste` => `HHHHHH` => `Paste` => `HHHHHHHHH`

Number of operations: `6`

### Usage

```bash
$ cat 0-main.py
#!/usr/bin/python3
"""
Main file for testing
"""

minOperations = __import__('0-minoperations').minOperations

n = 4
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))

n = 12
print("Min # of operations to reach {} char: {}".format(n, minOperations(n)))

$ ./0-main.py
Min # of operations to reach 4 char: 4
Min # of operations to reach 12 char: 7
```