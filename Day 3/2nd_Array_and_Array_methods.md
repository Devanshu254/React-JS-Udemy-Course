# Arrays Can Contain any type of value numbers, string
```
const hobbies = ["Sports", "Cooking", "Reading"];
console.log(hobbies[0]);
Output: Sports
```
> Push method.
```
hobbies.push("Working");
console.log(hobbies); // 4 Elements will be outputted.
```
> findIndex method.
```
hobbies.findIndex((item) => {
    return item === 'Sports';
})
// We can also store this index within a variable and then console.log it.
const index = hobbies.findIndex((item) => {
    return item === 'Sports';
});
console.log(index);
```
