# Lesson Title

## Learning Goals

- Explain a Java object
- Create objects in Java


## Java Object

In Java, an object is an instance of a class. 

Consider our `Bicycle` class from earlier: 

```java 
public class Bicycle {
    String color; 
    int height; 
    int position; 
} 
```

It describes the properties of a bicycle, but how do I actually store any information about John's actual bicycle? 

When I create an instance of this class, I am telling Java to create something for me that will comply with the structure 
described by the class. In other words, John's bicycle will have a property named `color` of type `String`, and property named 
`height` of type `int` and finally a property named `position` of type `int`. 

What I'm asking Java to create is an "object of type Bicycle". 

This is bringing several of our previous concepts together. When we create a class in Java, we create a new "type", which can 
then be assigned to a "variable": 

```java 
Bicycle johnsBike = new Bicycle(); 
```

The `new` instruction tells Java to create a new instance of the class `Bicycle` and assign it to the variable named `jonhsBike`. 
Once that variable has been defined, we can give its variables values: 

```java 
Bicycle johnsBike = new Bicycle(); 
johnsBike.color = "blue"; 
johnsBike.height = 36; 
johnsBike.position = 0;  
```

We can also create another object of type `Bicycle` to represent Claire's bike: 

```java 
Bicycle clairesBike = new Bicycle(); 
clairesBike.color = "green"; 
clairesBike.height = 42; 
clairesBike.position = 10;  
```
