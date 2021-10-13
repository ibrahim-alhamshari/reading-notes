## 1. Compiler vs. Interpreter
- Compliers and interpreters are programs that help convert the high level language (Source Code) into machine codes to be understood by the computers.

>  A high level language is one that can be understood by humans(human-readable code)

- A preprocessor: is a program that works on the source before the compilation. As the name implies, the preprocessor prepares the source code for compilation.

- Java, being a platform-independent programming language, doesn’t work on the one-step compilation. Instead, it involves a two-step execution, first through an OS-independent compiler; and second, in a virtual machine (JVM) which is custom-built for every operating system.

![Compilation process](https://sp-ao.shortpixel.ai/client/to_avif,q_glossy,ret_img,w_839/https://simplesnippets.tech/wp-content/uploads/2018/03/java-execution-flow-diagram.png)

**Steps**

- Compile time [ Java code(abc.java) ==> complier ==> Bytecode(abc.class) ] ===> Run time(JVM && OS)
- Run time [Class loader(Linker, ) ==> Interpreter ==> machine code ]

1. When we click run, this will invoke the Java Compiler. The compiler checks the code for syntax errors and any other compile time errors and if no error is found the compiler converts the java code into an intermediate code(abc.class file) known as *`bytecode`* (vertual code). This intermediate code(bytecode) is platform independent, hence it is only understandable by the JVM and not the user or even the hardware /OS layer.

2. This is the start of the **Run Time** phase, where the bytecode is loaded into the JVM by the **class loader**(another inbuilt program inside the JVM).

>- Linking is one of the three activities performed by ClassLoaders. It includes verification, preparation, and (optionally) resolution.
>- The Java ClassLoader: is a part of the Java Runtime Environment **(JRE)** that dynamically loads Java classes into the Java Virtual Machine **(JVM)**.

1. Source code:(abc.java) Instructions in human readable (programming) language.

2. High-level code: Instructions written in a high level (programming) language. e.g., C, C++ and Java programs

3. Byte code:(abc.class) It is a code that has been compiled from source code into low-level code designed for a software interpreter. We can name it virtual code, intermediate code. Like source code, byte code is *portable* to any computer that has an environment for running it.

4. Object code:(abc.obj) is a portion of machine code not yet **linked** into a complete program (native code). It's the machine code for one particular library or module that will make up the completed product. It may also contain placeholders or offsets not found in the machine code of a completed program. The **linker** will use these placeholders and offsets to connect everything together.

5. Machine code: is binary (1's and 0's) code that can be executed directly by the CPU.

6. Executable file:(abc.exe) The product of **linking proccess**. They are **machine code** which can be directly executed by the CPU. e.g., an .exe file.


## Resources1
- [Execution-process-of-java-program](https://simplesnippets.tech/execution-process-of-java-program-in-detail-working-of-just-it-time-compiler-jit-in-detail/)
- [JVM-works](https://www.geeksforgeeks.org/jvm-works-jvm-architecture/)
- [machine-code-vs-byte-code-vs...](https://rahul-saini.medium.com/machine-code-vs-byte-code-vs-object-code-vs-source-code-vs-assembly-code-812c9780f24c)

<br>

# Data types

- byte: (1B ==> 8 bit)
- short: (2B ==> 16bit)
- int: (4B ==> 32bit)
- long: (8B ==> 64bit)
- float: (4B ==> 32bit)
- double: (8B ==> 64bit)
- char: (1B ==> 8bit)


> A final variable can only be initialized once, either via an initializer or an assignment statement. It does not need to be initialized at the point of declaration.

```
final boolean hasTwoDigits;
if (number >= 10 && number < 100) {
  hasTwoDigits = true;
}
if (number > -100 && number <= -10) {
  hasTwoDigits = true; // compile-error because the final variable might already be assigned.
}
```

```
final boolean isEven;

if (number % 2 == 0) {
  isEven = true;
}

System.out.println(isEven); // compile-error because the variable was not assigned in the else-case.
```

```
boolean isEven; // *not* final

if (number % 2 == 0) {
  isEven = true;
}

System.out.println(isEven); // Same compile-error because the non-final variable was not assigned in the else-case.
```

> **Java annotation** is a small comment we can insert before class, method or field declarations. It represents a *metadata* which can be used by java compiler and JVM.

```
@Override
@Override annotation assures that the subclass method is overriding the parent class method. If it is not so, compile time error occurs.
```

