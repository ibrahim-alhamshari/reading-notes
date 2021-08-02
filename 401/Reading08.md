### SOLID is an acronym for the first five object-oriented design (OOD) principles.

**SOLID stands for:**
- S - Single-responsiblity Principle
- O - Open-closed Principle
- L - Liskov Substitution Principle
- I - Interface Segregation Principle
- D - Dependency Inversion Principle

> Single-responsibility Principle (SRP) states: A class should have one and only one reason to change, meaning that a class should have only one job.



> Open-closed Principle (OCP) states: Objects or entities should be open for extension but closed for modification. This means that a class should be extendable without modifying the class itself.
**Ex: phones have app stores and via the app store, you can extend the phone's capabilities to allow you to manage your to-do list. the mechanism that allows you to do this is purely one of extension. so phone functionality is closed for modification and they open it to an extension.**


> Liskov Substitution Principle states: This means that every subclass or derived class should be substitutable for their base or parent class.

> Interface segregation principle states: A client should never be forced to implement an interface that it doesn’t use, or clients shouldn’t be forced to depend on methods they do not use.

>Dependency inversion principle states: Entities must depend on abstractions, not on concretions. It states that the high-level module must not depend on the low-level module, but they should depend on abstractions.
**Ex: if you want to pay for something with a credit card; the clerk seeing that your card is a visa. he just takes your card, whatever it is, and swipes it. both you and the clerk depend on the credit card abstraction without worrying about specifics.**

### Resources
- https://scotch.io/bar-talk/s-o-l-i-d-the-first-five-principles-of-object-oriented-design
- https://dzone.com/articles/the-solid-principles-in-real-life