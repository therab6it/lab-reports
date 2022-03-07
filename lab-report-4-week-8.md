## MarkdownParse repositories   

My MarkdownParse repo:    
[not-a-virus.exe](https://github.com/therab6it/markdown-parse)     
       
Reviewed repository:     
[likely-a-virus.exe](https://github.com/PierreBeur/markdown-parse)   
    
    
---     
     
     
## Tests written for snippets   
      
![image](https://user-images.githubusercontent.com/97642829/156686718-fcafd077-aa34-4011-adc4-19d4b8133dc3.png)
    
      
---   
    
    
## Running tests on my MarkdownParse
      
```
.E.E.E
Time: 0.015
There were 3 failures:
1) snippetOneTest(MarkdownParseTest)
java.lang.AssertionError: expected:<[`google.com, google.com, ucsd.edu]> but was:<[url.com, `google.com, google.com, ucsd.edu]>
        at org.junit.Assert.fail(Assert.java:89)
        at org.junit.Assert.failNotEquals(Assert.java:835)
        at org.junit.Assert.assertEquals(Assert.java:120)
        at org.junit.Assert.assertEquals(Assert.java:146)
        at MarkdownParseTest.snippetOneTest(MarkdownParseTest.java:79)
2) snippetThreeTest(MarkdownParseTest)
java.lang.AssertionError: expected:<[https://ucsd-cse15l-w22.github.io/]> but was:<[
    https://www.twitter.com
,
    https://ucsd-cse15l-w22.github.io/
, github.com

And there's still some more text after that.

[this link doesn't have a closing parenthesis for a while](https://cse.ucsd.edu/



, https://cse.ucsd.edu/



]>
        at org.junit.Assert.fail(Assert.java:89)
        at org.junit.Assert.failNotEquals(Assert.java:835)
        at org.junit.Assert.assertEquals(Assert.java:120)
        at org.junit.Assert.assertEquals(Assert.java:146)
        at MarkdownParseTest.snippetThreeTest(MarkdownParseTest.java:94)
3) snippetTwoTest(MarkdownParseTest)
java.lang.AssertionError: expected:<[a.com, a.com(()), example.com]> but was:<[a.com, b.com, a.com((, example.com]>
        at org.junit.Assert.fail(Assert.java:89)
        at org.junit.Assert.failNotEquals(Assert.java:835)
        at org.junit.Assert.assertEquals(Assert.java:120)
        at org.junit.Assert.assertEquals(Assert.java:146)
        at MarkdownParseTest.snippetTwoTest(MarkdownParseTest.java:86)

FAILURES!!!
Tests run: 3,  Failures: 3
```
    
A screenshot could not be included because the screen was too small to fit the entire output.
    
---    

   
## Running tests on reviewed java file
    
![image](https://user-images.githubusercontent.com/97642829/156697298-714a7872-c72e-4f27-a59a-83d3e2b503df.png)   
     
      
---
    
    
## For FAQs sake
    
### Question 1
It will take more than more than 10 lines for my program to be able to work with backticks. I would need for loops that iterate through each line if the code and if statements to verify, in order to record the start and end of the backtick.    
     
### Question 2 
It will take more than 10 lines for my program to be able to handle parentheses as a part of the link. The reason is it takes only one set of parentheses into account and does not run accurately in case of a "nested" set of parentheses. I would need couple new if statements and variables to properly tackle this situation.
      
### Question 3
It will take less than 10 lines for my program to be able to handle newline characters in links. I would probably take the input from the md file as a single line. I would need to adjust my ```getLinks()``` method, and remove the for loop that iterates through lines and compares them.
    
     
