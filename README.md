# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Read the input matrix (and right-hand side vector for solving equations) from the user.
2. Convert the given input into a NumPy array.
3. Apply LU decomposition to factorize the matrix into Lower triangular matrix (L) and Upper triangular matrix (U).

4. Display the L and U matrices, and if required, solve the system of linear equations using the decomposed matrices.


## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: GOWTHAM M
RegisterNumber: 212225100013
'''
import numpy as np
from scipy.linalg import lu

matrix=np.array(eval(input()))
P,L,U=lu(matrix)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
Program to find L and U matrix using LU decomposition.
Developed by: GOWTHAM M
RegisterNumber: 212225100013
'''

import numpy as np
from scipy.linalg import lu_factor,lu_solve

Matrix=np.array(eval(input()))
constant=np.array(eval(input()))
piv,lu=lu_factor(Matrix)
result=lu_solve((piv,lu),constant)
print(result)

```

## Output:
(i) To find the L and U matrix

<img width="1252" height="892" alt="image" src="https://github.com/user-attachments/assets/a98a388b-3bc2-4b83-92f7-1c7eee72ce3c" />


(ii) To find the LU Decomposition of a matrix
<<img width="1342" height="925" alt="image" src="https://github.com/user-attachments/assets/be745920-8a08-46b1-9eb9-fe5642b3a30d" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

