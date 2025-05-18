# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
# Program 1
### step 1:
Input matrix A (coefficients) and vector b (constants).

### step 2:
Perform LU decomposition of matrix A to get combined LU matrix and pivot array.

### step 3:
Use the LU factors to solve the linear system AX = b.

### step 4:
Compute the solution vector X.

### step 5:
Output the result X.

# Program 2:

### step 1:
Input matrix A.

### step 2:
Perform LU decomposition using scipy.linalg.lu() to obtain matrices P, L, and U.

### step 3:
Extract the lower triangular matrix L.

### step 4:
Extract the upper triangular matrix U.

### step 5:
Print matrices L and U.



## Program:
(i) To find the L and U matrix

'''Program to find L and U matrix using LU decomposition.
Developed by: BALA B
RegisterNumber: 212224100005
'''

~~~python
import numpy as np
from scipy.linalg import lu

A = np.array(eval(input()))
P, L, U = lu(A)
print(L)
print(U)
~~~
## Output:
![image](https://github.com/user-attachments/assets/6fad967d-6446-4e09-b68c-bb8b7a7b632f)




(ii) To find the LU Decomposition of a matrix
'''Program to solve a matrix using LU decomposition.
Developed by: 
RegisterNumber: 
'''
~~~python
import numpy as np
from scipy.linalg import lu_factor, lu_solve

A = np.array(eval(input()))
b = np.array(eval(input()))
lu, piv = lu_factor(A)
X = lu_solve((lu, piv), b)
print(X)
~~~
## Output:
![image](https://github.com/user-attachments/assets/c31c4486-db87-496a-b1d9-505ce1518727)


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

