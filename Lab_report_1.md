1. The working directory is  `/home`  <br>
The commend `cat` is used to duplicate the content based on the argument. If the commend `cat` follows no argument, when we return, we will get blank output because there is no content in the terminal.<br> 
The output is not an error. If the commend `cat` follows with no argument, it defaults duplicate the content in the terminal. Since the current working path has nothing in the terminal, so the output is blank.<br>

2. The working directory is */home*  <br>
For this code, commend `cat` follows the argument `lecture1`. The output warns us that `lecture1` is a directory. Therefore, we failed to duplicate any content from the argument *lecture1* <br>
This output is an error because we can't duplicate a direcotry. Therefore, we can't use a directory's name as the argument for cat. 
![image](Labreport1%20cat%201%20.png)<br>
3. The working directory is */home/lecture1/messages*<br>
The commend cat is used to duplicate the content in the argument. So this code duplicates the content in the file `en-us.txt`<br>
This output is not an error because it duplicates the content from en-us.txt successfully. 
![image](Labreport1%20cat%202.png)<br>
4. The working directory when the commend was run was */home/lecture1*<br>
The commend `cd` is used to change directory. When cd execute without arguments, the working directory will be changed back to home. So the working directory after the commend is */home*<br>
The output is not an error because the working directory is changed successfully.
![image](Labreport1%20cd%201%20.png)<br>
5. The working directory when the commend was run was */home<br>
The argument is `lecture1`, and this directs the working directory change to */home/lecture1*. So after this commend, the working directory becomes */home/lecture1*<br>
The output is not an error because we didn't get a message indicates that there is anthing wrong with the commend from the system.<br>
![image](Labreport1%20cd%202.png)<br>
6. The working directory when the commend was run was */home/lecture1/messages*<br>
The argument is a file name `en-us.txt` so the output warns that **en-us.txt is not a direcotry**.<br>
This output is an error. Since cd is used to change directory, we should add a directory's name as an argument instead of using a file as an argument. If we use file as an argument, the computer would warn us that an error occurs. 
![image](Labreport1%20cd%203.png)<br>
7. The working direcotry is */home/lecture1/messages*<br>
The commend `ls` is used to list out all the files in the directory. When `ls` follows no argument, it list out all the files in he default terminal. So the output is the 3 language files under `messages`.<br>
The output is correct since it successfully lists out all the files' name under `messages`
![image](Labreport1%20ls%201.png)<br>
8. The working directory is */home*<br>
The argument `lecture1` directs the commend to list out all the files under the directory `lecture1`. So the output are `Hello.java`, `Hello.class`, `messages` and `README`.<br>
The output is correct since it successfully listed out all four files' name under directory `lecture1`<br>
![image](Labreport1%20ls%202%20.png)<br>
9. The working direcytory is */home*<br>
The argument `Hello.calss` is a file name, and no other files under this file. So when we commend `ls Hello.class`, we can't find any file names to be listed, so the system would output a warning.<br>
The output is an error because the warning states that **ls: cannot access 'Hello.class': no such file or directory**. The warning tells us that there is no files or folders under current paths.<br>
![image](Labreport1%20ls%203.png)<br>



