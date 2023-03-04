```python
X = np.array([[1,1],[3,4]])
y = np.array([0,1])

if(X.shape[0]>X.shape[1]):
    print("Overdetermined")
elif(X.shape[0]<X.shape[1]):
    print("Under")
else:
    print("EVEN")
    
#print(np.linalg.inv(X))
print(np.linalg.inv(X) @ y)
```

Q6

When given in a certain form, make sure to use X.T instead of the normal one, to check for the constrained forms


Q8.

Just multiply to see how it goes eventually


