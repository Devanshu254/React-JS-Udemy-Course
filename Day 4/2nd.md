# Using Functions as values.
> You can pass functions as values to other functions. For eg: we could set a timer with the help of built in setTimeout function. A function that is provided by the browser. <br>
> SetTimeOut function accepts two input parameters. First -> Function itself.

```
function handleTimeOut() {
    console.log("Timed Out");
}
const handleTimeOut2 = () => {
    console.log("Timed Out Again");
};

// We can pass both the above created functions as a parameters to the setTimeOut function.

setTimeOut(handleTimeOut, 2000); 
setTimeOut(handleTimeOut2, 3000);
setTimeOut(()=>{
    console.log("More Timings...");
}, 4000);
```
> Above mension method is not only valid for the built in function. But we can also create our own functions and pass them as parameter to other functions.
```
function greeter(greetFn) {
    greetFn();
}
greeter(()=>{console.log("Hi")}); // This function which is an arrow function here is passed as a value to greetFn and then greetFn is executed here.
```
<img src="./images/Screenshot 2024-06-30 130118.png" alt="alt text" width="400" height="200">

# Defining functions within functions.
### Important topic in context of React.
> We can define greet within the function but not outside the function.
```
function init() {
    const message = "...";
    function greet() {
        console.log("Hi");
    }
    greet();
}
init(); 
```