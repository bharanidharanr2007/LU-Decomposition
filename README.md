# LU Decomposition 

## AIM:
To write a program to find the LU Decomposition of a matrix.

## Equipments Required:
1. Hardware – PCs
2. Anaconda – Python 3.7 Installation / Moodle-Code Runner

## Algorithm
### Step 1: Start with the Matrix ( A )
Take the square matrix ( A ) (of order ( n )).
Create empty matrices ( L ) (lower triangular) and ( U ) (upper triangular).

### Step 2: Compute Elements of ( L ) and ( U )
For each row ( i ) (from ( 1 ) to ( n )):
Calculate ( Ui][j] ) for ( j \geq i ): [ Ui][j] = Ai][j] - \sum_{k=1}^{i-1} Li][k] \cdot Uk][j] ]
Calculate ( Li][j] ) for ( j < i ): [ Li][j] = \frac{Ai][j] - \sum_{k=1}^{j-1} Li][k] \cdot Uk][j]}{Uj][j]} ]
Diagonal of ( L ): Set ( Li][i] = 1 ).

### Step 3: Loop Through All Rows
Repeat Step 2 for all rows of ( A ) until ( L ) and ( U ) are fully filled.

### Step 4 :
The matrix ( A ) is expressed as ( A = LU ), where:- ( L ) is a lower triangular matrix with ( 1 )s on the diagonal.
( U ) is an upper triangular matrix.


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

