# ECE-2112-PA-2
Made by: Henley Lorin M. De Guzman | 2ECEB

This repository contains the Programming Assignment #2 for the course ECE2112 "Advanced Computer Programming and Algorithms" in the A.Y. 2026 - 2027. This assignment covers three Python programming problems related to Module 2, titled Numpy.

#**A. REPRODUCIBLE NORMALIZATION PROBLEM**

Create a reproducible random 5x5 integer ndarray named X. 

The following functions and methods were used and executed in this problem:

1) `np.random.seed()` - The code that sets the random seed so the computer produces the exact same set of numbers every single time.

``` python
np.random.seed(2112)
```
2) `np.random.randit()` - The code that creates the 5 x 5 matrix X filled with random integers from 10 to 100.

``` python
X = np.random.randint(10, 101, size=(5, 5))
X
```
3) `np.mean()` - The code that computes the average (mean) value of all numbers in matrix X.

``` python
mean = np.mean(X)
mean
```
4) `np.std()` - The code that computes the population standard deviation 

``` python
std = np.std(X)
std
```
5) `X_normalized` - The code that normalizes the array using the Z-score formula so the new data has a mean of 0 and a standard deviation of 1.

``` python
X_normalized = (X - mean) / std
X_normalized
```

#**B. CUBES DIVISIBLE BY 4 PROBELEM**

Create the first 100 positive integers, cube every element and reshape the result into a 10 × 10 ndarray named C.

The following functions and methods were used in this problem:

1) `np.arange()** #).reshape()` - The code that generates integers 1 to 100, cubes each value, and reshapes them into a 10 x 10 grid C.

``` python
C = (np.arange(1, 101) ** 3).reshape(10, 10)
```
2) `div_by_4` - The code that filters matrix C to keep only the cubed numbers that are divisible by 4.

``` python
div_by_4 = C[C % 4 == 0]
div_by_4
```
3) `C.shape` - The code that checks and displays the dimensions of matrix C to prove it is 10 x 10.

``` python
print("Shape of C:", C.shape)
```
4) `div_by_4.size` - The code that counts and displays the total number of filtered elements.

``` python
print("\nSelected elements:", div_by_4.size)
```

#**C. ABOVE-MEAN SQUARES PROBELM**

Create a 6 × 6 ndarray named S containing the squares of the first 36 positive integers in increasing row-major order.

The following functions and methods were used in this problem:

1) `np.arange()** #).reshape()` - The code that generates integers 1 to 36, squares each value, and reshapes them into a 6 x 6 grid S.

``` python
S = (np.arange(1, 37) ** 2).reshape(6, 6)
```
2) `np.mean()` - The code that calculates the overall average of all squared numbers in grid S.

``` python
mean = np.mean(S)
```
3) `above_mean` - The code that filters matrix S to extract only the values strictly greater than the average.

``` python
above_mean = S[S > mean]
```
4) `above_mean.size` - The code that counts and displays how many squared values survived the filter.

``` python
print("\nNumber of selected elements:", above_mean.size)
```

Thank you for reading!

Programming Assignment #2: https://github.com/deguzmanhenleylorin/ECE-2112-PA-2/blob/main/Programming_Assignment_2.ipynb

#### **READ ME FILE HISTORY: **

September 1, 2026 - Initial README output uploaded.

September 2, 2026 - README output updated.

September 3, 2026 - README output finalized.
