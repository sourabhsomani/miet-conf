Lambda function is also known as anonymous function.

Syntax

`lambda arguments: expression`

Normal function looks like as follows

```python
def cube(y): 
    return y*y*y; 
```

In lambda

```python
cube=lambda x: x*x*x
print(cube(8))
```

Power of lambda

**filter**

```python
lst = [1,2,3,4,5,6,7,8] 
newlst = list(filter(lambda x: (x%2 == 0) , lst)) 
print(newlst) 
```

**map**

```python
lst = [1,2,3,4,5,6] 
squares = list(map(lambda x: x**2 , lst)) 
print(squares)
```

**reduce**
```python
from functools import reduce
lst = [1,2,3,4,5,6]
addition = reduce((lambda x, y: x + y), lst)
print(addition)
```