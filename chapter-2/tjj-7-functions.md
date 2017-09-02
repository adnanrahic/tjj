# The JavaScript Journey #7 - What are Functions?

![Space Man](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-7/1-sky-earth-space-working.jpg)

I guess if you've ever watched the any space sci-fi movie ever you'll be familiar with what functions are. In space travel all the heroes need to go to cryo-sleep in order to travel the vast distances between stars. How does any of this make any sense, you ask? I'm not losing my mind, promise! View functions just like the space heroes exploring galaxies. Functions freeze code in order to use it at a later time. This frozen code can be re-used as many times as you wish, without the need to write it again and again. 

## Dry Theory
First and foremost let's go though some dry theory. Before being able to understand the logic behind functions we need to hear the official definitions.

### Wrapping code
Any function is a piece of code or program wrapped in a value. These values can be executed in order to run the wrapped program. Executing such a value, a function, is called **invoking**, **calling**, or **applying** it. All of these are heavy words. In the rest of the lesson we'll stick to **calling** to keep it simple and concise. So how do we tell our program to call a function? Easy, we just put parentheses after the value which holds the function.

![Call a function](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-7/2-pexels-photo%20(1).jpg)

```javascript
alert('Hello Steemit!');
```
###

Here we see a builtin that will create an alert window in your browser with the text *Hello Steemit!*. But of more use to us is the ```console.log()``` function.

```javascript
console.log('Hello Steemit!');
```
###
It'll output the value given to it back to the console.

## Return to sender
The behavior above is all classified as side effects. Functions are not that simple. They can also produce new values! Which is awesome, because you don't need side effects to be useful. Let's take another built in function in JavaScript, ```Math.max```.

```javascript
var maxNumber = Math.max(2, 4);
console.log(maxNumber); 
// 4
```
###

![Return To Sender](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-7/3-14155209556_c46e13cd15_b.jpg)

You see? The function has returned a value and assigned it to the variable ```maxNumber```. This means the function produced a value. Having this in mind, everything that produces a value is an expression. So it can be used in combination with other expressions.

```javascript
Math.max(2, 4) + 6 > 5 || 1 == Math.min(1, 7)
// true
```
###

## Bread and butter
Functions are the core of programming in JavaScript. They are used to structure larger programs, and to reduce repetition. This means we can create sub-programs in our larger program. Remember, above I mentioned that functions freeze code to be used later. This can be viewed as a sub-program. And to call upon it at a later time we give it a name. Meaning every function has a name, and that it is isolated from another sub-program.

Want to create a function? I bet you do.

## Function definition
A function definition is just like a variable definition. The value of the function is assigned to the variable. 

```javascript
var square = function(x) {
  return x * x;
};
var result = square(12);
console.log(result);
// → 144
```
###

Functions are created with the ```function``` keyword. Every function has a body and parameters. The body is wrapped in curly braces (```{}```), and contains all the expression that will be executed when the function is called. Functions can have as many parameters as the programmer wants, or none at all. Here are two examples.

```javascript
// No parameters
var sayHello = function() {
  console.log("Hello!");
};
sayHello();
// → Pling!

// Multiple Parameters
var addTwoNumbers = function(x, y) {
  return x + y;
};
var result = addTwoNumbers(5, 1);
console.log(result);
// → 6!
```
###

## Backtracking
Let's take a step back and focus on ```return``` statements a bit more. I mentioned it determines what value will be returned from the function execution. But I didn't mention that the code in the function stops executing when it reaches a return statement. All code underneath a return will never be executed! 

```javascript
var addTwoNumbers = function(x, y) {
  return x + y;
  console.log('This will never be reached!');
};
var result = addTwoNumbers(1, 5);
console.log(result);
// the console.log() in the function will never be called!
// → 6!
```
###

The code that called the function will receive the value returned from it. In the example above that means the variable ```result``` will be assigned the value ```6```. But, what if we don't have a return statement in a function? What happens then!? Remember our friend ```undefined```? Every function that does not have a return statement will return ```undefined```. Take a look.

```javascript
var addTwoNumbers = function(x, y) {
  console.log(x + y);
};
var result = addTwoNumbers(1, 5);
console.log(result);
// → 6
// → undefined
```

## Summary
Today you have learned what functions are and their basic use case. You now understand that they are used to structure larger programs, and that they freeze code to be used later. They are defined with the ```function``` keyword, they have parameters and a body. Functions are **called** by putting two braces after their name. This act is also called invoking. It runs the code which has been frozen inside if the function and returns a value if it is specified within the function. Otherwise the value ```undefined``` is returned.

Hope you guys and girls has as much fun reading this as I had writing it. Next time I'll be writing about control flow and conditional statements. Heads up though, we'll return to functions more a bit later.

Until next time, have fun!

---

## Check out previous lessons
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)
- [Lesson 3 - Logical Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators)
- [Lesson 4 - Special Values and Precise Comparisons](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons)
- [Chapter 1 Recap](https://steemit.com/programming/@adnanrahic/the-javascript-journey-chapter-1-recap)
- [Lesson 5 - Expressions and Statements](https://steemit.com/programming/@adnanrahic/the-javascript-journey-5-expressions-and-statements)
- [Lesson 6 - Variables](https://steemit.com/programming/@adnanrahic/the-javascript-journey-6-variables)

---

*Drop an upvote if you liked the article, share if you believe it will be of help to someone. Feel free to ask any questions you have in the comments below.*