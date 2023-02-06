There are many startegies to format the data, some of them are listed here:
- Binary Coding: To convert the various categories into Binary Form
	- One Hot Encoding: Simplify seveal entities with a single colour
	- The 3 main colours are RGB:
		- IE 
			- red = [1,0,0]
			- green = [0,0,1]
			- yellow = [0,1,0]
- Normalization: Linear scaling each variable to between [0,1]. This is also called mean normalization
	- Can be done by the following formula:
$$
x_{i} = \frac{x_{i}^{raw} - x^{min}}{x^{max} - x^{min}} , i = 1,2..M
$$

- Z-Score Standardisation: each independant dimension of the data is normally distributed. **The real question is how is this done**
- This is done based on the following formula
$$
x_{i} = \frac{x_{i}^{raw} - E[X]}{\sigma(X)},  i=1,2,...M
$$
