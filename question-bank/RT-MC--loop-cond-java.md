The following Java method produces the output shown below. 
Determine which of the given inputs would produce this output.

``` 
public class ReverseTrace {                                                                                
                                                                                                             
  public static int countIncreases(int[] arr) {                                                          
      int count = 0;                                                                                     
      for (int i = 1; i < arr.length; i++) if (arr[i] > arr[i-1]) count++;                                                                                   
      return count;                                                                                      
  }                                                                                                      
                                                                                                             
  public static void main(String[] args) {                                                               
      int[] input = ???;  // Which input produces the output?                                            
      int output = countIncreases(input);                                                                
      System.out.println(output);                                                                        
  }                                                                                                      
}                                                                                                          
```                                                                                                              

Output: 3                                                                                                          
                                                                                                             
Which input array produces this output?                                                                    
                                                                                                             
A) {2, 1, 3, 4, 2}                                                                                     
B) {5, 1, 2, 3, 0}                                                                                         
C) {1, 3, 2, 4, 5}                                                                                          
D) {4, 3, 5, 6, 2}                                                                                         
                                                                                                             

Rubric: correct answer is C                                                                                         
                                                                                                             
Explanation: The method counts how many times a value is greater than the previous value (ascending consecutive pairs). 
                                                                                                             
