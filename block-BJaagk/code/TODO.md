1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

let percentage = function (marks, total) {
  return (marks * 100) / total;
};

let percentage = (marks, total) => (marks * 100) / total;
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
Arrow Function
```

```js
let percentage = (marks, total) => (marks * 100) / total;
Arrow Function
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

Beacause function is an object in javascript so it can be stored in a variable.

```js
let sayHi = function (name) {
  console.log(`Hi ${name}`);
};
```

4. Why is a function call an expression in JavaScript?

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid, return 5
five = add; // Valid, return function definition
five = five(10, 11); // Valid, return 21 because five stores function definiton
five = function () {
  return "Hello";
}; // Valid, can store function in a variable.
```

6. What is the difference between function definition and function call? Explain with an example.

Defining a function involves naming the function, identifying the parameters, and identifying a returned result while function call is invoking or calling that function.

```js
//Function definition
let sayHi = function (name) {
  console.log(`Hi ${name}`);
};

//Function call
sayHi(`Arya`);
```

7. What is the similarities between function definition and function call?

Both are expressions.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log("Hello World!");
}

hello.user = "Sam"; // Valid, because function is an object
```

9. What is higher order function explain with an example.

A function that accepts or returns another function is called a higher-order function.

```js
let numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9];
let even = numbers.filter((num) => num % 2 === 0);
```

10. Explain what is callback function. Why you can pass a function inside a function?

A function which is passed in higher order function as an argument is a callback function.
Because functions are expressions.
