# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Import numpy package
2. from scipy.linalg  import lu
3. solve using scipy.linlag(variable)
4. End the program

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
matrix=np.array(eval(input()))
piv,l_matrix,u_matrix=lu(matrix)
print(l_matrix)
print(u_matrix)
```
/*
Program to find the L and U matrix.
Developed by: 
RegisterNumber: 
*/
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: 
RegisterNumber: 
*/
```
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

