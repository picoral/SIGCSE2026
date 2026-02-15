Shown below is a description of a function. After the description you will be shown three functions. You should select which of the three is the correct implementation. For the other two, identify and explain at least one issue with each one that would either cause an error, or cause the wrong answer to be produced. 

The description of the function is as follows:

Write a function named `validate_binary` . This function should have one parameter which you can expect will be a string. The function should determine if every character in the string is either a `1` or a `0`. For example:

```
assert validate_binary('12345') == "invalid"
assert validate_binary('1010') == "valid"
```

The three options are below:


**A**
```
1 def validate_binary(binary):
2    for c in binary:
3          if c == '0' and c == '1':
4              return 'invalid'
5    return 'valid'
```

**B**
```
1 def validate_binary(binary):
2    i = 0
3    while i < len(binary):
4        if binary[i] != '0':
5            if binary[i] != '1':
6                return 'invalid'
7        i += 1
8    return 'valid'
```

**C**
```
1 def validate_binary(binary):
2    i = 100
3    while i > 0:
4        if binary[i] < '0':
5            if i < '1':
6                return 'invalid'
7    i += 1
8    return 'valid'
```

This question is assessing whether you are able to:

* Read code
* Find bugs and resolve errors

Rubric:

- [ ]  +2 Multiple choice -- only the correct choice selected
- [ ]  +1 Identified one error
- [ ]  +1 Identified one error
- [ ]  +1 Explained how to fix error
- [ ]  +1 Explained how to fix error