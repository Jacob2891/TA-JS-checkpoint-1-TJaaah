1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let y = 0 ;
letx=0 ;
for (i=1;i<=10;i++) {
x = Number (prompt(`enter a number`));
y += x ;
}


let average = (y/2); 
console.log(`The average of given 10 numbers is ${average} .`)

```

2. What will be the output of the code below
```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
ANS - error , it needs to be console.log in place of printIn.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

ANS - 
```js

let evenNum=0;
function getEvenSum (max=10){
 for(i=0;i<=max;i++){
   if (i%2 == 0)
   evenNum += i ;
 }
 console.log(evenNum);
}

```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

ANS - 

```js

let oddNum=0;
function getOddSum (max=10){
 for(i=0;i<=max;i++){
   if (i%2 != 0)
   oddNum += i ;
 }
 console.log(oddNum);
}

```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

ANS - 

Knowledge Gap , Iam not able to find solution with current knowledge .

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // Bigger than 5
check(1); // Smaller than 5
check(5); // 5 , reason being we havent mentioned any output for when num =5 , so the default action of returning the num value is met , so output is the num value 
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output
getOutput('John'); // what will be the output
getOutput(); // what will be the output
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // You are arya / 'Who are you' / reason being one output is due to the condition being met , and the other out put is due to the return statement 
getOutput('John'); // You are john / 'Who are you' / reason same as above
getOutput(); // 'Who are you' / reason being if paramenter being blank the return statement is `Who are you`
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

ANS -  NO , we cant have two return statement , reason being its too confusing in general when we will call function in future and the current syntax doesnt allow it too .

Example
```js

function addNumbers (x,y){
  return x+y ;
  return x*y ;
  }

  addNumbers(3,5);
 ```
This code returns the output of first return statement , i.e 8 , hence the second return statement is ignored .

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

ANS - for loop is used when we know the start and end point of a loop for loop is preferred over while loop by coding community in general , whereas While loop is very useful when we have only one condition to work with .

Example :- 

For loop can be used to print out numbers 1-10

```js
for(i=1;i<=10;i++){
  console.log(i);
}
```

While loop is useful when we aren't aware of the start and end of a loop

```js
let x = 0;
let y = 0;

while (x < 4) {
  x++;
  y += x;
}
```