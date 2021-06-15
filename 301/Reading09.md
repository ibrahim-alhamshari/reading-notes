## From the website

### 1- What is functional programming?
- Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.

### 2- What is a pure function and how do we know if something is a pure function?
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects


### 3- What are the benefits of a pure function?
- The code’s definitely easier to test. We don’t need to mock anything

### 4- What is immutability?
- Unchanging over time or unable to be changed. When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.

### 5- What is Referential transparency?
- This pure function will always have the same output, given the same input.
- `pure functions + immutable data = referential transparency`

## From the video

### 1- What is a module?
- **something that makes the file connected with another file (b) to allow a new folder to have access to the file (a) contant.**

### 2- What does the word ‘require’ do?
- **is used to load JavaScript modules in another file.**

### 3- How do we bring another module into the file the we are working in?
- ** using require(the mpdule path)**

### 4- What do we have to do to make a module available? 
- get access to module features is export it by the export statement `module.export`.

### Resources:
- *https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa*

- *https://www.youtube.com/watch?v=xHLd36QoS4k*