## Packages and Import

**package = the directory which contains our .java files**


### Package declaration
The first statement, in our .java file (Java source file), must be the package declaration.
- Ex: `package illustration;`

- The statement order inside (.java file) is as the following:
1. Package statment (optional).
2. Imports (optional).
3. Class or interface definitions.

`package illustration;`

`import java.awt.*;`

`public class Drawing {`
 `   . . .`
`}`

### Imports: We can do three options:
- 1. The *JOptionPane* class is in the *swing package*, which is located in the *javax package*.
- Ex: `import javax.swing.*; ` : The wildcard character (`*`) means, all classes with that package are available to your program.

- 2. Classes can be specified explicitly by writng the name of the package.
Ex: `import javax.swing.JOptionPane;` . Make a single class visible.

- 3. We can write the class name in the code without an import.
Ex: `    public static void main(String[] args) {`
       ` javax.swing.JOptionPane.showMessageDialog(null, "Hi");`
     `   System.exit(0);`
    `}`

**Questions from the site:**
> Q: Does importing all classes in a package make my object file (.class or .jar) larger?
> No, import only tells the compiler where to look for symbols.

> Q: Is it less efficient to import all classes than only the classes I need?
> A: No. The search for names is very efficient so there is no effective difference.

> Q: I've imported java.awt.*, why do I also need java.awt.event.*?
> A: The wildcard "*" only makes the classes in this package visible, not any of the subpackages.

> Q: Why don't I need an import to use String, System, etc?
> A: All classes in the java.lang package are visible without an import.

> Q: Is the order of the imports important?
> A: No. Group them for readability.

### Looping: as performing some lines of code in an ordered until a condition is false.

**Types of loops in Java:**
1. for loop: Allow us to execute a block of code specific number of time.
2. for-each loop: loop used to iterate through elements of arrays and collections.
3. While loop: It executes a set of statements until its boolean condition returns false.
4. Do-while loop: It works like the while loop, but the difference is that it executes the statement firstly and then checks for the condition.

