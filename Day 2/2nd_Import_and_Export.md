# Import and Export within JavaScript and React.

### There are particularly three to four ways to include something from one file to another.

## Way 1: Normal way.
```
util.js file.

export let apiKey = 'alsdjflkjaidj'; // we can use single quotation or double quotation doesn't matter.
```
```
app.js file.

import {apiKey} from './util.js';
console.log(apiKey);
// When working with JavaScript alone we do need to write the extension like we have writtern .js but when working with react.js the .js extension is omitted.
```
```
Note: To work with the import and export keywords within JavaScript we must have to include type keyword in JavaScript which we have learned in Day1. In React we do not need it.

<head>
    <script src="assets/scripts/app.js" type="module"></script>
</head>
```

## Way 2: Using Default Keyword.

```
util.js file.

export default "asdkfjladjsf"; 
```
```
app.js

import apiKey from "./util.js";

console.log(apiKey);

In react we have components so In one file we have one component so we export them as a default.
You can "export default" a function or variable that was created before but you can not "export default let.." in one single line.
```

## Way 3: As a JavaScript object.

```
util.js file.

export default "asdkfjladjsf"; 
export let abc = "abs";
export let acb = "acb";
```
```
import apiKey from "./util.js"; // For default;
// import { abc, acb } from ".util.js";

// Using as object.
import * as util from "./util.js";
console.log(util.abc);
console.log(util.acb); // like this.
```

## Way 4: Using alias, Extension of way 3.
```
import {apiKey, abc as content} from './util.js';
console.log(content.abc);
console.log(content.apiKey);
```
