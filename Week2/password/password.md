
## Password 

### Learning Goals 
1. Practice iterating through a string
2. Practice using the ```ctype``` library
3. Practice using Boolean variables


### Background
<a href="https://www.youtube.com/watch?v=B-NhD15ocwA&t=1s" target=_blank><img src = "spaceballs.png"> </a>

As we all know by now, it’s important to use passwords that are not easy to guess! Many web apps now requre passwords that requre not only alphabetical characters, but also number and symbols.

In this lab, the user is prompted for a password, which will then be validated using a function ```check```
that you will complete. If the password contains at least one upper case letter, one lower case letter, 
a number and a symbol (meaning a printable character that’s not a letter or number, such as ‘!’, ‘$’ and ‘#’ 
the function should return ```true```. If not it should return ```false```.

### Demo 
<img src="passwordDemo.gif"> 

### Getting Started 
1. Log into code.cs50.io using your GitHub account.
2. Click inside the terminal window and execute ```cd```.
3. At the ```$``` prompt, type ```mkdir password```
4. Now execute ```cd password```
5. Then copy and paste ```wget https://cdn.cs50.net/2022/fall/labs/2/password.c``` into your terminal to download this lab’s distribution code.
6. You are to complete the function, check, which returns true if the password passes all criteria, and false if it does not.

### Implementation Details
Your function will iterate through the password that’s supplied to it as an argument. 
Since you have to find at least one lower case letter, one upper case letter, one 
number and one symbol, you may want to create a boolean variable for each and 
set each to ```false``` before you iterate through the string. If you then find a number, 
for instance you can set that boolean to true. If all booleans are ```true``` at the end of 
the function, it means all criteria are met, and you would return ```true```.

### Thought Question 
- How many different passwords do you think can be made that are 8 letters long, can use any of 95 printable ASCII characters?

### How to Test Your Code 
Your program should behave per the examples below. 

```
password/ $ ./password
Enter your password: hello
Your password needs at least one uppercase letter, lowercase letter, number and symbol!
```

```
password/ $ ./password
Enter your password: h3ll(
Your password needs at least one uppercase letter, lowercase letter, number and symbol!
```

```
password/ $ ./password
Enter your password: h3LL0!
Your password is valid!
```

You can check your code using check50, a program that CS50 will use to 
test your code when you submit, by typing in the following at the ```$``` prompt. 
But be sure to test it yourself as well!

```check50 cs50/labs/2022/fall/password```

To evaluate that the style of your code, type in the following at the $ prompt.
```To evaluate that the style of your code, type in the following at the $ prompt.```


