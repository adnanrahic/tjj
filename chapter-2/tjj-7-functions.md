# The JavaScript Journey #7 - Functions

![]()

I guess if you've ever watched the any space sci-fi movie ever you'll be familiar with what functions are. In space travel all the heroes need to go to cryo-sleep in order to travel the vast distances between stars. How does any of this make any sense, you ask? I'm not losing my mind, promise! View functions just like the space heroes exploring galaxies. Functions freeze code in order to use it at a later time. This frozen code can be re-used as many times as you wish, without the need to write it again and again. 

## Dry Theory
First and foremost let's go though some dry theory. Before being able to understand the logic behind functions we need to hear the official definitions.

### Wrapping code
Any function is a piece of code or program wrapped in a value. These values can be executed in order to run the wrapped program. Executing such a value, a function, is called **invoking**, **calling**, or **applying** it. All of these are heavy words. In the rest of the lesson we'll stick to **calling** to keep it simple and concise. So how do we tell our program to call a function? Easy, we just put parentheses after the value which holds the function.

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

You see? The function has returned a value and assigned it to the variable ```maxNumber```. This means the function produced a value. Having this in mind, everything that produces a value is an expression. So it can be used in combination with other expressions.

```javascript
Math.max(2, 4) + 6 > 5 || 1 == Math.min(1, 7)
// true
```


## 