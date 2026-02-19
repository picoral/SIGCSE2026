Given the following Python function, match each input (1-5) with its corresponding output (A-E). 
Write your answers in the format: 1-, 2-, etc.                                                      
   
```                                                                                                          
def process_list(data):                                                                                    
    result = []                                                                                            
    for i in range(len(data)):                                                                             
       if data[i] > i:                                                                                    
            result.append(data[i] * 2)                                                                     
        elif data[i] < i:                                                                                  
            result.append(data[i] - 1)                                                                     
        else:                                                                                              
            result.append(data[i])                                                                         
    return result                                                                                          
```   

Inputs:                                                                                                    
                                                                                                             
1. [5, 3, 1, 0, 2]                                                                                         
2. [0, 1, 2, 3, 4]                                                                                         
3. [2, 2, 2, 2, 2]                                                                                         
4. [1, 0, 3, 1, 5]                                                                                         
5. [4, 4, 0, 6, 1]                                                                                         
                                                                                                             
Outputs:                                                                                                   
                                                                                                             
A) [10, 6, 2, 0, 4]                                                                                        
B) [2, 4, 2, 6, 10]                                                                                        
C) [0, 1, 2, 3, 4]                                                                                         
D) [4, 2, 2, 4]                                                                                            
E) [8, 8, -1, 6, 3]                                                                                        
                                                                                                             
Match input with output:                                                                                             
                                                                                                             
- Input 1 matches Output: _____                                                                            
- Input 2 matches Output: _____                                                                            
- Input 3 matches Output: _____                                                                            
- Input 4 matches Output: _____                                                                            
- Input 5 matches Output: _____  


Answer Key:                                                                                                
                                                                                                             
1. A - [5, 3, 1, 0, 2] → [10, 6, 0, -1, 1]                                                                 
2. C - [0, 1, 2, 3, 4] → [0, 1, 2, 3, 4]                                                                   
3. B - [2, 2, 2, 2, 2] → [4, 4, 2, 1, 1]                                                                   
4. D - [1, 0, 3, 1, 5] → [2, -1, 6, 0, 10]                                                                 
5. E - [4, 4, 0, 6, 1] → [8, 8, -1, 12, 0]                                                                 
