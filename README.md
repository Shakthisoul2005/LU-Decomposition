# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
```
(i) To find L and U matrix
1.Input Matrix: Read the square matrix (or rectangular matrix) input from the user.
2.Convert to NumPy Array: Parse the input into a NumPy array for efficient numerical computations.
3.Perform LU Decomposition: Use the scipy.linalg.lu function to compute the LU decomposition, yielding the permutation matrix (P), lower triangular matrix (L), and upper triangular matrix (U).
4.Extract L and U Matrices: Ignore the permutation matrix and extract the L and U matrices from the decomposition result.
5.Output the L Matrix: Print the L (lower triangular) matrix.
6.Output the U Matrix: Print the U (upper triangular) matrix.
7.End Program: Ensure the program ends cleanly after displaying the results.
```
```
(ii) To find the LU Decomposition of the matrix

1.Input Matrix and Vector: Read the coefficient matrix and the right-hand-side vector 
b from the user.
2.Convert to NumPy Arrays: Parse both the matrix and vector inputs into NumPy arrays for numerical processing.
3.Perform LU Factorization: Use scipy.linalg.lu_factor to compute the LU decomposition of the matrix.
4.Solve the System: Pass the LU decomposition result and the vector 
𝑏 to scipy.linalg.lu_solve to solve the system of equations.
5.Extract Solution: Obtain the solution vector from the output of lu_solve.
6.Output Solution: Print the solution vector, representing the values of the unknowns.
7.End Program: Ensure the program concludes after displaying the solution
```


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

