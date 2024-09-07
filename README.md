# PA-2-Numerical-Python
This repository includes the solution to different programming problems involving the Numpy Library. 

## 1. Normalization Problem
This code generates and prints a 5X5 array with random values and its normalized version 
```python
# import numpy to access its library
import numpy as np

# store the value of a random 5x5 ndarray in X
X = np.random.rand(5, 5)
# store the mean of X in variable A
A = X.mean()
# store the standard deviation of X in B
B = X.std()
# store the normalization formula in C
C = (X - A) / B

# prints the 5x5 array with original Values
print("The Normal Values are:")
print(X)

# prints the 5x5 array with the normalized values
print("The Normalized Values are:")
print(C)
```
**Output:** 

![image](https://github.com/user-attachments/assets/f5f13a19-2b67-4ea8-a52a-ee6f63b935d0)

## 2. Divisible By 3 Problem
This code prints out a 10X10 array filled with the squared values of the integers 1-100. It also prints the numbers within the array that are divisible by 3. 
```python
# import numpy to access its library
import numpy as np

# generates values inside an array ranging from 1-100 
X = np.arange(1, 101)
# square the values inside the array and declare it as A 
A = X * X
# Reshape array A into a 10X10 Matrix
B = A.reshape(10, 10)

# checks and filters the value divisible by 3 in A 
# returns an array filled with the numbers that are divisible by 3
C = A[A % 3 == 0]
# reshape the array into a 3X11 for readability 
D = C.reshape(3, 11)

# print the squares of the first 100 natural numbers
print("The squares of the first 100 natural numbers are:")
print(B)

# \n for readability 
print("\n") 

# prints the numbers divisible by 3 found on array B 
print("The numbers divisible by 3 are:")
print(D)
```
**Output:** 

![image](https://github.com/user-attachments/assets/152bf7e6-133f-42eb-a954-aae979a0bcc5)
