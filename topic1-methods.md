
# Topic 1. Methods - Overview

- What is methods?
- Structure of a method (modifier, argument(s), return value)
- Defining a method
- Calliing a method (call stack) (execution flow of a method and main)
- Return types : void and others (what do I do with the return value?)
- pass by value VS pass by reference
- The scope of variables
- Modularizing
- General design : top down design and implementation


# 1. What is methods?

#### Lecture) 

magic box, re-use, blocks

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

# 2. Structure of a method (modifier, argument(s), return value)

#### Lecture) 

![example](https://github.com/lukesterlee/review-session/blob/master/methods/structureOfMethods.JPG)

p:108~111

#### Example)

> **Exercise:** 

# 3. Defining a method

#### Lecture) 

Declaring/defining(making,creating) VS Calling(using)

#### Example)

> **Exercise:** Write a static method named `min` which takes TWO integer numbers as arguments and returns the smaller one. 

> **Exercise:** Change code example 1.1 to a method which takes TWO integer numbers as arguments and returns the sum of between two numbers.

# 4. Calliing a method (call stack) (execution flow of a method and main)

#### Lecture)  

![Calling](https://github.com/lukesterlee/review-session/blob/master/methods/calling.JPG)

ex) checkCity, person class example
max, sum

![](https://github.com/lukesterlee/review-session/blob/master/methods/callstack.JPG)

#### Example)

> **Exercise:**

# 5. Return types : void and others (what do I do with the return value?)

#### Lecture) 

difference between void print and return value

#### Example)

> **Exercise:**


# 6. pass by value VS pass by reference

#### Lecture) 

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

> **Exercise:**

change the code so it does something.


# 7. The scope of variables

#### Lecture) 

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopeforloop.JPG)

![](https://github.com/lukesterlee/review-session/blob/master/methods/scopecomparison.JPG)

#### Example)

> **Exercise:**

# 8. Modularizing

#### Lecture) 

#### Example)

drawRocket

calendar

> **Exercise:**

# 9. General design : top down design and implementation

#### Lecture) 




#### Example)

#### Exercise)


ex) what is wrong with following examples?
