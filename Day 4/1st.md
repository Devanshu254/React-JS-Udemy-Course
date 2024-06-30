# Spread Operator.
> If we have a hobbies list and we want to merge it with another hobbies list.
```
const hobbies = ["Sports", "Cooking"];
const newHobbies = ["Reading"];
```
```
// Spread operator (...).
const mergedHobbies = [...hobbies, ...newHobbies];
Output: const mergedHobbies = ["Sports", "Cooking", "Reading"];
```
```
// Below code would give array with two nested arrays.
const mergedHobbies = [hobbies, newHobbies];
console.log(mergedHobbies);
```
> We can also use spread operator on objects.
```
const user = {
    name: "Max",
    age: 34
};
const extendedUser = {
    isAdmin = true,
    ...user
}
console.log(extendedUser);

Output: An object which contains all the key value pair of user as well as extendedUser object.
{
    name: "Max",
    age: 34,
    isAdmin: true
}
```
# Revisiting Control Structures.
## If Else Statement.
```
const password = prompt("Your password");
if(password === "Hello") {
    console.log("Hello works");
}else if(password === "hello") {
    console.log("hello works");
}else {
    console.log("Access not granted");
}
```
## For loop.
> If we want to iterate over an array.
```
const hobbies = ["Sports", "Cooking"];
for(const hobby of hobbies) {
    console.log(hobby);
}
Output: 
Sports
Cooking.
```
# Dom Manipulation.
> We will not use DOM manipulation mostly because we will use react. In react Dom's are not used. 
```
// Below is something which we are not going to do mostly.
const list = document.querySelector("ul");
list.remove();
```