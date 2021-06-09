### Form controls :They are responsible to accept the User input in a specified manner. as an example : Adding text, Making choices , Submitting forms, Uploading files.

> You can add a text by these three ways , where everyone have a specific use :
* 1- Text input (single-line)
* 2- Password input
* 3- Text area (multi-line)

> How Forms Work: 
- 1- the page ask the user to enter a specific information.
- 2- After the user entering the information , these information do send to the server who check the values and return a new page according to that information .

> Form structure: 
 `<form action="http://www.example.com/subscribe.php" method="get">`
`<p>This is where the form controls will appear. </p>`
`</form>`

### The `list-style-type` property allows you to creat a list for your contents , which can be ordered list or unordered list.

> - Unordered Lists: the values can appear to you in one of these shapes: none, disc, circle, square 
`<ul><li> The text ..............</li></ul>`
> - Ordered Lists : you will get an order list . `<ol><li>The text .........</li></ol>`

### Event flow : When you put elements inside eachothers like : `<html><body><ul><li>` , and then you press on the link insid `<li>` the process will be outwards exceed the elements `<li><ul><body><html>` with this direction ,   and after that the response will be inwards exceed all the elements `<html><body><ul><li>` with the same order.