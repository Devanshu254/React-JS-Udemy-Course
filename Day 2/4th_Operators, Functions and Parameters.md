# Operators.
```
We have +,-,*,/ operators and also === for checking equal conditions.
+ -> Can be used for adding two or more values and also used for string.
we have >, <, and >=, =<.
```

# Functions.
### Simple Function.
```
// Code Definition.
function greet() {
    console.log("Hello");
}
// Function Call.
greet();
greet();
```
### Parameterized Functions.
```
function greetUser(userName, message) {
    console.log(userName);
    console.log(message);
}
greetUser("Max", "Hello");
greetUser("Dev", "Hii, what's up");
```
### Assigning Default Value.
```
function greeUser(userName, message = "Hello!") {
    console.log(userName);
    console.log(message);
}
greetUser("Max");
```
### Returning the Value;
```
function greeUser(userName, message = "Hello!") {
    return "Hi" + userName + "." + message;
}
greetUser("Max");
```
### Using Const Keyword Storing Values.
```
function greeUser(userName, message = "Hello!") {
    return "Hi" + userName + "." + message;
}
const greeting = greetUser("Max");
console.log(greeting);
```
