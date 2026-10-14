# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

##5a Algorithm
1. import os and numpy module packages and import lu from scipy.linalg.
2. Get input and convert to matrix form in the code.
3. Find the L and U matrices in code and store in variables.
4. Print the result.
##5b Algorithm
1. import os and numpy module packages and import lu_solve and lu_factor from scipy.linalg.
2. Receive inputs from user and convert it to matrices in code.
3. Solve using the inputs and find the LU Decomposition.
4. Print the result.

## Program:
(i) To find the L and U matrix
```
/*
Program to find the L and U matrix.
Developed by: Harish Bakavadh J
RegisterNumber: 26007865
*/
'''Program to find L and U matrix using LU decomposition.
Developed by: Harish Bakavadh J
RegisterNumber: 26007865
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U= lu(A)
print(L)
print(U)
```
(ii) To find the LU Decomposition of a matrix
```
/*
Program to find the LU Decomposition of a matrix.
Developed by: Harish Bakavadh J
RegisterNumber: 26007865
*/
'''Program to solve a matrix using LU decomposition.
Developed by: Harish Bakavadh J
RegisterNumber: 26007865
'''
import os
os.environ["OPENBLAS_NUM_THREADS"]="1"
# To print X matrix (solution to the equations)
import numpy as np
from scipy.linalg import lu_factor,lu_solve
a=np.array(eval(input()))
b=np.array(eval(input()))
l,p=lu_factor(a)
x=lu_solve((l,p),b)
print(x)
```

## Output:
###5a output
<img width="851" height="900" alt="image" src="https://github.com/user-attachments/assets/69374f9c-ff0c-4b40-b32f-2a25255ebe65" />
<img width="918" height="947" alt="image" src="https://github.com/user-attachments/assets/a94a02ed-3ff6-4081-9f28-1df89d81ff9f" />
###5b output
<img width="898" height="918" alt="image" src="https://github.com/user-attachments/assets/ebbdbf9f-11ff-442f-9ff4-b50b506726a7" />



## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

