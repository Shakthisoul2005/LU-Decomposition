# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
1.Import Necessary Libraries: Import numpy as np for numerical computations and lu from scipy.linalg for LU decomposition.

2.Input the Matrix: Accept a matrix as input from the user. The input is expected in a format that can be evaluated as a valid Python list of lists.

3.Convert Input to a NumPy Array: Use np.array() to convert the evaluated input into a NumPy array for numerical operations.

4.Perform LU Decomposition: Call the lu() function from scipy.linalg on the input matrix. This function decomposes the matrix into three components:

*Piv: Permutation matrix (not used in this code).
*L: Lower triangular matrix.
*U: Upper triangular matrix.
5.Store Decomposed Matrices: Assign the lower triangular matrix to l_matrix and the upper triangular matrix to u_matrix.

6.Output the Lower Triangular Matrix: Print the lower triangular matrix (l_matrix).

7.Output the Upper Triangular Matrix: Print the upper triangular matrix (u_matrix).

8.Validate Input Matrix: Ensure that the input matrix is a valid square or rectangular matrix (implicitly handled by the LU function).

9.Handle Errors: If the matrix is not decomposable or invalid input is provided, the program will raise an error.

10.Display Results: Display the l_matrix and u_matrix as outputs, which represent the LU decomposition of the input matrix.








```  
## Program:
(i) To find the L and U matrix
```
Program to find the LU Decomposition of a matrix.
Developed by: Shakthivel v
RegisterNumber:24901278 

import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)
```
(ii) To find the LU Decomposition of a matrix
```
Program to find the LU Decomposition of a matrix.
Developed by: Shakthivel v
RegisterNumber:24901278

import numpy as np
from scipy.linalg import lu_factor,lu_solve
matrix=np.array(eval(input()))
b=np.array(eval(input()))
x=lu_factor(matrix)
solution=lu_solve(x,b)
print(solution)
```
## Output:
![image 1](<Screenshot 2024-11-26 224429.png>)
![Screenshot 2024-11-27 213729](https://github.com/user-attachments/assets/4794b843-cf7c-42c6-b30e-96dc4527fac1)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

