Carefully study the code shown below. When run, this code could potentially produce at least 2 different
errors. You should identify specifically where each of these errors could occur, explain why it would occur, and
provide a way to fix the issue.

```
1 def run_code(words):
2    ''' You can expect words to be a list with 0 or more strings '''
3    if len(words) > 20:
4       if len(words[25]) == 'youtube':
5          return 'word is' + words[25]
6    
7    for w in words:
8       result += 10 * w
9    return result
```

Rubric:

- [ ]  +1 Identified one error -- line 3
- [ ]  +1 Identified one error -- line 8
- [ ]  +1 Explained error -- conditional `if len(words) > 20` does not guarantee that index `25` exists
- [ ]  +1 Explained how to fix error -- do `if len(words) <= 25` or `if len(words) >= 25` instead
- [ ]  +1 Explained error -- `result` variable is never initialized
- [ ]  +1 Explained how to fix error -- initialize `result` , something like `result = ""` since w is always a string 