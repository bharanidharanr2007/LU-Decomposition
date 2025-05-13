# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
 1. Import numpy library using import statement.
 2. From scipy package import lu().
 3. Get input from user and pass it as an array.
 4. Get P,L,U matric using lu().
 5. Print L and U matrix

## Program:
(i) To find the L and U matrix
```
import numpy as np
from scipy.linalg import lu
A=np.array(eval(input()))
P,L,U=lu(A)
print(L)
print(U)
 

```
(ii) To find the LU Decomposition of a matrix
```
import numpy as np
from scipy.linalg import lu_factor,lu_solve
A=np.array(eval(input()))
b=np.array(eval(input()))
lu,piv=lu_factor (A)
X=lu_solve((lu,piv),b)
print(X)


```

## Output:
![lu decomposition]()
![image](https://github.com/user-attachments/assets/b0666c8c-09d6-42f9-917d-b5472683830e)
![image](https://github.com/user-attachments/assets/57241632-d96d-4ff2-9463-f6dce3260bbe)





## Result:
Thus the program to find the LU Decomposition of a matrix is written and verified using python programming.

