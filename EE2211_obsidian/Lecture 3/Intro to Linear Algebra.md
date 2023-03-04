- A scalar is a simple numerical value like 15 or -3.4 or something like that
	- The focus is more on the real numbers than those in the complex plane
- Variables or constants that take scalar values are denoted by either *x or a*

# Vectors, Matrices, Notations
- A vector is an ordered list of scalar values
	- Denoted by some bold character like **x or a**
- In many books, vectors are usually written column wise, but they can be represented row wise as well, there is no requirement for them to be written in a single way

$$
\begin {bmatrix} 1 & 2 & 3 \\ a & b & c \end {bmatrix}
$$
The above was just a test, in actuality, vectors look a little more like this

In simpler terms, vectors look like this
$$
a = \begin{bmatrix} 2 \\ 3 \end{bmatrix}, b = \begin{bmatrix} 3 \\ 4 \end{bmatrix}, c = \begin{bmatrix} 5 \\ 6 \end{bmatrix}
$$


Generally, the **ith entry is denoted by a super script on the element value**. Ie

$$
a = \begin{bmatrix} 2^{(1)} \\ 3^{(2)} \end{bmatrix}
$$
But this is generally considered to be equivalent to the following:
$$
a = \begin{bmatrix} a_{1} \\ a_{2} \end{bmatrix}
= \begin{bmatrix} 2 \\ 3 \end{bmatrix}
$$

Vectors can generally be visualized in dimensions, with each element consisting of one dimension

You can plot these vectos in those dimensions, and then you would have a visual understanding of what these vectors are like

Something like this:
![[Pasted image 20230213135251.png]]

# Matrices
- Rectangular arrays stacked on top of each other
- Denoted by capital letters such as X or W
- **Usually for input data, rows represent samples and the columns represent features**
$$
\sum\limits_{a}^{b} x^{i} = x_{1} + x_{2} + x_{3} ...
$$
Capital Pi is also the same in a certain way, this usually implies multiplication over a very large range


# Systems of Linear Equations
- A collected of d-vectors is considered to be *linearly independant*, iff
$$
\beta_{1}x_{1} + \beta_{2}x_{2} ... \beta_{m}x_{m} =0
$$
holds for
$$
\beta_{1}, \beta_{2}, \beta_{3}....\beta_{m} != 0
$$

If any of these are **0, then the system is considered to be linearly dependant**

![[Pasted image 20230213141225.png]]


Note that if at any point in time, if all the rows or columns of a square matrix are **linearly independant**, then **X** is **invertible**


These equations can usually be written in matrix vector notation
in such a way:
$$
Xw = y
$$
Where
$$
X = \begin{bmatrix} x_{1,1} & x_{1,2} & x_{1,3} &...& x_{1,d}  \\ ... & ... & ... & ... & ...\\ ... & ... & ... & ... & ...\\... & ... & ... & ... & ...\\ x_{m,1} & x_{m,2} & x_{m,3} &...& x_{m,d} \end{bmatrix}, w = \begin{bmatrix} w_{1} \\ . \\ . \\. \\ w_{d} \end{bmatrix}, y = \begin{bmatrix} w_{1} \\ . \\ . \\. \\ w_{m} \end{bmatrix}
$$
