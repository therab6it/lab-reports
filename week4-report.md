# Code changes


Here are some code changes that from labs 3 and 4.

Have fun!


## Number one

![image](https://user-images.githubusercontent.com/97642829/151638960-c20c6bf1-b977-475b-877e-65f2ec780a1f.png)  


The test file that induces this failure is [Test File 7](https://github.com/therab6it/markdown-parse/blob/main/test-file7.md)  


Screenshot of the symptom:  
![image](https://user-images.githubusercontent.com/97642829/153681972-7c142f2a-c3b4-4f11-9691-56532c683a26.png)


Description:   
The code causes an infinite while loop. The changes help resolve the issue of a file containing just ```)[``` to not have an infinite while loop. However, there were still bugs in the code which had to be fixed, but at this point, the changes helped resolve the infinite while loop.


---
## Number two

![image](https://user-images.githubusercontent.com/97642829/153682937-24ecdb2d-ed31-4f70-ae5e-7a4612f0fade.png)


The test file that induces this failure is [Test File 5](https://github.com/therab6it/markdown-parse/blob/main/test-file5.md)   


Screenshot for the symptom:   
![image](https://user-images.githubusercontent.com/97642829/153309895-7d6bab9f-1d4e-4c08-b42a-7889788593dd.png)   


Description:    
The initial code is structured in such a way that it does not account for the possibility of text appearing in between the end of the link header and the beginning of the link address container, i.e. text in between the ']' and '('. The altered code tackles this issue by checking specifically for a ```](```, which only passes if there is no text between the ']' and '('.



---
## Number three  

![image](https://user-images.githubusercontent.com/97642829/153307706-b09ae2d0-a091-41a9-889f-78089a4c8c05.png)  


The test file that induces this failure is [Test File 2](https://github.com/therab6it/markdown-parse/blob/main/test-file2.md).  


Screenshot for the symptom:  
![image](https://user-images.githubusercontent.com/97642829/153307526-bc12c65e-86ed-4de7-8cb5-57b77c865da5.png)  


Description:  
The while loop was written in a way without considering the possibility of there being text after the links. This caused the infinite while loop, which is fixed when the while loop stops after finding ```'('```. This stops the while loop at the end of the link, although it must be noted that this did not produce the right output. It was, however, a step in the right direction.

