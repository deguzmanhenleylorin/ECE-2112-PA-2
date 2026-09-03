# ECE-2112-PA-2
Made by: Henley Lorin M. De Guzman | 2ECEB

This repository contains the Programming Assignment #2 for the course ECE2112 "Advanced Computer Programming and Algorithms" in the A.Y. 2026 - 2027. This assignment covers three Python programming problems related to Module 2, titled Numpy.

#**A. REPRODUCIBLE NORMALIZATION PROBLEM**

Create a reproducible random 5x5 integer ndarray named X. 

The following functions and methods were used and executed in this problem:

1) `np.random.seed()` - 
Example:
``` python
np.random.seed(2112)
```
2) `np.random.randit()` -
Example:
``` python
X = np.random.randint(10, 101, size=(5, 5))
X
```
3) `np.mean()` -
Example:
``` python
mean = np.mean(X)
mean
```
4) `np.std()` -
Example:
``` python
std = np.std(X)
std
```
5) `X_normalized` -
Example:
``` python
X_normalized = (X - mean) / std
X_normalized
```
6) `np.save` -
Example:
``` python
np.save("X_normalized.npy", X_normalized)
```

#**B. CUBES DIVISIBLE BY 4 PROBELEM**

Create the first 100 positive integers, cube every element and reshape the result into a 10 × 10 ndarray named C.

The following functions and methods were used in this problem:

1) `np.arange()** #).reshape()` -
Example:
``` python
C = (np.arange(1, 101) ** 3).reshape(10, 10)
```
2) `div_by_4` -
Example:
``` python
div_by_4 = C[C % 4 == 0]
div_by_4
```
3) `C.shape` -
Example:
``` python
print("Shape of C:", C.shape)
```
4) `div_by_4.size` -
Example:
``` python
print("\nSelected elements:", div_by_4.size)
```
5) `np.save` -
Example:
``` python
np.save("div_by_4.npy", div_by_4)
```

#**C. ABOVE-MEAN SQUARES PROBELM**

Create a 6 × 6 ndarray named S containing the squares of the first 36 positive integers in increasing row-major order.

The following functions and methods were used in this problem:

1) `np.arange()** #).reshape()` -
Example:
``` python
S = (np.arange(1, 37) ** 2).reshape(6, 6)
```
2) `np.mean()` -
Example:
``` python
mean = np.mean(S)
```
3) `above_mean` -
Example:
``` python
above_mean = S[S > mean]
```
4) `above_mean.size` -
Example:
``` python
print("\nNumber of selected elements:", above_mean.size)
```
5) `np.save` -
Example:
``` python
np.save("above_mean.npy", above_mean)
```

Thank you for reading!

Programming Assignment #2:

#### **READ ME FILE HISTORY: **

September 1, 2026 - Initial README output uploaded.
September 2, 2026 - README output updated.
September 3, 2026 - README output finalized.
