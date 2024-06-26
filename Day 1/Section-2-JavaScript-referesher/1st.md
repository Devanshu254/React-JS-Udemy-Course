# JavaScript.

### JavaScript can be executed in many environments.
* **In the browser**: JavaScript code can be included within any website. The code then executes inside the browser (i.e on the machine of the website visitors).
* **On any computer**: Thanks to Node JS or Deno, JavaScript code can be executed outside the browser too. The code then executed directly on machine.
* **On mobile devices**: With Extra technologies like **Capacitor** or **React Native**, you can build mobile apps based on JavaScript. The code then executed on mobile device.


## Adding JavaScript Code to a website.
* Between `<script>` tag: Can Quickly leads to unmaintainable and complex HTML files.
* Via `<script>` import: Separates HTML and JavaScript code.

## Practically adding.
### One Thing To Remember: defer tag.
```
<head>
   <script src="assets/script/app.js" defer></script>
</head>
```
* Here we are using defer the reason is, if we are implementing a code which does require HTML to be loaded first then not including defer would create a trouble.
* There is another way to do the same thing is to include the script file after body tag.

### Another Thing To Remember: type tag.
```
<head>
    <script src="assets/scripts/app.js" type="module"></script>
</head>

It usually defines the type of the script.
This module type will be treating the Javascript file as a module. We can import code from one JS file to another.
```

### React Project Uses A Build Process.
