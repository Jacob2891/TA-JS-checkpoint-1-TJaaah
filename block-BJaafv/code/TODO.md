1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

Answer - the first sum function will return a value which means we may store in a variable , Whereas second sum function output is in console , and we cant store it in a variable  .


2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

Answer - 

value of first - 10 sum(5,5);

value of second - 10 sum(5,5);

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

answer - 
sum(5,5,5);
10

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

ANS - yes we can store the sum variable into add , reason being there is not limit of which variable well be storing into another , if we have specified explicitly the given value will be reasssigned to a new variable.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

ANS - 

```js
function sayHello (name){
  return (`Hello`+` `+`${name}.`)
}

```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
ANS - `Hello, John` , there is a space in function body between Hello and username, hence the output has a space in it . 

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // John

showMessage(); // `Hello John`

alert(userName); // John
```

8. What is a Anonymous Function give example of three functions.

ANS - anonymous function is one where we dont mention function name in function declaration , it usually occurs when we are assigning a function to a varaiable ,
EX: let X = function (a,b) {
  return (a+b);
}

9. Can function declaration be a Anonymous Function? Explain

Yes reason same as Q.8

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
ANS - 

1. calcSalary
2. showResult
3. checkStatement
4. createLine
5. getBalanceSheet