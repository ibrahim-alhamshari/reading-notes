**How would you break a mock into a component heirarchy?**
- The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names.

**What is the `single responsibility principle` and how does it apply to components?**
- It's a technique that means, every module, class or function should have responsibility over a single part of that program's functionality, and it should encapsulate that part

**What does it mean to build a *‘static’* version of your application?**
- It's a way to implement your app ,  to build a version that takes your data model and renders the UI but has no interactivity.

**Once you have a static application, what do you need to add?**
- you’ll want to build components that reuse other components and pass data using props.

**What are the three questions you can ask to determine if something is state?**
- 1-Is it passed in from a parent via props? 
- 2-Does it remain unchanged over time?
- 3-Can you compute it based on any other state or props in your component? 

**How can you identify where state needs to live?**
- It should be owned to a component above all the components that need the state in the hierarchy.