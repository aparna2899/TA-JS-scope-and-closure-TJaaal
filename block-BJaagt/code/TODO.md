Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = "Arya";
}
console.log(username); // output
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = "Arya";
}
console.log(username); // output
```

We can't access the variable username defined inside a block from outside because const is block scoped.
The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = "Arya";
}
console.log(username); // output
```

We can't access the variable username defined inside a block from outside because let is block scoped.
The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = "Arya";
}
console.log(username); // Arya
```

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  var username = "Arya";
}
console.log(username); // output
```

let variables can't re-declared.
The above code will throw an error `Uncaught SyntaxError: Identifier 'username' has already been declared`.

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
if (true) {
  let username = "Arya";
}
console.log(username); // John
```

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = "John";
function sayHello() {
  let username = "Arya";
}
sayHello();
console.log(username); // John
```

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, "First"); // 0 'First', 1 'First', 2 'First', 3 'First', 4 'First', 5 'First', 6 'First', 7 'First', 8 'First', 9 'First'
}
console.log(i, "Second"); // 10 'Second'
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, "First"); // 0 'First', 1 'First', 2 'First', 3 'First', 4 'First', 5 'First', 6 'First', 7 'First', 8 'First', 9 'First'
}
console.log(i, "Second"); // output
```

We can't access variable i outside the block because i declared by let is block scoped.
It will throw an error `ReferenceError: i is not defined`
