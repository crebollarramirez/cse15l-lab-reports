# Lab Report 2
When working in labs, I forked the professors program. The TA told us that we will have our own copy of the code so we didn't work on the same file. We still collectivly found bugs in the code and discussed how to fix the bugs. Here is the code forked from the professor:

![Image](professorCode.png)

# Test files that will be used to test the program
[test-file](test-files/test-file.md)  [test-file2](test-files/test-file2.md)

# First Change of the Code
The professor's code didn't account to ignore image links so it adds them to the website links array which is incorrect. 

Since image links are very similar to website links, the program will add the image links to the list. The only difference that the image link has is the "!" at the start of the link which we can take into account in order to fix that bug in the algorithm. 

We added an instruction to ignore image links so we can only add website links to the ArrayList.

![image](step1.png)

This fix caused an issue if the first line didn't contain an image link, it will give us an out of bound error. 

**With an image link in the first line of the Test File:**

![Image](withfirstLine.PNG)

**Without an image link in the first line of the Test File:**

![Image](withoutImageLink.png)

As you can see, when there isn't a image link at the start of the Test File, there will be an index out of bound of -1 since the first bracket has an index of 0 since it's at the start of the file and has nothing before it. 

# Second Change of the Code
Now I have altered the code so there will be no error when it's check for a link in the first line but there is still a bug present after the updated code. 
![Image](secondChange.png)


# Third Change of the Code
![Image](full-code.png)



# Simplified and Fully Working Code:

This is the code fully working where it only takes the links for websites and completely ignored image links. 


# Summary
