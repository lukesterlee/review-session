
# Topic 2. Class - Overview

- What is class?
- What is object?
- Difference between class and object
- Constructor
- static? non-static? (class variables VS instance variables)
- this keyword
- public? private? and getter and setter
- primitives VS references (pass by value)


# 1. What is class?

#### Lecture)

// white board explanation part

blueprint, template, recipe, format/form of the card

Definition from Oracle : 

Definition from somwhere : 

#### Example)

Anything with Capital letters is Class.

Class has TWO things : data members + class methods

String class, Scanner Class, ArrayList Class, Person Class

#### Exercise)

# 2. What is object?

#### Lecture)

// white board explanation part

actual object, copy,

Definition from Oracle : 

Definition from somwhere : 

#### Example)

#### Exercise)

# 3. Difference between class and object

#### Lecture)

// white board explanation part

analogies : apple pie recipe VS apple pie

empty card with field

#### Example)

#### Exercise)

# 4. Constructor

#### Lecture)

// white board explanation part

in order to create instances, every time you see new

#### Example)

#### Exercise)

# 5. static? non-static? (class variables VS instance variables)

#### Lecture)

// white board explanation part

static : class variables, one copy, general, global, independent from instances

non-static : instance variables, specific,

#### Example)

```java

```
instance variables : age, 
static : number of legs of dogs
static : number of dogs, people


#### Exercise)

# 6. this keyword

#### Lecture)

// white board explanation part

why are we using this keyword? constructor with this keyword

#### Example)

```java
public class Person {

     private String name;
     private int age;
     
     public Person(String name) {
          this.name = name;
          age = 0;
     }
}
```

#### Exercise)

why we don't use `this.age` while we use `this.name`?

# 7. public? private? and getter and setter

#### Lecture)

// white board explanation part

data encapsulation

#### Example)

#### Exercise)

# 8. primitives VS references (pass by value)
# THIS IS THE MOST IMPORTANT PART!!!

#### Lecture)

// white board explanation part

heap, stack, cup, remote control

#### Example)

```java

public static void main(String[] args) {
     int a = 3;
     int b = 7;
     hello(a, b);
}
public static void hello(int x, int y) {
     System.out.println("I'm just an example!");
}
```

```java

public static void main(String[] args) {
     Person p1 = new Person("Luke");
     Person p2 = new Person("Will");
     hello(p1, p2);
}
public static void hello(Person mimi, Person bobo) {
     System.out.println("I'm just an example!");
}
```

```java
public static void main(String[] args) {
     Person p1 = new Person("Dan Stevens");
     Person p2 = new Person("Zac Efron");
     
     Person p2 = new Person("Luke Lee");
     Person p3 = p2;
}
```



> **Exercise:** What is wrong with this code?

```java
Person p1;
for (int i = 1; i < 10; i++) {
     p1 = new Person();
}
```

> **Exercise:** Now we fully understand why we can't use `==` for String class. Explain to me! 

# 9. Final

> **Final Exercise:** Implements a Circle class

> underline : static

> \+ : public

> \- : private

![](https://github.com/lukesterlee/review-session/blob/master/class/circle.JPG)


Dog

Person

Book

TV


