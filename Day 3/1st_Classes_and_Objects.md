# Classes and Objects.

### Suppose we have two values.
```
const userName = "Max";
const userAge = 34;
```
## We can group these within an object.
```
const user = {
    name: 'Max',
    age: 34
};
console.log(user); // Whole objecte will get outputed.
console.log(user.name);
console.log(user.age);
```
We can also Define functions within our Object which we call as methods.
Example 1:
```
const user = {
    name: 'Max',
    age: 34,
    greet() {
        console.log('Hello');
        console.log(this.age);
    }
};
console.log(user.name);
user.greet();
```
Or We can create blueprint by creating class keywords.
```
class User {
    constructor(name, age) {
        this.name = name;
        this.age = age;
    }
    greet() {
        console.log("Hello");
    }
}
const user1 = new User("Manuel", 34);
console.log(user1);
user1.greet();
```