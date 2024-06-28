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
> Map method: Map allows us to transform every item in an array to another item. It takes an arrow function as an argument. It will receive every item array in the input as findIndex method. Map will not edit the orignal array instead that array. Map will return a new array. 
```
const editedHobbies = hobbies.map((items) => items + "!");
console.log(editedHobbies); // Output will give an object. 

// Instead of converting strings into strings we can also convert them to javascript objects. 

const editedHobbies = hobbies.map((items) => ({text: item}));
Output:
```
![alt text](<Screenshot 2024-06-28 170146.png>)