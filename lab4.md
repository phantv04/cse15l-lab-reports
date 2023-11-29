# CSE 15L Lab Report #4: Thoai Phan

___

## Step 4: Log into ieng6

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/36eb219e-f362-4809-a40c-ee7cfd3a85de)

Keys pressed:
* `ssh` `< space >` `cs15lfa23eu@ieng6.ucsd.edu` --> This will log you into your ieng6 account.


___

## Step 5: Clone your fork of the repository

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/5b639fb0-5cb3-4464-9a60-74b8e7ae4c02)

Keys pressed:
* `git` `< space >` `clone` `< space >` `git@github.com:phantv04/lab7.git` --> This will clone the file into your current directory.


___

## Step 6: Run the tests, demonstrating that they fail

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/b81c9bec-c963-4839-808c-22c015c2420e)


Keys pressed:
* On Visual Studio Code, I pressed the play button on the left side to run the jUnit test cases.


___

## Step 7: Edit the code file to fix the failing test

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/611ea647-d2ea-49d5-929b-3b26a5b4f74a)

Keys pressed:
* Type `cd lab7` (if you haven't already)
* Type `vim ListExamples.java`
* Hold `j` until you get to the line --> this is the down arrow for Vim
* Press the right arrow `->` 6 times
* Press `x` to remove the 1 --> the `x` will remove the character that is being highlighted
* Press `i` to insert 2 at that position --> `i` command means insert in Vim
* Press `Esc` key to get out of edit mode
* Type `:wq!` to quit and save your work, and you should see that your code was fixed!


___

## Step 8: Run the tests, demonstrating that they now succeed

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/77f4c94f-2eeb-40d0-8c09-17778552ebed)


Keys pressed:
* On Visual Studio Code, I pressed the play button on the left side to run the jUnit test cases.


___

## Step 9: Commit and push the resulting change

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/5e1d46b1-9914-48da-a5aa-cff8c3dd2b9d)

Keys pressed:
* To add the new edited file to your directory:
`git` `< space >` `add` `< space >` `ListExamples.java`
  
* To commit the new changes of the file to your directory:
`git` `< space >` `commit` `< space >` `-m` `< space >` `"Lab 7!"`
  
* To push the new changes to your repository:
`git` `< space >` `push`
