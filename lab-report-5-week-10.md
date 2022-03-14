## Finding the test  
   
Using the command ```diff <file-1> <file-2>``` a line-by-line comparison produces the following output.
     
![image](https://user-images.githubusercontent.com/97642829/158104033-d8f85dc0-ff37-4834-abb1-175f35f40a1e.png)     
     
Each block of output contains the following:     
  * ```<n1>c<n2>``` : line number of file-1 and file-2 that are compared   
  * ```< [link]```  : line from file-1 (Instructor's code's results)
  * ```> [link]```  : line from file-2 (Our group's code's results)
    
--- 
    
## Test File 194    
   
![image](https://user-images.githubusercontent.com/97642829/158155543-d966a56b-4075-456a-881a-153e97ea233e.png)     
     
This test file does not have a link defined in the correct syntax, and so, markdownParse must not output any links.    
     
This means our output must look like this: ```[]```      

![image](https://user-images.githubusercontent.com/97642829/158156751-6accf38a-bd73-412d-a4b8-dba085167d49.png)
    
This is the case with our group's code and not the instructor's. The instructor's program does not account for the syntax demanding a closed square bracket immediately preceeding  the opening parenthesis. This caused ```url``` to be incorrectly identified as a link, which the instructor's program outputs.
      
      
     
## Test File 506
    
![image](https://user-images.githubusercontent.com/97642829/158160577-ced1424a-be02-4d69-945d-f9eecc46e679.png)
    
This test file has the link defined in the correct syntax, and so, markdownParse must output the contents within the parentheses.

This means our output must look like this: ```[/url "title"]```     
     
![image](https://user-images.githubusercontent.com/97642829/158162437-c3958f3a-6aa0-49af-b605-28f5a71af4da.png)
     
And this is the case with our group's code. It however isn't with the instructor's.
     
![image](https://user-images.githubusercontent.com/97642829/158162274-f7aaa2b4-fe21-47d7-a539-72fc29d3516a.png)
     
As one of our groupmates pointed out, Github allows spaces in a link, which is why the instructor's code would not be the correct output in this case. It must treat the space character as a valid character that is a part of the link, and not replace it with a question mark as observed above.
       
---   
   
![image](https://c.tenor.com/iS66oB4_6SwAAAAd/soldier-family.gif)   
   
