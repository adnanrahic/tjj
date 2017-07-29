# The JavaScript Journey #5 - Expressions and Statements

## Intro
Have you ever heard of program structure? I haven't for a very long time. Why is that, you now ask yourself? Well, let me break it down. As a productive human being, a part of society, you learn social norms and practices by which you act on a daily basis. You know not to chew with you mouth open, you know how to behave kind in the supermarket. You simply know all these socially acceptible things by which you choose to live. 

The exact same principles go for writing programs. There exist norms and laws by which you structure your program. They have not been introduced to the programming codex just on a whim. Every single one of them exist for a reason. And just as with social norms, you get used to them, they stick to you, your character, the way you act. In turn, becoming a part of your personality. After a while you stop thinking about these codes. The norms just seem natural to you, as will program structure, in time, grow on you to a point where it is as natural as the air we all breathe.

Today's lecture will finally contain some *real* programming. The things we'll start doing today can actually be percieved as programming. Hereto, we have only been playing with nouns and fragments of sentences in the language of JavaScript. Ready to jump into the deep end of the pool? I sure am.

## Expressions and statements
Values are essential in every part of a JavaScript program. You may now asume how incedibly important it is to be able to create them at will. This is what an expression actually is. An expression is a fragment of code that produces a value. Imagine this, every value is actually an expression. How trippy is that?

Take a look, all of these values are expression:
- 22
- "psychoanalysis"
- (2 * 4)

How can we as humans understand what the logic behind this actually means, and how to *translate* it into human language? An expression symbolises a sentence fragment, lets say a verb or noun. While a JavaScript statement is a full sentence. Meaning that all a JavaScript program actually is, is a large list of sentences. Taking a step back and thoroughly thinking about this fact, it makes so much sense. Programming code exists so that humans can read it, and understand the commands the computer should execute. Programming code exists for humans, we write code for other humans to understand. The computer doesn't care what the code looks like. It will only compile it into simple bits in the end.

But how do we know what a statement is? The simplest kind of statement is an expression with a semicolon after it.
This is a program:

```
!false;
```

###

It is a useless program, though. When executing the program, nothing observable happens. But, it gets the point across. This small snippet of code will execute and produce an effect. Sadly nothing will happen as the program will only run this single line of code. What's important to take away from this example is the semicolon (```;```). When JavaScript sees a semicolon it always ends the execution of that statement. The ```;``` is a global symbol for signaling the end of a statement.
