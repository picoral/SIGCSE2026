Given a list of lists of floats, this function should return a new list with the average of each sublist in the argument list.

```
grades = [ [ 80.5, 90.5, 85.5],
           [96.0, 97.0],
           [100.0, 100.0, 80.0, 92.8]]
assert get_averages == [ 85.5, 96.5, 93.2]
```

Choose which implementation below solves the problem:

**A**
def get_averages(numbers):
    out = []
    total = 0
    for row in numbers:
        for grade in row:
            total += grade
        out.append(total/len(row))
    return out


**B**
def get_averages(numbers):
    out = []
    for row in numbers:
        total = 0
        for grade in row:
            total += grade
        out.append(total/len(row))
    return out

**C**
def get_averages(numbers):
    out = []
    for row in numbers:
        total = 0
        for grade in row:
            total += grade
        out.append(total)
    return out
    
    
Rubric:

- correct answer is B