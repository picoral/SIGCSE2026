Check the two implementations that do exactly the same thing.

**A**

```
public static String doSomethingOne(int a, int b) {
  String out = "";
  for (int n = 0; n < b; n++) {
    int sum = a + n;
    if (sum % 2 != 0) out += sum;
  }
  return out;
}
```

**B**

```
public static String doSomethingTwo(int a, int b) {
   if (b <= 0) return "";
   if (a % 2 != 0) return a + doSomethingTwo(a+1, b-1);
   else return doSomethingTwo(a+1, b-1);
}
```

**C**

```
public static int doSomethingThree(int a, int b, int out) {
  if (b <= 0) return out;
  if (a % 2 != 0) return doSomethingThree(a+1, b-1, out+a);
  else return doSomethingThree(a+1, b-1, out);
}
```