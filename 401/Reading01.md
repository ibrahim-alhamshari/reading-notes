## Variables
- Java programming language have the following types of variables:
1. Instance Variables (Non-Static Fields): also known as instance variables because their values are unique to each instance of a class.
2. Class Variables (Static Fields): class variable is any field declared with the static modifier. Ex: `static int numGears = 6;`
- Ex: `final int number = 5;` the keyword final could be added to indicate that the number will never change.

3. Local Variables: Any variable declared between the opening and closing braces of a method. It will not accessible from the rest of the class.

4. Parameters: 
- Ex: `public static void main(String[] args)`. The `args` variable is the parameter to this method.
- parameters are always classified as "variables" not "fields".

## What does it mean to compile code?
- It's converting the source code or the code which written by humans(The machine didn't understand this code) to the machine code/binary code(zero-one-code). So, the machine can understand it and execute it.

## Making Sense of Java’s API Documentation
> You can find things in the API documentation in a number of different ways. Each way is convenient in one situation or another.
- Using the index
- Using the list of classes

- To create the API documentation, the captains of Java ran a program called javadoc. The javadoc program took lines like these right out of the PrintStream.java file and used the lines to make the documentation that you see in your web browser.
- When you download the JDK, you get the javadoc program.

### Resources
1. https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html
2. https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/
3. https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/