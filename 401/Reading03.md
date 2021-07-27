## Primitives vs. Objects

- autoboxing : The process of converting the primitive type to the reference type .
- unboxing : The process of converting the reference type to the primitive type.

> primitive type variables have the following impact on the memory:
- boolean – 1 bit
- byte – 8 bits
- short, char – 16 bits
- int, float – 32 bits
- long, double – 64 bits


> referance types like:
- Boolean – 128 bits
- Byte – 128 bits
- Short, Character – 128 bits
- Integer, Float – 128 bits
- Long, Double – 192 bits

* primitive types are faster in their operations generally than the reference types.

* Default values of the primitive types are `0` for numeric types, `false` for the boolean type, `\u0000` for the char type. 
* For the reference types, the default value is `null`.

* The primitive types require much less memory (because that it much faster). But the reference types use higher memory.

## Exceptions in JAVA

**What Is an Exception?**
- It is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

- The code that might throw certain exceptions must be enclosed by either of the following: 
1. The try must provide a handler for the exception.
2. A method that specifies that it can throw the exception.

- We have three exceptions: checked exception, error exception, runtime exception.
**Note: Code that fails to honor the Catch or Specify Requirement will not compile.**

**Objects of type `Scanner` are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.**

### Resources 
- https://www.baeldung.com/java-primitives-vs-objects
- https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html
- https://docs.oracle.com/javase/tutorial/essential/io/scanning.html