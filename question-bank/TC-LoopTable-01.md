Given the function below:

```
def foo(strings):
  for i in range(len(strings)):
    for j in range(len(strings[i])):
      strings[i][j] = len(strings[i][j])
  return strings
```

Complete the `loop table` below with the corresponding values of `i`, `j`, `len(strings[i])`, `len(strings[i][j])` and `strings` for the following function call:

```
foo([["cat", "jump", "marvel"], ["smart"]])
```

This question is assessing whether you are able to:

* Read code
* Understand nested for loops

Rubric:
- [ ] +1 i values are all correct
- [ ] +1 j values are all correct
- [ ] +1 len(strings[i]) values are all correct
- [ ] +1 len(strings[i][j]) values are all correct
- [ ] +1 strings values are all correct
