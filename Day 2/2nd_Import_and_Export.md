# Import and Export within JavaScript and React.

## There are particularly three ways to include something from one file to another.

## Way 1.
```
util.js file.

export let apiKey = 'alsdjflkjaidj'; // we can use single quotation or double quotation doesn't matter.
```
```
app.js file.

import {apiKey} from './util.js';
// When working with JavaScript alone we do need to write the extension like we have writtern .js but when working with react.js the .js extension is omitted.
```