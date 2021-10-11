## 1. Compiler vs. Interpreter
- Compliers and interpreters are programs that help convert the high level language (Source Code) into machine codes to be understood by the computers.

>  A high level language is one that can be understood by humans(human-readable code)

- A preprocessor: is a program that works on the source before the compilation. As the name implies, the preprocessor prepares the source code for compilation.

- Java, being a platform-independent programming language, doesn’t work on the one-step compilation. Instead, it involves a two-step execution, first through an OS-independent compiler; and second, in a virtual machine (JVM) which is custom-built for every operating system.

![Compilation process](https://sp-ao.shortpixel.ai/client/to_avif,q_glossy,ret_img,w_839/https://simplesnippets.tech/wp-content/uploads/2018/03/java-execution-flow-diagram.png)

**Steps**

- Compile time [ Java code(abc.java) ==> complier ==> Bytecode(abc.class) ] ===> Run time(JVM && OS)
- Run time [Class loader(Linker, ) ==> Interpreter ==> machine code ]

1. When we click run, this will invoke the Java Compiler. The compiler checks the code for syntax errors and any other compile time errors and if no error is found the compiler converts the java code into an intermediate code(abc.class file) known as *`bytecode`*. This intermediate code(bytecode) is platform independent, hence it is only understandable by the JVM and not the user or even the hardware /OS layer.

2. This is the start of the **Run Time** phase, where the bytecode is loaded into the JVM by the **class loader**(another inbuilt program inside the JVM).

>- Linking is one of the three activities performed by ClassLoaders. It includes verification, preparation, and (optionally) resolution.
>- The Java ClassLoader: is a part of the Java Runtime Environment **(JRE)** that dynamically loads Java classes into the Java Virtual Machine **(JVM)**. 

## Resources
- [Execution-process-of-java-program](https://simplesnippets.tech/execution-process-of-java-program-in-detail-working-of-just-it-time-compiler-jit-in-detail/)
- [JVM-works](https://www.geeksforgeeks.org/jvm-works-jvm-architecture/)
- [machine-code-vs-byte-code-vs...](https://rahul-saini.medium.com/machine-code-vs-byte-code-vs-object-code-vs-source-code-vs-assembly-code-812c9780f24c)