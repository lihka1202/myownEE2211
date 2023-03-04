
You can get the rank by essentially taking 2 main things

## Number of pivots in the RREF form

This is a lot harder as a few things need to be considered, what exactly is a pivot?

### Pivots
A pivot is essentially the first non zero element in the row.

Hence you can understand the [[Rank]] of a matrix by *converting it to RREF and finding out how many pivots there are*.

**Is there a way to get the RREF using python?**

Yep, you would need to import `sympy`. This would allow you to keep track of the RREF,should you ever need it.

This is what the function looks like:
```python
import sympy as sp
print(sp.Matrix(A).rref())
```




## Number of Linearly Independant rows

If you see hard enough, you would be able to find out how many rows/columns are **Linearly Dependant**, from there you can work your way out to find the rows that are LI

# How in Python?
I think in numpy or so there probably is some way to do it

In Numpy, you can use the `numpy.linalg.matrix_rank`. This should be able to get the rank that you need to get.

So the command is pretty simple:

it is `print(np.linalg.matrix_rank(A))` This would be able to generate the rank in the overall.

# Nature of solutions in Linear Algebra
X: design matrix
y: Target matrix

Xw = y

Very often we would wish to find w, which has the same dimensions as y. Dimensions of w are *d by 1*. The dimensions of x are *m by d*. Where **m is the number of training sets and d is the number of features**. Y is naturally a *m by 1* vector, as there is some outcome for every single row. Each **row** in X, is one sample. Based on matrix multiplication, this adds up to the answer. 

## For a linear system ther are 3 cases

For a system Xw = y, there are three scenarios
- Unique Solution
- No solution
- Infinitely Many solutions

Need to create an augmented matrix, in order to check whether they fit in any of the three cases. But how do you do this in python?

### Augmenting a Matrix in python
This can be done by using the `hstack` operation

```python
print(np.hstack((A,B)))
```

**I do think that the reshape command can be used, but on the overall, either one can be used**

So here are a few postulates,

In general we can claim that
$$
\overline{X} = [X | y].
$$

This is often called the augmented matrix.

### Unique Solution
Xw=y has a unique solution when
$$
rank(X) = rank(\overline{X}) = d
$$
d here is the number of features and how they correlate with the final output.

### No solution
Xw=y has no solutions when
$$
rank(X) < rank(\overline{X})
$$

Generally this happens when the number of equations is greater than the number of unknowns, this is over determined.

### Infinitely many solutions when
Xw=y has infinitely many solutions when the system is underdetermined, USUALLY.
$$
rank(X) = rank(\overline{X}) < d
$$


**A general note about what the rank could be**
$$
rank = min(m,n)
$$
Since the row rank and the column rank are mathematically defined to be the same, hence the rank is the min, as the rank cannot be more than *either number of rows or columns*


*Questions* Can an under determined system have a no solution
it can, if the original matrix is filled with vectors who are just linear multiples of themselves, and the addition of `y` would definitely increase the rank.

# Even determined system

Essentially in any case when the **Number of rows is equal to the number of columns** or simply when m = d.

Then the equation would be: Xw = y

Hence, the value of ==w== would be :
$$
w = X^{-1} y
$$

In the case the system is not even, then it can be one of the 2 systems:

# Over determined System
Some ways to say this:
- The number of equations is greater than the number of unkowns
- The number of samples is greater than the number of features
- m > d
This generally means that:
- X is tall
- X is non square --> singular 
However, we can find an approximate solution, called the ==LEAST SQUARE SOLUTIONS==


Now in a situation of this sort, if you want to find the value of w, you can do the following:
$$
w = \left( X^{T}X \right)^{-1} X^{T} y
$$

Note that since you are inverting something, it is very important to consider what does it mean to invert something. Or rather does the inverse even exist

So we can determine that:
$\left(X^{T}X \right)^{-1}$ only exists if X has full column rank. This means that the 
column rank must be equal to d


# Under determined systems

The number of unknown bigger than the number of equations

- X is fat
- X is not invertible

usually there are infinite solutions, we want to find one special solution


The solution is to find the least norm solution, this is the least distance solution


Essentially when we are given 

$$
w = X^{+}y
$$

here the 

$$
X^{+} = X^{T} \left( X X^{T}\right)^{-1}
$$


in gist

$$
w = X^{T} \left( X X^{T}\right)^{-1} y
$$

The right inverse exists iff
- X has full Row rank

# Sets
An unordered collection of objects, There can be no duplicates either 


# Affine functions
An affine function is a linear function plus a constant. In essence

$$
f(x) = a^{T}x + b
$$

Linear functions must pass through the origin, but affine functions do not have to. Hence **ALL affine functions are linear but not all linear functions are affine**

# Min
There can be global and local minimum/minima.

Local minima are the smallest values in the neihbourhood

Global Minima are the smallest values in the whole range

So the **min** returns the smallest value in the range and the arg min returns the argument that produces the smallest value



# Derivatives
![[Pasted image 20230228025215.png]]
![[Pasted image 20230228025353.png]]
![[Pasted image 20230228030303.png]]