# Rotate 2D Matrix
![image](https://github.com/ugoem/alx-interview/assets/24642339/983ccab2-3cce-4aab-bfab-5cc73f27e170)

# Requirements
## General
* Allowed editors: ``vi, vim, emacs``
* All your files will be interpreted/compiled on ``Ubuntu 20.04 LTS using python3 (version 3.8.10)``
* All your files should end with a new line
* The first line of all your files should be exactly ``#!/usr/bin/python3``
* A ``README.md`` file, at the root of the folder of the project, is mandatory
* Your code should use the ``pycodestyle style (version 2.8.0)``
* You are not allowed to import any module
* All modules and functions must be documented
* All your files must be executable

Question
Given an n x n 2D matrix, rotate it 90 degrees clockwise.

-> Prototype: def rotate_2d_matrix(matrix): Do not return anything. The matrix must be edited in place. You can assume the matrix will have 2 dimensions and will not be empty.

expected output

```
jessevhedden$ cat main_0.py
#!/usr/bin/python3
"""
Test 0x07 - Rotate 2D Matrix
"""
rotate_2d_matrix = __import__('0-rotate_2d_matrix').rotate_2d_matrix

if __name__ == "__main__":
    matrix = [[1, 2, 3],
              [4, 5, 6],
              [7, 8, 9]]

    rotate_2d_matrix(matrix)
    print(matrix)

jessevhedden$
jessevhedden$ ./main_0.py
[[7, 4, 1],
[8, 5, 2],
[9, 6, 3]]
jessevhedden$
```
Now if you look closely the columns are reversed for all ith indexes in each row and also the size of the matrix is maintained. so get the indexes of the rows in the matrix(outer iteration/loop) and now iterate the matrix(inner loop).

On your inner loop, form a new list(row) containing the ith element of all rows visited then append this to the new_matrix object.

lastly, reassign the new_matrix to the matrix.

if you need more help reach out, Happy coding
