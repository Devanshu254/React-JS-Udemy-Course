# Destructuring.
> Related to arrays and objects there are two crucial relatively new and modern JavaScript features we should know.
> First feature is about destructing.
> Normally we handle the codes like below.
```
const userNameData = ["Max", "Maxwell"];
const firstName = userNameData[0];
const lastName = userNameData[1];
```
> But we can also write it as below.
```
const [firstName, lastName] = ["Max", "Maxwell"];
console.log(firstName); // Output: Max
console.log(lastName); // Output: Maxwell
```
> We can also destructure objects. 
> Instead of doing below.
```
const user = {
    name: "Max",
    age: 34
};
const name = user.name;
const age = user.age;
```
> We can write.
```
const {name: userName, age} = {
    name: "Max",
    age: 34
};
console.log(userName); // Output: Max
console.log(age); // Output: 34
```