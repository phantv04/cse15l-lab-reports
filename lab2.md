# CSE 15L Lab Report #2: Thoai Phan

___

## Part 1: StringServer


Code:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/82857e12-3644-417c-8a37-7fa90b51b046)


Using `/add message` in the code sample #1:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/d337d006-79b4-4972-967a-0939c32565da)

* The method that is called for the first message is handleRequest(URI url) from the Handler class.
* A relevant argument to this method is the `URI uri` because the URI identifies the web address as it contains a path. With this information, this request will have a path of `/add message` and the information that is retrieved in this case is `s=Welcome to UC San Diego!`.
* The values of num, input, and messages are changed because they were initially null or 0. After the request is processed, `num` incremented to 1 (as shown on the left side), `input` is "Welcome to UC San Diego!", and this input is added to the `messages` list. These changes allowed "1. Welcome to UC San Diego!" to be returned.


Using `/add message` in the code sample #2:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/bf3aaff8-92d5-47c5-b789-dee50056bea2)

* The method that is called for the second message is handleRequest(URI url) from the Handler class.
* A relevant argument to this method is the `URI uri` because once again, it identifies the resource from the HTTP request and the path and query of the request will be identified. In this case, the path is still `/add-message` and the new query or information that is retrieved is "It's beginning to look a lot like Christmas!".
* The value of `num` changed from 1 to 2, `input` changed from the previous one to "It's beginning to look a lot like Christmas!", and the `messages` list will have another message appended to it. The result of the `messages` list is now "1. Welcome to UC San Diego!" and "2. It's beginning to look a lot like Christmas!" underneath it.

___

## Part 2: LS & SSH

Current files with the `/ls` command:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/df5956ad-ae15-4ddf-8fe3-7cad97d7815b)


Path to a Private Key:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/03524f46-95af-4abf-9267-64b721ef607d)


Path to a Public Key:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/c64d34d5-6353-4d8f-8a70-6a94c724b46b)

Logging in Without a Password:

![image](https://github.com/phantv04/cse15l-lab-reports/assets/146781799/bc760880-506f-4455-a8c4-c9e6c8152747)

___

## Part 3: Learning

* I have learned a lot over the past few weeks because I came to San Diego without any programming experience. Although I took a few computer science courses last year, this class feels totally different because I learned to create local servers, add sentences to empty servers, and how directories work behind the scenes. I never knew how to print the files inside a folder and switching directories for one's convenience until this course.
