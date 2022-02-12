# Streamlining SSH Configuration     

Follow the instructions below to save some typing!   


### Step 1  
Open Windows Explorer and navigate to the folder called ```.ssh```. You should usually find it under the user profile for your computer.  

![image](https://user-images.githubusercontent.com/97642829/153685365-5ba270a7-c5c0-4f6a-b108-e6ab306c5ba0.png)   


### Step 2  
Inside the folder, right click and select ```Open with Code```. This opens the folder on VSCode.  

![image](https://user-images.githubusercontent.com/97642829/153685691-9e85b446-7239-488e-80c1-476752a7656f.png)  


### Step 3  
Click on the New File button (or right click and click on New File) and name it ```config```. Do NOT add an extension to the file.


### Step 4
Add the following code in the file. Replace the ```cs15lwi22xxx``` with your ieg6 username.  

```
Host ieng6
	HostName ieng6.ucsd.edu
	User cs15lwi22xxx
 ```   
 
 
### Step 5
Now, you can simply use the command ```ssh ieng6``` to login, using the username and the public key present in the folder. If it does not work, add the following line of code to the file to help it navigate to the public key file in the folder. Remember to indent the line with the Tab key, keeping it in line with the preceeding lines of code. Also, replace the ```<your profile name>``` with the name of your user profile on your computer.
```
 	IdentifyFile C:\Users\<your profile name>\.ssh\id_rsa
 ```     
        
        
---      
    
      
       
 ![image](https://media.giphy.com/media/5IT69msgpaOcg/giphy.gif)
 
