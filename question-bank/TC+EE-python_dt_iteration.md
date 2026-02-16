This question tests your understanding of looping patterns and overall access-patterns for the various data structures. Consider the following function:

```
def foo(structure):
    result = ""
    for something in structure:
        this_thing = str(structure[something])
        result += this_thing + " "
    return result
```

For each input below either indicate it would crash, or if it would run to completion, write out what the output would be. (if there are multiple possible correct outputs, for example because dictionaries and sets are unordered, give one possible output)

# A

```
fruit={"apple": 10, "pear": 30, "kiwi", 0}
print(foo(fruit))
```

# B

```
var= ["one", "two", "three"]
print(foo(var))
```

Rubric:
- [ ] +1 A runs, output is `"10 30 0"` 
- [ ] +1 B throws an error 