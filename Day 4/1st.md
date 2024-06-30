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
