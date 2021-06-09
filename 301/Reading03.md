- 1. What does .map() return?  it returns a new array with the same length of the orignal one.

- 2. If I want to loop through an array and display each value in JSX, how do I do that in React? JSX allows embedding any expression in curly braces so we could inline the map() result

- 3. Each list item needs a unique __Key__.

- 4. What is the purpose of a key? Keys help React identify which items have changed, are added, or are removed


- 1. What is the spread operator? It refers to the use of an ellipsis of three dots (…) to expand an iterable object into the list of arguments.

- 2. List 4 things that the spread operator can do. 
***Copying an array***
***Adding an item to a list***
***Adding to state in React***
***Combining objects***

- 3. Give an example of using the spread operator to combine two arrays.

`const hello = {hello: "😋😛😝"}`
`const world = {world: "🙂🙃😇🥰😍🤩!"}`

`const helloWorld = {...hello,...world}`
`console.log(helloWorld) // Object { hello: "😋😛😝", world: "🙂🙃😇🥰😍🤩!" }`

- 4. Give an example of using the spread operator to add a new item to an array.

`const fewFruit = ['🍏','🍊','🍌']`
`const fewMoreFruit = ['🍉', '🍍', ...fewFruit]`
`console.log(fewMoreFruit) //  Array(5) [ "🍉", "🍍", "🍏", "🍊", "🍌" ]`

- 5. Give an example of using the spread operator to combine two objects into one.
`const objectOne = {hello: "🤪"}`
`const objectTwo = {world: "🐻"}`
`const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}`
`console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }`

* 1. In the video, what is the first step that the developer does to pass functions between components? change the value of state in the parent, by creating a function in the same level.

* 2. In your own words, what does the increment function do? pass in the parent states and update the values.

* 3. How can you pass a method from a parent component into a child component? by using props

* 4. How does the child component invoke a method that was passed to it from a parent component? this.props.(the name of the function)