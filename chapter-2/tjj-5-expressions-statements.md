# The JavaScript Journey #5 - Expressions and Statements

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-5/1-pexels-photo-154141.jpeg)

## Intro
Have you ever heard of program structure? I haven't for a very long time. Why is that, you now ask yourself? Well, let me break it down. As a productive human being, a part of society, you learn social norms and practices by which you act on a daily basis. You know not to chew with your mouth open, you know how to behave kindly in the supermarket. You simply know all these socially acceptable things by which you choose to live. 

The exact same principles go for writing programs. There exist norms and laws by which you structure your program. They have not been introduced to the programming code just on a whim. Every single one of them exists for a reason. And just as with social norms, you get used to them, they stick to you, your character, the way you act. In turn, becoming a part of your personality. After a while, you stop thinking about these codes. The norms just seem natural to you, as will program structure, in time, grow on you to a point where it is as natural as the air we all breathe.

Today's lecture will finally contain some *real* programming. The things we'll start doing today can actually be perceived as programming. Hereto, we have only been playing with nouns and fragments of sentences in the language of JavaScript. Ready to jump into the deep end of the pool? I sure am.

![](https://github.com/adnanrahic/cdn/raw/master/tjj-5/2-pexels-photo-247791.png)

## Expressions and statements
Values are essential in every part of a JavaScript program. You may now assume how incredibly important it is to be able to create them at will. This is what an expression actually is. An expression is a fragment of code that produces a value. Imagine this, every value is actually an expression. How trippy is that?

Take a look, all of these values are expressions:
- ```22```
- ```"psychoanalysis"```
- ```(2 * 4)```

How can we as humans understand what the logic behind this actually means, and how to *translate* it into the human language? An expression symbolizes a sentence fragment, let's say a verb or noun. While a JavaScript statement is a full sentence. Meaning that all a JavaScript program actually is, is a large list of sentences. Taking a step back and thoroughly thinking about this fact, it makes so much sense. Programming code exists so that humans can read it, and understand the commands the computer should execute. Programming code exists for humans, we write code for other humans to understand. The computer doesn't care what the code looks like. It will only compile it into simple bits in the end.

But how do we know what a statement is? The simplest kind of statement is an expression with a semicolon after it.
This is a program:

```
!false;
```

###

It is a useless program, though. When executing the program, nothing observable happens. But, it gets the point across. This small snippet of code will execute and produce an effect. Sadly nothing will happen as the program will only run this single line of code. What's important to take away from this example is the semicolon (```;```). When JavaScript sees a semicolon it always ends the execution of that statement. The ```;``` is a global symbol for signaling the end of a statement.

## Summary
Today we covered the basics of program structure, JavaScript expressions, and statements. You now know expressions are just nouns, verbs or sentence fragments, while statements are the actual sentences. When you break it down like this it is much easier to understand. A simple statement can be:

```
2 * 8 > 5;
```

###

And it will run the program evaluate the expression to ```true```, and stop the execution. JavaScript knows when to finish executing a line of code when it reaches a semicolon (```;```). It immediately skips reading the rest of that line and just jumps down to the line beneath.

Stay tuned for next time when I'll be writing more about **program structure** and **variables**.

---

## Check out previous lessons
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)
- [Lesson 3 - Logical Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators)
- [Lesson 4 - Special Values and Precise Comparisons](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons)
- [Chapter 1 Recap](https://steemit.com/programming/@adnanrahic/the-javascript-journey-chapter-1-recap)

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*
*It means a lot to me.*

*Feel free to ask any questions you have in the comments below.*