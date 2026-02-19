The following Java program produces the output shown below. Your task is to determine    
what the input must have been. Write down the **exact input** that was passed to the `transform` method to 
produce the given output.                                                                                  
                                                                                                             
                                                                                                             
```                                                                                                   
  public class TracingProblem {                                                                              
                                                                                                             
      public static String transform(String input) {                                                         
          String result = "";                                                                                
          for (int i = 0; i < input.length(); i++) {                                                         
              char c = input.charAt(i);                                                                      
              if (i % 2 == 0) {                                                                              
                  result = result + c;                                                                       
              } else {                                                                                       
                  result = c + result;                                                                       
              }                                                                                              
          }                                                                                                  
          return result;                                                                                     
      }                                                                                                      
                                                                                                             
      public static void main(String[] args) {                                                               
          String input = "???";  // What was the input?                                                      
          String output = transform(input);                                                                  
          System.out.println(output);                                                                        
      }                                                                                                      
  }                                                                                                          
```                                                                                                             

Output: nhyPto                                                                                                     
                                                                                                             
What was the input string? ___________________________                                                     
                                                                                                             
Rubric: correct answer is "Python""                                                                                           
                                                                                                             
  Tracing explanation (you might require students to show their work):                                                                      
  Input: "Python"                                                                                            
  i=0, c='P', even index → append to end:    result = "P"                                                    
  i=1, c='y', odd index → prepend to start:  result = "yP"                                                   
  i=2, c='t', even index → append to end:    result = "yPt"                                                  
  i=3, c='h', odd index → prepend to start:  result = "hyPt"                                                 
  i=4, c='o', even index → append to end:    result = "hyPto"                                                
  i=5, c='n', odd index → prepend to start:  result = "nhyPto"                                               
                                                                                                             