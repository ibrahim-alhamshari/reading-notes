
### The `transform` property applies a **2D** or **3D** transformation to an element. This property allows you to *rotate, scale, move, skew*, etc., elements.

> Examples:
> - `transform: scale(1.5);` ===> when you hover the element, the area or the volum will increase by 1.5  
> - `transform: rotate(20deg);`===> when you hover the element, it will rotate to 20 degree only.
> - `transform: scale(.5, 1.15);` ===> This will change the element's shap, where it will shrink from x-axis by 0.5 ,  and increase from y-axis by1.15 .
> - `transform: skewX(5deg);` ===> Will make an oblique to the element.
> - `transform: perspective(200px)` ===> It give the object value to far this object is away from the user.

### `transitions` allows us to change property values smoothly, over a given duration. And there are four properties related to it :`transition-property`, `transition-duration`, `transition-timing-function` and `transition-delay`.

### `animation` move the element with number of iterations in a specific way , It used mostly with `transition` to make the element more controlled. We use `@keyframes` to set multiple points at which an element should undergo a transition.

> Example :
> `.stage:hover .ball {`
 ` animation-name: slide;` // **To give the element a name.** 
  `animation-duration: 2s;` //**property defines how long an animation should take to complete one cycle.**
  `animation-timing-function: ease-in-out;` // **Specify the speed curve of an animation.**
  `animation-delay: .5s;` // **Start the animation after 0.5 second**
`}`
> `@keyframes slide {` // **Here is the animation code.**
  `0% {`
    `left: 0;`
    `top: 0;`
  `}`
  `50% {`
    `left: 244px;`
    `top: 100px;`
  `}`
  `100% {`
    `left: 488px;`
    `top: 0;`
 ` }`
`}`
