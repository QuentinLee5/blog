---
layout: post
title:  "Crash course Java"
date:   2014-09-10 20:45:35
categories: 
---

## Crash course Java

In this blog post I’m not really going to talk about a certain topic, but I’m going to give a crash course about the programming language Java. As you know I’m a computer science student and I noticed that students without any programming experience are struggling for days with simple Java exercises they get in the first weeks of college. To help those students I’m going give a crash course in Java so new computer science students can have a little experience before going to college.

In this post I’m going to talk about the programming concepts I think are most important to know before going to college. So I’m going to talk about:

* Data types and variables
* Operations
* Conditions
* Iterations
* Methods

So let’s start with data types and variables. In Java you have lot’s of different data types. The most important are:

* Integers (-3, -2, -1, 0, 1, 2, 3, ...)
* Floats and doubles (floating point numbers like 3.4935)
* Strings (this could contain text, like “this is a String”)
* Booleans (can have 2 values: true of false)

In Java you can declare variables. This means that you can assign a value of a data type to a variable. You declare variables like this:

```
int x = 5;
```

When the Java Compiler runs this code, the variable x will have a value of 5. As you can see when declaring a new variable you have to specify its data type by writing the data type before the variable name. If the variable already exists this is not needed.

```
int x = 5;
x = 3;
```

The code above will assign 5 to x in the first statement and 3 to x in the second statement. After the second statement, variable x won't have the value 5 anymore but only the value 3. To declare a String you would have to do this:

```
String y = “this is a string”;
```

Now you know about variables let’s talk about operations. Java supports lots of operations like addition (+), substraction (-), division (/) and multiplication (*). To perform such operations you can write code like this:

```
// x will contain the value 6.
int x = 2*3;

// y will contain the value 2. 
int y = x - 4;

// z will contain the value 8.
int z = y + x:
```

(As you can see, I wrote // in the code above. Using // will comment out all code on the same line after the //. This means that the commented code won't be executed by the compiler and this can be used to explain your code)

You can use variables or just values to do operations. If you want to increment an int by 1, you can just write the variableName++. So the statement x++ will increase the value of x by one. 

Before I will continue on conditions, let me first talk about some syntax. As you can see, after every statement, I put a semicolon to tell to the compiler that this is the end of an statement. This is something must do. Otherwise your code won’t run. 
Another thing I want to tell you is that you can write values to the console using System.out.println(). 

```
System.out.println(“hello world”)
```

will print hello world to the console. Just try it out yourself. If you put variables between the parentheses, it will print the value of those brackets. 

So now let’s talk about conditions. In Java you have if, else if and else conditions. Let's first talk about if and else:

```
if (5 > 3) {
    ...
}
else {
    ...
}
```

This example above will first check the condition between brackets. If the condition is true, the statements between the curly braces will be executed. If the condition is false, then the statements at the else statement will be executed. Another statement you can use is the else if:

```
if (5 > 3) {
    ...
}
else if (3 < 5) {
    ...
}
else {
    ...
}
```

So in this example the first condition is false so it will check for the second condition which is true so the compiler will execute the statements of the else if statement. 

The next topic I'm going to talk about is iterations. There are 2 types of iterations. You can use a for loop or a while loop. A for loop is written as follows:

```
for (int i = 0; i < 10; i++) {
    System.out.println(“hello”);
}
```

This example will print hello 10 times.
The syntax is as follows. You first initialize a variable, then you give a condition and last but not least you let the code do something after each iteration. So in this case you set an int to 0, give the condition that i should be less than 10 and you increment i by 1 after every loop.
A while loop works as follows: 

```
int x = 0
while (x < 10) {
    System.out.println(“hello”):
    x++;
}

```
After every iteration the code checks if the condition is still true and it will run the code again until the condition is false. So this time you have to make sure yourself that the condition will ever be false, otherwise the program will stuck in this loop forever. 

Last but not least I’ll talk a bit about methods. Methods can be used to group code. You can call methods, which will execute the code inside the method. This way you can prevent code duplication. This is an example of a method:

```
void methodName() {
    ...
}
```

So when you call in your code:br>
methodName();
The code inside the method will be executed.
Now you know what a method is, let’s tell you a bit more about methods. Methods can just execute code or it can execute code and return a data type. In the first case, you have to add void before the method name as you can see I did above. In the second case you have to replace void by the data type you want to return. So a function returning a data type looks like this:

```
int calculateAmount() {
    int x = ...
    ...
    return x
}
```

So in this case the value of x will be returned. A way you can use these methods is:

```
int amount = calculateAmount();
```

amount will have the value that is returned by the calculateAmount method. 

(Don’t forget: when you call return the method will be exited so all code below a return won’t be executed). 

Another important thing about methods are parameters. You can pass parameters through methods. So for example let’s say you want to calculate the square of an int. Then you can write a method like this:

```
int square(int input) {
    return input * input;
}
```

So as you can see you can put parameters between the parentheses and you have to tell which type the parameter is. You can call a method with a parameter like this:

```
int x = square(4);
```

So you can just put the value between the parentheses. Writing methods with more than 1 parameter will look like this. 

```
int multiply(int x, int y) {
    return x * y;
}
```

Calling such a method goes like this:

```
int result = multiply(3, 4);
```

So you can separate different parameters using a comma and you can add as many parameters as you want. 

This is the end of this crash course. I hope now you know more about data types, operations, conditions, loops and methods and that you are able to write small Java programs yourself. I could tell more but I think this is most important for you to know if you are completely new to programming. If you still have any questions after reading this blog post, you can add a reaction below or you can contact me on Twitter.