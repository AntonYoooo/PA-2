# PA-2
This repository includes the solution to different programming problems involving the Numpy Library. 

## 1. Normalization Problem
#import numpy to access its library
import numpy as np

#store the value of a random 5x5 ndarray in X
X = np.random.rand(5, 5)
# store the mean of X in variable A
A = X.mean()
# store the standard deviation of X in B
B = X.std()
# store the normalization formula in C
C = (X - A) / B

#prints the 5x5 array with original Values
print("The Normal Values are:")
print(X)
#prints the 5x5 array with the normalized values
print("The Normalized Values are:")
print(C)

**Output:** The Normal Values are:
[[0.0429153  0.71320353 0.84346377 0.89792048 0.00908847]
 [0.27847999 0.24716525 0.6438421  0.30452875 0.96621432]
 [0.18870679 0.79441247 0.18555828 0.38369649 0.40057524]
 [0.86066334 0.55140194 0.04712129 0.71553944 0.81095392]
 [0.1058107  0.09822365 0.83620896 0.45017441 0.35128752]]
The Normalized Values are:
[[-1.38171428  0.79146717  1.21379165  1.390349   -1.49138624]
 [-0.61797595 -0.71950332  0.56658636 -0.53352171  1.61176854]
 [-0.90903497  1.05475952 -0.91924295 -0.27684725 -0.22212365]
 [ 1.26955542  0.2668806  -1.36807777  0.79904056  1.10838954]
 [-1.17779734 -1.20239577  1.19027039 -0.06131523 -0.38192229]]


## 2. Divisible By 3 Problem
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

**output:** The squares of the first 100 natural numbers are:
[[    1     4     9    16    25    36    49    64    81   100]
 [  121   144   169   196   225   256   289   324   361   400]
 [  441   484   529   576   625   676   729   784   841   900]
 [  961  1024  1089  1156  1225  1296  1369  1444  1521  1600]
 [ 1681  1764  1849  1936  2025  2116  2209  2304  2401  2500]
 [ 2601  2704  2809  2916  3025  3136  3249  3364  3481  3600]
 [ 3721  3844  3969  4096  4225  4356  4489  4624  4761  4900]
 [ 5041  5184  5329  5476  5625  5776  5929  6084  6241  6400]
 [ 6561  6724  6889  7056  7225  7396  7569  7744  7921  8100]
 [ 8281  8464  8649  8836  9025  9216  9409  9604  9801 10000]]


The numbers divisible by 3 are:
[[   9   36   81  144  225  324  441  576  729  900 1089]
 [1296 1521 1764 2025 2304 2601 2916 3249 3600 3969 4356]
 [4761 5184 5625 6084 6561 7056 7569 8100 8649 9216 9801]]
