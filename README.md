# INVERSE-OF-A-MATRIX
## Aim:
To write a python program to find the inverse of a matrix
## Equipment’s required:
1. 	Hardware – PCs
2. 	Anaconda – Python 3.7 Installation / Moodle-Code Runner
## Algorithm:
1. Check if the Matrix is Invertible:
Ensure that the matrix 
𝐴
A is square (i.e., it has the same number of rows and columns, 
𝑚
=
𝑛
m=n).
Check if the determinant of 
𝐴
A, denoted as 
det
(
𝐴
)
det(A), is non-zero. If 
det
(
𝐴
)
=
0
det(A)=0, the matrix is not invertible and does not have an inverse.
2. Create the Augmented Matrix:
Form an augmented matrix 
[
𝐴
∣
𝐼
]
[A∣I], where 
𝐴
A is the matrix whose inverse is to be found, and 
𝐼
I is the identity matrix of the same size as 
𝐴
A.
3. Perform Gaussian Elimination:
Apply row reduction (Gaussian elimination) to the augmented matrix 
[
𝐴
∣
𝐼
]
[A∣I] with the goal of transforming 
𝐴
A into the identity matrix.
Perform the following steps for each column:
Find the pivot element (the first non-zero element in the column) and swap rows if necessary.
Normalize the pivot row by dividing all elements of the row by the pivot element.
Eliminate the entries below and above the pivot using row operations (subtract multiples of the pivot row from other rows).
Continue until the left side of the augmented matrix is the identity matrix 
𝐼
I.
4. Check for Identity Matrix:
After row reduction, if the left side of the augmented matrix is the identity matrix, the right side will be the inverse of 
𝐴
A.
If the left side cannot be reduced to the identity matrix, the matrix is singular (i.e., it does not have an inverse).
5. Extract the Inverse Matrix:
The right side of the augmented matrix 
[
𝐼
∣
𝐴
−
1
]
[I∣A 
−1
 ] now contains the inverse of 
𝐴
A, denoted as 
𝐴
−
1
A 
−1
 .


## Program:
```
import numpy as np
a=np.array([[2,1,1],[1,1,1],[1,-1,2]])
b=np.linalg.inv(a)
print(b)
```

## Output:
![Screenshot (44)](https://github.com/user-attachments/assets/9ede6325-3c1e-4f67-bc30-40430287de64)



## Result:
Thus the inverse of given matrix is successfully solved using python program

