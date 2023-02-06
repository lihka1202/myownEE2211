The process of **detecting and remove corrupted data from a record, set or a table is considered to be data cleaning**

- One example is clipping **outliers**
- Another one is handling the missing features

# Handling Missing Features
There are 3 main ways of handling missing features
- Removing the examples with missing features from the data set
	- Can be done if the dataset is big enough so we can sacrifice some training examples
	- Can remove if there is some priority to the data
- Using a learning algo that can deal with missing data
	- A [[random forest]]?
		- *What is this?*
- Using a **Data Imputation Technique**
	- Again what is this?

2 main methods are described:
- Method 1: Replace the missing value of a feature by an average value of this feature in the dataset. This makes sense as added in the average value doesnt really change the mean.
  In more mathy terms:
  $$
  \hat{x^{(j)}} <- \frac{1}{N} \sum_{i=1}^{N}x_{i}^{j}
  $$
Again, I represents the feature i and j represents which data set. More on this later

- Method 2: Highlight the missing value
  This can generally be done by replacing the missing value with a value outside the normal range of values
  For example if the normal range is [0,1], then you can replace that value with a -1 and ensure to train the algorithm to differentiate between these features.
