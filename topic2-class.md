
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

blueprint, template, recipe, format/form of the card

#### Example)

#### Exercise)

# 2. What is object?

#### Lecture)

actual object, copy,

#### Example)

#### Exercise)

# 3. Difference between class and object

#### Lecture)

apple pie recipe VS apple pie

empty card with field

#### Example)

#### Exercise)

# 4. Constructor

#### Lecture)

in order to create instances, every time you see new

#### Example)

#### Exercise)

# 5. static? non-static? (class variables VS instance variables)

#### Lecture)

static : class variables, one copy, general, global, independent from instances

non-static : instance variables, specific,

#### Example)

#### Exercise)

# 6. this keyword

#### Lecture)

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

data encapsulation

#### Example)

#### Exercise)

# 8. primitives VS references (pass by value)

#### Lecture)

heap, stack, cup, remote control

#### Example)

#### Exercise)

What is wrong with this code?

```java
Person p1;
for (int i = 1; i < 10; i++) {
     p1 = new Person();
}
```

# 9. Final

Circle

Dog

Person

Book

TV


