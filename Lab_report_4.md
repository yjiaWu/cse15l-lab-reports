# Lab Report 4
**Step 4**
![image1](Labreport4_4.png)<br>
Key pressed: `ssh yiw128@ieng6-201.ucsd.edu` then I press `enter` <br>
Use `ssh` to log into `ieng6` server. This command line is used to log into ieng6 by using my own school account so that the terminal can run on school's computer.<br>

**Step 5**
![image2](Labreport4_5.png)<br>
Key pressed: "git clone git@github.com:yjiaWu/lab7.git" then I press `enter`<br>
Use `git clone` command to clone the the repository into `ieng6`. Since we should use the forked repository from Github, we use the password-protected `ssh key`, which is `git@github.com:yjiaWu/lab7.git`. This command line helps me to successfully clone the lab7 into the computer.<br>

**Step 6**
![image3](Labreport4_6.png)<br>
Key pressed: `cd lab7`<br>
This command line is used to change directory into lab7, so I can use terminal to make changes for lab7.<br>
Key pressed: `ls`<br>
This command line is used to list out all the files in `lab7` directory. I want to see what's the file's name for `bash` to run the test.<br>
Key pressed: `bash test.sh`
Use `bash` command to run the `test.sh` file. This command aims to run the tests in the directory to check the test results, so I can know if the java file has bugs. After press `enter`, the tests result shows in terminal. The result shows that 1 test fails, so it gives me a sign that the java file has a bug. <br> 

**Step 7**
![image6](Labreport4_7.3.png)<br>
![image4](Labreport4_7.png)<br>
![image5](Labreport4_7.2.png)<br>
Key press: `vim ListExamples.java`<br>
Use `vim` command to open the java file `ListExamples.java`. This command line allows me to see the java file in the terminal and make changes on the java file.<br>
Key press: `i` and then `delete`, then press `2`, and then press`esc`. <br>
I first press `i` to enter insert mode, so that I can edit the content of the file. I can directly locate the mouse to the place after the word I want to edit. For this example, I can locate the mouse after word `1`. Then I press `delete` to delete the word 1. Then I press `2` to change the word from 1 to 2 to make the code run succesfully. After all those, I press `esc` to exit back to normal mode. <br>
Key press: `:wc` `enter`<br>
After editing the file, I should exit back to the terminal. So I use `:wc` to save the changes and exit the `vim`. I should press `enter` to run the command. <br>

**Step 8**
![image7](Labreport4_8.jpg)<br>
Key press: `bash test.sh` then `enter`<br>
After I change the file, I should run the test again to make sure all tests are passed now. Use `bash` to run `test.sh`. This command aims to run the test file, and then `enter` can give me the test results in terminal. This time, the terminal shows that all the tests pass.<br>

**Step 9**
![image8](Labreport4_9.1.png)<br>
![image9](Labreport4_9.2.png)<br>
Key press: `git add .`<br>
This command line add all modified files or new files in the current directory to required area. 
Key press: `git commit -m "The file is commited to GitHub"`<br>
Use `commit` to save all the changes to the local git repository. Comman `-m` allows me to specify the commit mesage through terminal. This whole command line is used to save all changes in local git repository and appoint the commit message. 
Key press: `git push origin main`<br>
The command `git push` allows me to push the commited changes to GitHub. `main` indicates the branch in GitHub that I want to push the changes into. 




