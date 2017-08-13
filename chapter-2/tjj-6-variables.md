# The JavaScript Journey #6 - Variables

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-6/1-pexels-photo-346885.jpeg)

## Intro
You've heard of this before, haven't you? Just like in algebra, variables have their place in programming. What an important place it is indeed. Let's use the generic, boring, and worn out explanation of what a variable is in JavaScript. It's a container for holding different values. Simple enough, right? 

## Catching values
Sadly, this is not the case. Variables are not containers. Variables catch and hold on to values. We do not put values into variables. Think outside the box for the rest of this lesson.

```
var catchingSomeValue = 8 * 8;
```

###

This, as well, is a statement. More precisely, the act of **declaration** / **definition**. The keyword ```var``` indicates that the expression is going to define a variable. The expression above states that we are going to assign the value of ```8 * 8``` to the variable ```catchingSomeValue```. This means we can now use the name of the variable as an expression. After a variable has been defined its name will always be an expression. The value of this expression is the value it has been assigned, in our case ```8 * 8```. 

```
var eight = 8;
var catchingAnotherValue = eight * eight;

// whats the value of catchingAnotherValue ?
-> 64
```

###

Let's see this in action. Open up your browser of choice, and open up the developer tools. My browser of choice is Chromium, I usually press ```ctrl + shift + j``` to open up the console. You can also press ```F12```. This works in every browser, even Internet Explorer (please don't use IE though). Okay, so after pressing ```F12``` you should see a window pop up with some tabs, press the ```console``` tab. And click just right of the little chevron symbol. Go ahead and write:

```
var eight = 8;
```

###

And hit enter. Now write ```eight``` and hit enter again. You should see the value ```8``` get printed to the console! Play around a bit with this and you'll get the hang of it.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-6/2-Selection_018.png)

## Naming your variables
Think about giving your variable the name ```var```. Do you think this would be valid? No. You're right. There are certain laws about what is allowed in a variable name. You definitely do not need to know them all by heart, just remember the main things and everything else will come naturally the more time you spend coding.

Moving on, what can be in a variable name? Any word that is not a reserved word, such as ```var``` or any other keyword in JavaScript. Spaces are not allowed, nor is punctuation (except for ```$``` and ```_```). The thing with numbers is strange, they are allowed, but only if they are not at the beginning of the variable name. This means ```catching77``` is valid, but ```77isCaught``` is not.

## Variables are not containers
Let's touch on this again. Variables point to values, they are not tied forever. Values are not put into containers. The ```=``` operator is used to connect and disconnect values from variables. 

```
var weather = 'rain';
-> the value fo weather is 'rain'

weather = 'sunshine';
-> now the value of weather is 'sunshine'
```

###

See? First, weather pointed to the value ```'rain'```. Then, we made it point to another value, ```'sunshine'```. Imagine variables as tentacles. They are not buckets, nor containers. They grasp values, hold on to them, as you would grasp a glass of water with your hand. You can drop it if you so wish, or drink it. Both of which will change the value of what you are holding. Variables do not contain values! This is why two variables can refer to the same value. Just as you can hold the same glass of water with both hands.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-6/3-octo.jpeg)

## Grasping variables
In JavaScript and programming in general, you can only access values you have a hold on. If you want to hold on to more values, you have to grow more tentacles, or just reattach one of your existing tentacles to the new value.

Let's say I want to buy a new shirt. I'm a bit broke so I only have $130 in my bank account.
```
var bankBalance = 130;
bankBalance = bankBalance - 30;

-> the value of bankBalance is 100
```

###

## Having nothing to grasp
Defining a value without giving it a value is like growing a new tentacle but not giving it anything to grasp. 

```
var emptyTentacle;
```

###

This is called a **variable declaration**. Creating a variable, without giving it a value. Here's a quick question. Having in mind all the things we have learned in the previous lessons. What do you think the value of ```emptyTentacle``` is? Have in mind, the variable has been declared, but not defined. What does this tell you?

If you think the value is ```undefined``` you'd be right. It makes sense when you think about it. The variable is declared but not given a value, not defined, ```undefined```.

The act of defining variables is where you declare it as well as give it an initial value. Another cool thing you can do with variables is to define multiple variables on the same line.

```
var one = 1, two = 2, three = 3;

var five = one + two + three;
-> the value of five is: 5
```

###

## Summary
Variables are the fundamental building blocks of all JavaScript programs. We use them in every part of our programs to grasp values. Variables are themselves expressions. They can be declared and defined, and the value they grasp can be easily changed. The ```=``` operator is called the assignment operator. It tells variables to point to certain values. Don't forget this part. Variables are **not** buckets, they are **tentacles**.

Stay tuned next time when I'll be writing about functions.

---

## Check out previous lessons
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)
- [Lesson 3 - Logical Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators)
- [Lesson 4 - Special Values and Precise Comparisons](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons)
- [Chapter 1 Recap](https://steemit.com/programming/@adnanrahic/the-javascript-journey-chapter-1-recap)
- [Lesson 5 - Expressions and Statements](https://steemit.com/programming/@adnanrahic/the-javascript-journey-5-expressions-and-statements)

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*

*Feel free to ask any questions you have in the comments below.*

