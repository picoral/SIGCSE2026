Consider these three methods:


```
public static String doSomethingOne(int a, int b) {
  String out = "";
  for (int n = 0; n < b; n++) {
    int sum = a + n;
    if (sum % 2 != 0) out += sum;
  }
  return out;
}

public static String doSomethingTwo(int a, int b) {
   if (b <= 0) return "";
   if (a % 2 != 0) return a + doSomethingTwo(a+1, b-1);
   else return doSomethingTwo(a+1, b-1);
}

public static String doSomethingThree(int a, int b, String out) {
  if (b <= 0) return out;
  if (a % 2 != 0) return doSomethingThree(a+1, b-1, out+a);
  else return doSomethingThree(a+1, b-1, out);
}

```

Briefly explain the difference across the three methods above:

Rubric:

- [ ]  +1 `doSomethingOne` implements iteration
- [ ]  +1 `doSomethingTwo` implements regular recursion
- [ ]  +1 `doSomethingThree` implements tail recursion

What does the following main method print? 

```
public static void main(String[] args) {
        System.out.println(doSomethingOne(5, 8));
        System.out.println(doSomethingTwo(5, 8));
        System.out.println(doSomethingThree(5, 8, ""));
    }
```

Rubric:

- [ ]  +1 first statement prints `"111315"` 
- [ ]  +1 second statement prints `"111315"` 
- [ ]  +1 third statement prints `"111315"` 