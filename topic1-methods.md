
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

> **Exercise:**

> **Exercise:** What is wrong with this code?

# 2. Define a method / Structure of a method (modifier, argument(s), return value)

#### Lecture) 

![example](https://github.com/lukesterlee/review-session/blob/master/methods/structureOfMethods.JPG)

Declaring/defining(making,creating) VS Calling(using)

p:108~111

#### Example)

> **Exercise:** Write a static method named `min` which takes TWO integer numbers as arguments and returns the smaller one. 

> **Exercise:** Change code example 1.1 to a method which takes TWO integer numbers as arguments and returns the sum of between two numbers.

> **Exercise:** What is wrong with this code?

# 3. Calliing a method (call stack) (execution flow of a method and main)

#### Lecture)  

![Calling](https://github.com/lukesterlee/review-session/blob/master/methods/calling.JPG)

ex) checkCity, person class example
max, sum

![](https://github.com/lukesterlee/review-session/blob/master/methods/callstack.JPG)

#### Example)

> **Exercise:** What is wrong with this code?

# 4. Return types : void and others (what do I do with the return value?)

#### Lecture) 

difference between void print and return value

#### Example)

```java

```

> **Exercise:** What is wrong with this code?


# 5. pass by value VS pass by reference

#### Lecture) 

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

swap
increment

> **Exercise:** What is wrong with this code?

change the code so it does something.


# 6. The scope of variables

#### Lecture) 

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopeforloop.JPG)

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopecomparison.JPG)

#### Example)

> **Exercise:** What is wrong with this code?

# 7. Modularizing

#### Lecture) 

The whole point of using methods is **`reducing redundant`** and **`code reuse`**.

Modularizing code also makes your main clean and more readible and logic becomes clear



#### Example)

[drawRocket](https://github.com/lukesterlee/accesscode/blob/master/AC_20150312/src/nyc/c4q/lukesterlee/DrawRocket.java)

calendar

> **Exercise:** What is wrong with this code?

# 8. Final

#### Example)

one big example 

> **Exercise:** do the same


> **Exercise:** What is wrong with this code?
