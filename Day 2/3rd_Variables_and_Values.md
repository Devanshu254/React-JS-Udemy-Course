## There are different types of Values.
1. **Strings**: Text values wrapped with single or double quotes, can also be created with backticks(`);
2. **Number**: Positive or negative. Float or Integer.
3. Boolean: True or False.
4. **Null and Undefined**: There is no value. **Undefined**: Default if no value was assigned yet.
**Null**: Explicitly assigned by developer (reset value).

## Identifiers must follow certain rules and recommendations.
**1. Must contain whitespace or special characters (except $ and _).** <br>
```
Valid: $UserName, age, user_name, data$,...
Invalid: %UserName, age/, user name...
``` 
**2. May Contain Numbers but must not start with a number.**
```
Valid: user3, us3r...
Invalid: 3user, 11player...
```
**3. Must not clash with reserved keywords.**
```
Valid: user, data, age....
Invalid: let, const, if...
```
**4. Should use CamelCasing.**
```
Recommended: userName, isCorrect,...
Uncommon: user_name, iscorrect..
```
**5. Should Describe What the "thing" it identifies contains or does.**
```
Recommended: userName, isCorrect, loadData..
UnCommon: userDataPoint, correctNess, dataLoader...
```

### Difference between Let and Const.
1. Var is globally scoped while let and const are blocked scoped.
2. Var can be update and re declared within its scope.
3. Let can be updated but not re declared.
4. Const can neither be updated nor be re declared.
5. Var variables are initialized with undefined whereas let and const variables are not initialized.
6. Const must be initialized during declaration unlike let and var.

```
var myVariable;
console.log(myVariable);
output: Undefined.

let myLetVariable;
console.log(myLetVariable);
output: Undefined.

const myConstVariable;
console.log(myConstVariable);
Output: Error.
```

