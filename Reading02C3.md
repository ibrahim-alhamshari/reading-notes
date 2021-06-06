**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**
- The render is first.

**What is the very first thing to happen in the lifecycle of React?**
- mounting 

**Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates?**
- 1-render 
- 2- react updates 
- 3- constrctour 
- 4- componentdidmount 
- 5- component willunmount 

**What does componentDidMount do?** 
- it used to load anything using a network request or initialize the DOm

**What types of things can you pass in the props?**
- text or disciption and anything we want to display to the user 

**What is the big difference between props and state?**
- if you handling the information inside the components you need to use ***state***, also if your information is not static (If the information going to chang).
- If you handling the information outside the components you need to pass it via ***props*** , also if your information is static (Not going to chang).
- in props you are passing into a component and in state is something handeled  inside the component, props is handeled outside the component 

**When do we re-render our application?**
- when we change the state inside our application 

**What are some examples of things that we could store in state?**
- The things that updating by the user, like : ***a counter*** ,***form*** ,***checkbox***