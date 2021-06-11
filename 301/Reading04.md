## What is a ‘Controlled Component’?
* It's components maintain their own `state` and update it based on user input . When the user types into the input field, the onChange handler updates these state (by setState) with the input’s value accessed from the event object: event.target.value.


## Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.
- we update the state with the user responses as soon as they enter them because we use elements that will get the updated data directly when the user change anything in the input field (we use the Controlled Components). 

## How do we target what the user is entering if we have an event handler on an input field?
- We target the user's entering by using onChange handler , and the target will be `event.target.value.`

## Why would we use a ternary operator?
- Because it's shorter than if statement to write and easy to dael with the same functionality.

## Rewrite the following statement using a ternary statement:
`if(x===y){ console.log(true);`
  `} else {`
 `console.log(false);`
  `}`

  By ternary: `x===y ? console.log(true) : console.log(false);`

  **Resorces:**
- *1- https://react-bootstrap.github.io/components/forms/*
  *2-  https://reactjs.org/docs/conditional-rendering.html*