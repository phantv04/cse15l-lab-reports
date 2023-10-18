# CSE 15L Lab Report #1: Thoai Phan

___

*Using cd:*
1. No arguments
  
![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/335313c2-f5f7-4fb6-ab20-2991abd1fb12)
* There are no errors in the output because we did not state an argument for the command. Therefore, the reason why there is no output for this command is because `cd"` will return to the user's home directory since we did not explicitly state a specific directory. When the command was in run, the working directory was `/home`. 

2. Path to a directory
  
![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/bb609b83-018b-4a04-af08-e3b65cd1a7ca)

* There are no errors in the output because in the command line, we explicitly switched the current working directory to the given path. The reason for the results is that we have officially changed the directory, which is illustrated on the left side of the bottom line.  When the command was in run, the working directory is `/home/lecture1`. 

3. Path to a file

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/f3ea6f05-e585-4fb5-9920-9ed7ca77a563)

* There is an error in the output because once you have established your current working directory, this command will be expected to change the current directory, suggesting that `cd` should include a directory path as an argument. Therefore, the reason for the output is because using a path to a file as an argument will not allow you to move between directories, which causes an error. 

___

*Using ls:*
1. No arguments
  
![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/4b19ba38-866f-4d6b-8d24-2d0e65936f39)

* There are no errors in the output because we did not state an argument for `ls`. The output is lecture1 for this command is because normally, it shows the name of the folders and files inside the current working directory. The current working directory is `/home`.
  
2. Path to a directory
  
![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/c52aecef-003e-49f7-af6b-c4166b7ae580)

* There are no errors in the output because in the command line, we stated the path to a directory using the `ls` command. The reason for the results is that `ls` lists the names of all the files and folders in the current working directory, and not the contents from other directories, which currently exists when we declared it to be lecture1.  Therefore, the current working directory is still `/home`. 
  
3. Path to a file
  
![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/f032cdd3-13d1-4445-a533-962399a5b44a)

* An error does not exist in the output because we clearly stated not just the current working directory, but also the file that we are trying to direct the path to. The reason for the output is because we listed the directory, folder, and file in the `ls` command, which basically lists specific information about the file that is at the end of the command. The current working directory in this case is also `/home`. Furthermore, you can also receive the output when you use the `ls` command with only a file name because it will assume to the default directory.

___

*Using cat:*
1. No arguments

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/d70c250e-62b7-403f-8bda-b2adc9f8dc96)


* Although there is no explicit error, the command does not print anything at first. However when you type something after cat, it will print whatever you inputted. For example, when I typed "The Voice," it printed "The Voice." You can exit out of this stage by holding Ctrl + Z. As usual, `/home` is the current directory because we have not made any changes yet, so it assumes to the default one.

2. Path to a directory

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/d88e4c47-5005-4c3d-9e96-66cea3f0d6d9)

* One can argue that there is an error with this command. This is because unlike `ls`, the `cat` command expects a file as an argument, not a directory. Although it is not obvious that there is an error message, the `cat` command will struggle to read the command without a file as a path. The current working directory is `/home` with the `pwd` command because we did not make any changes to it.

3. Path to a file

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/0418bc54-1780-49b9-9ea5-7d14c71b1a3a)

* There are no errors in this command because the `cat` command printed the content of the file. The reason for the result is that since we stated the working directory, folder, and file, or all of the components for a file that we are trying to print the content of, it will print the information inside the file, which is !Hola Mundo! in this case. Additionally, you do not need to state the folder; you can just use the command `cat lecture1/es-mx.txt` to print the same thing.
