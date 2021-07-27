### What Is an Object?
- Objects are key to understanding object-oriented technology.

- examples of real-world objects: your dog, your desk, your television set, your bicycle.

- Software objects are conceptually similar to real-world objects: they too consist of state and related behavior. Identifying the state and behavior for real-world objects is a great way to begin thinking in terms of object-oriented programming.

- An object stores its state in fields and exposes its behavior through methods . 

- Methods operate on an object's internal state and serve as the primary mechanism for object-to-object communication.

### What Is a Class? 
- A class is the blueprint from which individual objects are created.

- Here's a BicycleDemo class that creates two separate Bicycle objects and invokes their methods:

`class BicycleDemo {`
    `public static void main(String[] args) {`

       // Create two different
        // Bicycle objects
        Bicycle bike1 = new Bicycle();
        Bicycle bike2 = new Bicycle();

        // Invoke methods on 
        // those objects
        bike1.changeCadence(50);
        bike1.speedUp(10);
        bike1.changeGear(2);
        bike1.printStates();

        bike2.changeCadence(50);
        bike2.speedUp(10);
        bike2.changeGear(2);
        bike2.changeCadence(40);
        bike2.speedUp(10);
        bike2.changeGear(3);
        bike2.printStates();
   ` }`
`}`

**How do Decimal Numbers work?**
- Every digit in a decimal number has a "position", and the decimal point helps us to know which position is which:
![Decimal](https://www.mathsisfun.com/numbers/images/decimal.svg)

- The Decimal Number System is also called "Base 10", because it is based on the number 10, with these 10 symbols.

**Binary Numbers**
- Are just "Base 2" instead of "Base 10". So you start counting at 0, then 1, then you run out of digits ... so you start back at 0 again, but increase the number on the left by 1.


**Hexadecimal numbers**
- There are 16 of them. They look the same as the decimal numbers up to 9, but then there are the letters ("A',"B","C","D","E","F") in place of the decimal numbers 10 to 15.

### Resources
- https://docs.oracle.com/javase/tutorial/java/concepts/
- https://docs.oracle.com/javase/tutorial/java/javaOO/classes.html
- https://www.mathsisfun.com/binary-decimal-hexadecimal.html