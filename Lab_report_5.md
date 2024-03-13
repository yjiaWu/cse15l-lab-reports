# Lab Report 5

## Part 1 
The student post: <br>
I am testing the reserve method in the ArrayExamples.java, and run the ArrayTests.java. The the output said that one test failed for the reverse function. I believe it's the for loop for reverse method is wrong, so it didn't correctly reserve the array list into the new list. Below are my screenshots of the output and the code of the method. <br>
![image](Labreport5_1.1.png)<br>
![image](Labreport5_1.2.png)<br>

**TA response**
Yijia Wu: Try to replace the `arr` and `newArray`'s position in the for loop. Right now, you are copying the content in the `newArray` into the `arr`. You should do it in an oposite way, and return `newArray` at the end. 

**After the debugging**
The bug is acutally inside the for loop. I switch the position for `arr` and `newArray` to allow the the element in `arr` is copied into `newArray` in a reverse order through the for loop. Also, I change the returned varaible from `arr` into `newArray`, so that the output would be the reversed array list. I believe by doing this change, the for loop would copy the element in `arr` from the last element into the `newArray` from index 0 in an reverse order. 
![image](Labreport5_1.3.png)<br>

**Setup**
The file and direcotry needed are in the lab3. 
![image](Labreport5_1.4.png)<br>

