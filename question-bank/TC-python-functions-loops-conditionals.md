Consider the following code:


```
  def foo(x):
      if x < 0:
          return "N"
          
      if x % 2 != 1:
          return "E"
      else:
          return "O"

  def get_all(lst):
      result = ""

      for n in lst:
         result += foo(n)

      return result

  if __name__ == "__main__":
      numbers = [-4, 1, 3, 6]
      result = get_all(numbers)
      print(result)
```      



In the space below, indicate what this would print. For credit your answer must be EXACTLY correct, so a few hints:

* Do not worry about newlines or whitespace, only letters would be printed
* The question is case sensitive, lowercase letters will not be correct.

Rubric:
- [ ] +1 for `"NOOE"` 


