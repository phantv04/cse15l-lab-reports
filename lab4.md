# CSE 15L Lab Report #4: Thoai Phan

___

## Step 4: Log into ieng6

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/36eb219e-f362-4809-a40c-ee7cfd3a85de)

Keys pressed:
* ssh < space > cs15lfa23eu@ieng6.ucsd.edu


___

## Step 5: Clone your fork of the repository

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/5b639fb0-5cb3-4464-9a60-74b8e7ae4c02)

Key pressed:
* git < space > clone < space > git@github.com:phantv04/lab7.git


* Using `-iname` with the `find` command will search for a file or directory that has the specific name in it, but will also match the letters case-insensitively.
* It is useful because if you forgot whether or not you have a certain file or directory on your computer, you can search for it. If there is no result, than that means that it does not exist.
* Additionally, if you forgot that your file started with a capital letter, this is useful because it does not matter in this case.


## Find Command-Line Option #2: Using -atime*

* On Directories:

        $ find technical -atime +1
        // No result

* On Files:

        $ find technical/biomed -atime +1
        // No result

* The command `-atime + 1` locates and prints a list of files or directories that was last accessed more than 1 day ago.
* There was no result in these commands because I used all of the files in technical from biomed, plos, etc. for my lab report.
* When I used the command `-atime -1`, which prints the files and directories used less than 1 day ago, a long list came out, whether from the directory technical or a subdirectory such as plos.
* This is useful because if you want to see what files and directories you used over a certain period of time, you can use this command.


## Find Command-Line Option #3: Using -perm*

* On Directories:

      $ find technical -perm 755
      technical
      technical/911report
        technical/biomed
        technical/government
        technical/government/About_LSC
        technical/government/Alcohol_Problems
        technical/government/Env_Prot_Agen
        technical/government/Gen_Account_Office
        technical/government/Media
        technical/government/Post_Rate_Comm
        technical/plos

  * On Files:
 
        $ find technical/911report -perm 774
        // No result

* The `-perm` command locates and prints any directories or files whose octal permission bits are a certain value.
* For example, `-perm 755` means that the user can do anything with the directory, which includes reading, writing, and executing the files.
* `perm-774` is to change the file permissions to the default for reading, writing, and executing for all the users.
* This is useful because if you want to see how much access and power you have over the files, then `-perm` will tell you.


## Find Command-Line Option #4: -size*

* On Directories:

      $ find technical -size -1G -type d
        technical
        technical/911report
        technical/biomed
        technical/government
        technical/government/About_LSC
        technical/government/Alcohol_Problems
        technical/government/Env_Prot_Agen
        technical/government/Gen_Account_Office
        technical/government/Media
        technical/government/Post_Rate_Comm
        technical/plos

* On Files:

        $ find technical/government -size +1G -type f
          // No result

* The `-size` command locates and prints a list of directories or files (depending on the type) based on the value after that.
* In this example, I located all of the directories that are less than 1 gigabyte and all of the files in the government subdirectory that are greater than 1 gigabyte.
* If I also did `-size -1G` like I did for directories, it would've printed me a long list of files in the government subdirectory that are smaller than 1 gigabyte.
* This is useful because if you want to know which files are taking a large part of your storage, then `-size` will tell you if you open that directory onto a coding platform.


___

*Website Used for Lab Report #3:*
https://www.computerhope.com/unix/ufind.htm#examples
