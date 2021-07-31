### What Is a Class?
> A **class** is a blueprint or prototype from which *objects* are created.
- For the classes : Each class is allowed to have one direct superclass, and each superclass has the potential for an unlimited number of subclasses. You can create a subclass by: At the beginning of the class declaration, use the extends keyword, followed by the name of the class to inherit from.

### What Is an Object?
> An object is a software bundle of related state and behavior.

### What Is Inheritance?
> It is a mechanism in which one object acquires all the properties and behaviors of a parent object.
- Different kinds of objects often have a certain amount in common with each other.
![Inheritance](https://javatutorial.net/wp-content/uploads/2017/10/java-polymorphism-example.png)

- A subclass inherits all the members (fields, methods, and nested classes) from its superclass. But it can not inherite the constructors, you can invoke the constructors in the subclass.


### What Is an Interface?
> An **interface** is a completely *"abstract class"* that is used to group related methods with empty bodies. It can contain only constants, method signatures, default methods, static methods, and nested types.
- Ex:
`interface Animal {`
  `public void animalSound();` // interface method (does not have a body)
  `public void run();` // interface method (does not have a body)
`}`

> * **Why do we need interfaces?**
> The ability to perform the same operation on a number of different objects. If different objects all implement the same interface and have the same method, you can store all of those objects in a Vector, for example, and iterate through the Vector calling that method on each one.

### What Is a Package?
> - A package is a namespace for organizing **classes and interfaces** in a logical manner. Placing the code into packages makes large software projects easier to manage.
> - Conceptually you can think of packages as being similar to different folders.

### Resources
- https://docs.oracle.com/javase/tutorial/java/concepts/
- https://docs.oracle.com/javase/tutorial/java/IandI/index.html


