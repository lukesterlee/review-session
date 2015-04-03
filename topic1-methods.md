
# Topic 1. Methods - Overview

- What is methods?
- Define a method / Structure of a method (modifier, argument(s), return value)
- Calliing a method (call stack) (execution flow of a method and main)
- Return types : void and others (what do I do with the return value?)
- pass by value VS pass by reference
- The scope of variables
- Modularizing
- General design : top down design and implementation


# 1. What is methods?

#### Lecture) 

// white board explanation part

Methods are like `Magic Box`.

re-use, blocks

You don't have to exactly know how it works

what you need to know is what you should give (arguments) and what you are going to get (return value)

#### Example)

> **code example 1.1**

```java
public static void main(String[] args) {
    int sum = 0;
    for (int i = 1; i <= 10; i++)
        sum += i;
    System.out.println("Sum from 1 to 10 is " + sum);
    
    sum = 0;
    for (int i = 20; i <= 30; i++)
        sum += i;
    System.out.println("Sum from 20 to 30 is " + sum);
    
    sum = 0;
    for (int i = 35; i <= 45; i++)
        sum += i;
    System.out.println("Sum from 35 to 45 is " + sum);
}
```


# 2. Define a method / Structure of a method (modifier, argument(s), return value)

#### Lecture) 

// white board explanation part

![example](https://github.com/lukesterlee/review-session/blob/master/methods/structureOfMethods.JPG)

Declaring/defining(making,creating) VS Calling(using)

p:108~111

#### Example)


# 3. Calliing a method (call stack) (execution flow of a method and main)

#### Lecture)  

// white board explanation part

![Calling](https://github.com/lukesterlee/review-session/blob/master/methods/calling.JPG)

ex) checkCity, person class example
max, sum

![](https://github.com/lukesterlee/review-session/blob/master/methods/callstack.JPG)

#### Example)

What is wrong with this code?

```java
public static void main(String[] args) {
    int a = 3;
    int b = 7;
    System.out.println(sum(a,b));
}
public static void sum(int x, int y) {
    int sum = x + y;
    System.out.println(sum);
}
```

# 4. Return types : void and others (what do I do with the return value?)

#### Lecture) 

// white board explanation part

difference between void print and return value

#### Example)

```java
public class TestVoidMethod {
    public static void main(String[] args) {
        System.out.print("The grade is ");
        printGrade(78.5);
        
        System.out.print("The grade is ");
        printGrade(59.5);
    }
    
    public static void printGrade(double score) {
        if (score >= 90.0)
            System.out.println('A');
        else if (score >= 80.0)
            System.out.println('B');
        else if (score >= 70.0)
            System.out.println('C');
        else if (score >= 60.0)
            System.out.println('D');
        else
            System.out.println('F');
    }        
}            
```

> **Exercise:** What is the expected output?

> **Exercise:** Change this program to return type method.

# 5. pass by value VS pass by reference

#### Lecture) 

// white board explanation part

Java is **ALWAYS** pass by **VALUE!**

#### Example)

```java
public static void main(String[] args) {
    int a = 10;
    int b = 20;
    doSomething(a, b);
    System.out.println(a + " " + b);
}
public static void doSomething(int x, int y) {
    x = 100;
    y = 200;
}
```

swap example

> **Exercise:** What is the expected output?

```java
public class Increment {
    public static void main(String[] args) {
        int x = 1;
        System.out.println("Before the call, x is " + x);
        increment(x);
        System.out.println("after the call, x is " + x);
    }

    public static void increment(int n) {
        n++;
        System.out.println("n inside the method is " + n);
    }
}
```

> **Exercise:** Change this code to do something!

# 6. The scope of variables

#### Lecture) 

// white board explanation part

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopeforloop.JPG)

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopecomparison.JPG)

#### Example)



# 7. Modularizing

#### Lecture) 

// white board explanation part

The whole point of using methods is **`reducing redundant`** and **`code reuse`**.

Modularizing code also makes your main clean and more readible and logic becomes clear



#### Example)

[drawRocket](https://github.com/lukesterlee/accesscode/blob/master/AC_20150312/src/nyc/c4q/lukesterlee/DrawRocket.java)

calendar


# 8. Final

#### Example)

one big example 

> **Exercise:** do the same

#### Exercise 1)

Write a method named `cube` which takes an integer value as an argument and returns the cube of that integer. Then, call it in main.

#### Exercise 2)

Sum of the digits of a number.

number = 245, sum of digits = 11

Change this code into something modular. Write a method called `sumOfDigits` and use it in main method.


```java
public static void main(String[] args) {
    Scanner input = new Scanner(System.in);
    int n;
    System.out.print("Enter a positive integer: ");
    n = input.nextInt(); // 245
    
    int sum = 0;
    while (n > 0) {
        sum += n%10;
        n = n/10;
    }
    
    System.out.println("The digit sum is: " + sum);
}
```

Output will be :

```java
Enter a positive integer: 245
The digit sum is: 11
```

#### Exercise 3)

Write a static method named `min` which takes TWO integer numbers as arguments and returns the smaller one. 

#### Exercise 4) 

Change code example 1.1 to a method which takes TWO integer numbers as arguments and returns the sum of between two numbers.
