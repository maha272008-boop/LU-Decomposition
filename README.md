# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
1.Read the matrix A from the user. 
2.Convert the input into a NumPy array. 
3.Perform LU decomposition of matrix A using lu(A).
4.Read the constant matrix/vector B from the user.Solve the system of equations. 

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: P.MAHALAKSHMI 
RegisterNumber:  25017517
*/
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by:P.MAHALAKSHMI 
RegisterNumber: 25017517
*/
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
B=np.array(eval(input()))
lu,pivot=lu_factor(A)
x=lu_solve((lu,pivot),B)
print(x)
```

## Output:
(i)
<img width="1142" height="688" alt="Screenshot 2025-11-20 100939" src="https://github.com/user-attachments/assets/12a54f88-8a2f-4af5-89de-ac90aaabc99b" />
<img width="1186" height="559" alt="Screenshot 2025-11-20 100958" src="https://github.com/user-attachments/assets/578f87f3-84a3-43ae-b2ff-1da049775bb3" />

(ii)
<img width="1227" height="691" alt="Screenshot 2025-11-20 101009" src="https://github.com/user-attachments/assets/b6da73b0-cae1-4223-a20f-7be334df701f" />
<img width="1139" height="327" alt="Screenshot 2025-11-20 101018" src="https://github.com/user-attachments/assets/02c52db6-9a62-4b08-8b2a-56dc659f04ef" />

## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

