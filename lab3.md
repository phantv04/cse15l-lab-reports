# CSE 15L Lab Report #3: Thoai Phan

___

## Part 1: Bugs


Buggy Code:

    static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;

Failure-Inducing Input:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/8989935f-6ab0-48d2-b286-66c6d7364195)


Input with No Failures (Same Code):

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/eff75947-ca30-4553-98b6-9c41d8fa4c9b)


Symptom:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/b329b3f5-270c-434d-a968-e6d4b566e574)


Code Before:

    static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;


Code After:

    static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }

* Bug: It should be newArray[i] = arr[arr.length - i - 1] instead of arr[i] = newArray[arr.length - i - 1].
* Bug: We should return the newArray, not the original array.
* This fix addresses the issue because when we put newArray before the equal sign, we are saying what we will add to the newArray by calling certain elements from the original array.
* Additionally, with this change, we are returning the newArray that is being reversed instead of the original array.



___

## Part 2: Researching Commands

*Find Command-Line Option #1: Using -name*

* On Directories:

        $ find technical -name "911report"
        technical/911report

* On Files:

        $ find technical -name "commission_report.txt"
        technical/government/About_LSC/commission_report.txt

  
* Using `-name` with the `find` command will search for a file or directory that has the specific name in it.
* It is useful because if you forgot whether or not you have a certain file or directory on your computer, you can search for it. If there is no result, than that means that it does not exist.


*Find Command-Line Option #2: Using -iname*

* On Directories:

        $ find technical -iname 'BIOMED'
        technical/biomed

* On Files:

        $ find technical -iname 'JoUrNaL.pBiO.0020068.tXt'        
        technical/plos/journal.pbio.0020068.txt


* Using `-iname` with the `find` command will search for a file or directory that has the specific name in it, but will also match the letters case-insensitively.
* It is useful because if you forgot whether or not you have a certain file or directory on your computer, you can search for it. If there is no result, than that means that it does not exist.
* Additionally, if you forgot that your file started with a capital letter, this is useful because it does not matter in this case.


*Find Command-Line Option #3: Using -atime*

* On Directories:

        $ find technical -atime +1
        // No result

* On Files:

        $ find technical/biomed -atime +1
        // No result

* The command `-atime + 1` locates and prints a list of files or directories that was last accessed more than 1 day ago.
* There was no result in these commands because I used all of the files in technical from biomed, plos, etc. for my lab report.
* When I used the command `-atime -1`, which prints the files and directories used less than 1 day ago, a long list came out, whether from the directory technical or a subdirectory such as plos.


Find Command-Line Option #4:
