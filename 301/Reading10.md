### 1-What is a ‘call’?
- function invocation (call)


### 2- How many ‘calls’ can happen at once?
- one at a time.

### 3- What does LIFO mean? 
- it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

### 4- Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
- function firstFunction(){
  throw new Error('Stack Trace Error');
}
function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();


### 5- What causes a Stack Overflow?
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.



### 1- What is a ‘refrence error’?
- This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

### 2- What is a ‘syntax error’?
- this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.


### 3- What is a ‘range error’?
- Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.


### 4- What is a ‘tyep error’?
-  this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

### 5- What is a breakpoint?
- putting a debugger statement in your code in the line you want to break.

### 6- What does the word ‘debugger’ do in your code?
- If you add a debugger to your code it will reaching that code to a breakpoint.

### Resources:
- https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4
- https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c