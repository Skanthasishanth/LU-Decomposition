# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1 :
Read the elements of augmented matrix into arrays a and b
### Step 2 :
Calculate elements of L and U
### Step 3 :
Print elements of L and U
### Step 4 :
Find V by solving LV = B by forward substitution
### Step 5 :
Find X by solving UX = V by backward substitution
### Step 6 :
Print Array X as the solution



## Program:
(i) To find the L and U matrix
```
#Program to find the L and U matrix.
#Developed by: S Kantha Sishanth
#RegisterNumber: 22007660
import numpy as np   #from numpy import array
from scipy.linalg import lu
arr=eval(input())
A=np.array(arr)
P,L,U=lu(A)
print(L)
print(U) 

```
(ii) To find the LU Decomposition of a matrix
```
#Program to find the LU Decomposition of a matrix.
#Developed by: S Kantha Sishanth
#RegisterNumber: 22007660
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=eval(input())
res=lu_factor(A)
solution=lu_solve(res,B)
print(solution)
```

## Output:
### For (i) To find the L and U matrix
!['output'](/img01.png)
### For (ii) To find the LU Decomposition of a matrix
!['output'](/img02.png)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

