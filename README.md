# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Import the numpy module to use the built-in functions for calculation

2.Prepare the lists from each linear equations and assign in np.array()

3.Apply LU factorization to matrix A using lu_factor() and Solve the linear equations using lu_solve().

4.Store the solution in variable X.

5.End the Program
## Program:
(i) To find the L and U matrix
```import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu

a = np.array(eval(input()))

p, l, u = lu(a)

print(l)
print(u)
```

(ii) To find the LU Decomposition of a matrix
```import os
os.environ["OPENBLAS_NUM_THREADS"]="1"

import numpy as np
from scipy.linalg import lu_factor, lu_solve

a = np.array([[3, 2, 7],
              [2, 3, 1],
              [3, 4, 1]])

b = np.array([4, 5, 7])

lu, piv = lu_factor(a)

x = lu_solve((lu, piv), b)

print(x)
```

## Output:
<img width="1192" height="440" alt="Screenshot 2026-05-29 085245" src="https://github.com/user-attachments/assets/ad4a0b86-ccdd-4bb1-82ba-a01b07401a18" />
<img width="1053" height="184" alt="Screenshot 2026-05-29 085338" src="https://github.com/user-attachments/assets/c6494cf8-0e74-497b-8b02-627c69f1cb43" />


## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

