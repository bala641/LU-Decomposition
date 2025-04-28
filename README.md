# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1. Initialize:

𝐿
L as an 
𝑛
×
𝑛
n×n identity matrix (1's on the diagonal, 0 elsewhere).

𝑈
U as an 
𝑛
×
𝑛
n×n zero matrix.


2.To find 
𝐿
[
𝑖
]
[
𝑗
]
L[i][j]:

𝐿
[
𝑖
]
[
𝑗
]
=
𝐴
[
𝑖
]
[
𝑗
]
−
(
𝑡
ℎ
𝑖
𝑛
𝑔
𝑠
𝑎
𝑙
𝑟
𝑒
𝑎
𝑑
𝑦
𝑓
𝑖
𝑙
𝑙
𝑒
𝑑
𝑏
𝑒
𝑓
𝑜
𝑟
𝑒
)
L[i][j]=A[i][j]−(thingsalreadyfilledbefore)
To find 
𝑈
[
𝑗
]
[
𝑖
]
U[j][i] (if 
𝑖
>
𝑗
i>j):

𝑈
[
𝑗
]
[
𝑖
]
=
𝐴
[
𝑗
]
[
𝑖
]
−
(
𝑡
ℎ
𝑖
𝑛
𝑔
𝑠
𝑎
𝑙
𝑟
𝑒
𝑎
𝑑
𝑦
𝑓
𝑖
𝑙
𝑙
𝑒
𝑑
𝑏
𝑒
𝑓
𝑜
𝑟
𝑒
)
𝐿
[
𝑗
]
[
𝑗
]
U[j][i]= 
L[j][j]
A[j][i]−(thingsalreadyfilledbefore)
​
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

