# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm

## Sub-Experiment 1: Use LU Decomposition to find L and U matrix

### Step 1:

Import the `os` and `numpy` modules, set `OPENBLAS_NUM_THREADS` to `1`, and import the `lu` function from `scipy.linalg`.

### Step 2:

Get the matrix as input from the user and convert it into a NumPy array using `np.array()` and `eval()`.

### Step 3:

Using the `lu()` function, perform LU decomposition on the given matrix and obtain the permutation matrix `P`, lower triangular matrix `L`, and upper triangular matrix `U`.

### Step 4:

Print the `L` and `U` matrices obtained from the LU decomposition and end the program.

---

## Sub-Experiment 2: Use LU Decomposition to solve a matrix

### Step 1:

Import the `os` and `numpy` modules, set `OPENBLAS_NUM_THREADS` to `1`, and import `lu_factor` and `lu_solve` from `scipy.linalg`.

### Step 2:

Get the coefficient matrix `A` and constant matrix `b` as input from the user and convert them into NumPy arrays.

### Step 3:

Use `lu_factor()` to perform LU factorization of matrix `A`, and use `lu_solve()` with the factorized matrix and `b` to find the solution `X`.

### Step 4:

Print the solution matrix `X` and end the program.

## Program:
(i) To find the L and U matrix

Program to find the L and U matrix.

```
'''Program to find L and U matrix using LU decomposition.
Developed by: MAHASHREE S
RegisterNumber: 212225230163
'''

import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))

P, L, U = lu(A)

print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix

Program to find the LU Decomposition of a matrix.

```
'''Program to solve a matrix using LU decomposition.
Developed by: MAHASHREE S
RegisterNumber: 212225230163
'''
import os
os.environ["OPENBLAS_NUM_THREADS"] = "1"

import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()), dtype=float)
b = np.array(eval(input()), dtype=float)

lu, piv = lu_factor(A)
X = lu_solve((lu, piv), b)
print(X)
```

## Output:

<img width="1442" height="888" alt="image" src="https://github.com/user-attachments/assets/52332d49-9fba-4ebe-a01c-693e5c25d24c" />

<img width="1510" height="853" alt="image" src="https://github.com/user-attachments/assets/86ae75be-a86a-4a6f-a465-e9c85580ae0d" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

