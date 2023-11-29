# CSE 15L Lab Report #5: Thoai Phan

___

## Part 1.1: Original Post with Bug

To TA,

Hello! I hope you are doing well. I wanted to ask if you can help me with my code. I am trying to create a calculator for division, but it's giving me the wrong answer. I know that 5 / 2 = 2.5 and not 2, so I'm assuming that it's the data type declarations that are causing the wrong output to be produced.

Thank you!


Best,
Student


Code:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/785a46ba-2be6-4752-a4a2-8dc2785e7c0d)


___

## Part 1.2: TA Helping Student

Hello! Thank you for your post.

You are correct. Remember that in Java, an integer divided by an integer will give you an integer. What do you think you should change `int` to so that decimals can be accounted for in your code? Also, try editing it in Vim and see if you get the right output!


Best,
TA

___

## Part 1.3: Using the TA's Suggestions


Correct Output:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/d46cfc73-595b-4585-97ac-d645a2afafcb)

* As the TA mentioned, the bug was that in Java, any integer divided by an integer will result in an integer unless one of the numbers are a double. It is better to convert all numbers from integers to double so that an integer divided by an integer will give you the correct double.
  
* The changes made to the code is included in the next part of the lab report.

___

## Part 1.4: Information of Debugging Case

File & directory structure:
* Code with the calculator --> `Testing.java` in this case
* Bash script that runs the test --> `test.sh` in this case

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/d7e38214-aa3c-4ff0-8cca-beadfba66d7f)

Contents Before Fixing the Bug:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/785a46ba-2be6-4752-a4a2-8dc2785e7c0d)

* Used `bash test.sh` to run the code and inputted two values, which triggered the bug since int / int will result in an int value. 


Contents After Fixing the Bug:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/936565f8-53d3-4073-aa52-5671446bc987)

Using `vim Testing.java`: 

* Change every `int` to `double`
* Used `d` to delete the characters in `int`
* Insert mode by clicking on `i` and then inserted `double` before each variable.
* The correct result is illustrated in part 1.3.

___

## Part 2: Reflection

One thing that I learned in this class that I didn't know before is that you can edit code through the terminal. This was the most interesting thing to learn for me in the second half of the course because to me, it was amazing that you can use commands such as `vim` and `nano` to open an entire Java file through the terminal and you can even use edit commands such as insert mode `i` and delete mode `d` to edit the file. It was really interesting for me to practice these skills in the lab because I remember following a 30-minute tutorial/guide on Vim in a lab and it was really fun learning about the commands that you can use in the terminal to fix your Java code, rather than editing it directly. Also, learning about bash script was enjoyable for me because to me, using bash scripts to run code can be useful since the script runs all of the commands that you put in the file, which can be useful with multiple code files and commands.

___
