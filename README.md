# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1: Import the numpy module to use the built-in functions for calculation

### Step 2: Prepare the lists from each linear equations and assign in np.array()

### Step 3: Using scipy.linalg import lu ,we can find L and U matix.

### Step 4: By using lu_factor ,lu_solve .we can find lu decomposition matrix.

### Step 5: End the program

## Program:
(i) To find the L and U matrix
```
'''Program to find L and U matrix using LU decomposition.
Developed by: Balaji B
RegisterNumber: 212225040040'''
import os
os.environ['OPENBLAS_NUM_THREADS']="1"
import numpy as np
from scipy.linalg import lu
a=np.array(eval(input()))
piv,Lmatrix,Umatrix=lu(a)
print(Lmatrix)
print(Umatrix)
```
(ii) To find the LU Decomposition of a matrix
```
'''Program to solve a matrix using LU decomposition.
Developed by: Balaji B
RegisterNumber: 212225040040
'''
import os
os.environ['OPENBLAS_NUM_THREADS']="1"
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
piv,lu=lu_factor(a)
result=lu_solve((piv,lu),b)
print(result)
```

## Output:
![alt text](<Screenshot 2026-05-24 142850.png>)
![alt text](<Screenshot 2026-05-24 142902.png>)

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

