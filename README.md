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

<img width="645" height="380" alt="image" src="https://github.com/user-attachments/assets/f06808e4-788f-400b-b07c-56223e2c6818" />

(ii) To find the LU Decomposition of a matrix

Program to find the LU Decomposition of a matrix.

<img width="590" height="347" alt="image" src="https://github.com/user-attachments/assets/402e1caa-32f4-431c-94fa-e0350dea5739" />


## Output:

<img width="1182" height="438" alt="image" src="https://github.com/user-attachments/assets/7225e2c1-e6d8-4439-a2ea-44245065ccb8" />

<img width="930" height="282" alt="image" src="https://github.com/user-attachments/assets/cba83a35-eebb-4e93-9a26-e74ea963fcc5" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

