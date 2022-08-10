# Object

## Learning Goals

- Explain a Java object
- Create objects in Java

## Java Object

As stated before, in Java, an **object** is an _instance_ of a **class**.

To use an example from our everyday life, consider a contact in a phone. Each
contact has the same blank fields asking for a name, a phone number, and possibly
a picture as well. We can think of each contact as an object whereas the contact 
book would be a class.

Consider our `Bicycle` class from earlier:

```java
public class Bicycle {
    String color;
    int height;
} 
```

It describes the properties of a bicycle, but how do we actually store any
information about John's actual bicycle?

When we create an instance of this class, we are telling Java to create something
for us that will comply with the structure described by the class. In other
words, John's bicycle will have a property named `color`and another property
named `height`.

What we are asking Java to create is an object called `Bicycle` that has those
properties associated with it.

If we want to create John a `Bicycle` we can do so with the following snippet of
code:

```java
Bicycle johnsBike = new Bicycle(); 
```

Let's break down this bit of code!

- `Bicycle` is the **type** of object we want to create. Java is a strongly
  typed programming language. This means that every object that is defined
  must be defined with a data type. For example, the `color` property has a
  type `String` which specifies that color can be a word or a string of
  characters. We will talk more about different data types in the following
  lesson.
- `johnsBike` is the name that we are going to call the `Bicycle` object we are
  creating.
- The `new` instruction tells Java to create a new instance of the class
  `Bicycle` and assign it to `jonhsBike`.
- `Bicycle()` is the **constructor** of our `Bicycle` class. We will talk more
  about constructors later, but know that this method helps instantiate the new
  instance of the class `Bicycle`.

Once `johnsBike` has been defined, we can play with the property values in the
`Bicycle` class to be more specific to John's actual bike:

```java
Bicycle johnsBike = new Bicycle();
johnsBike.color = "blue";
johnsBike.height = 36;
```

The syntax we see above is called "dot notation" and it allows us to access the
object's properties. To further explain dot notation, consider the line
`johnsBike.color = "blue";`. We are accessing the property `color` of the object
`johnsBike` and assigning it to the word `blue`.

We can also create another object of type `Bicycle` to represent Claire's bike:

```java
Bicycle clairesBike = new Bicycle();
clairesBike.color = "green";
clairesBike.height = 42;
```
