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
# Destructuring in Function Parameter Lists
> The destructuring syntax explained in the previous lecture can also be used in function parameter lists.

> For example, if a function accepts a parameter that will contain an object it can be destructured to "pull out" the object properties and make them available as locally scoped variables (i.e., variables only available inside the function body).

```
function storeOrder(order) {
    localStorage.setItem('id', order.id);
    localStorage.setItem('currency', order.currency);
}
```
> Instead of accessing the items via dot notation inside storeOrder function body, you could desturcture like below.

```
function storeOrder({id, currency}) { // destructuring
  localStorage.setItem('id', id);
  localStorage.setItem('currency', currency);
}
```
> It is very important to understand that storeOrder only takes one parameter in this example. It does not accept two parameters - an object which then is just is destructured internally.
> The function call would be like.

```
storeOrder({id:5, currency: 'USD', amount: 15.99}); // One argument value.
```
