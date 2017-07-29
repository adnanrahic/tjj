# The JavaScript Journey #4 - Special Values & Precise Comparisons

## Intro
This lesson will cover the art of comparing values to each other. The phenomenon is called comparison operations. We touched upon the basics of arithmetic and comparison operators in [Lesson 2](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators). Today we will do a thorough deep dive into the inner workings of precise comparisons in JavaScript. Meaning we first need a good understanding of **data types** and **special values**.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-4/1-U5dsJ7tzqi3Zuy3fxBfvTWpwyKRFcVo_1680x8400.jpg)

## Special values
So, what's a data type? Hereto, we've been introduced to three main types of storing data. Numbers, Strings, and Booleans. They all represent a way of holding onto a set of bytes in a computer's memory. However, they have different meanings to us, people. We perceive them as meaningful information. A number can have some significance to us, as can a string. How then can we represent the absence of a value? Is the lack of a value still relevant to us? Of course! Hence the need for a way to represent the nothingness, or absence of something.

There exist **two** special values is JavaScript. They are:

- undefined
- null

As you can see, they are indeed values. They hold weight in the language of JavaScript, but they do **not** carry any information. Meaning they are of crucial importance in the language even if they do not carry any info. Weird right? At first glance, yes, very strange. But, take a step back and look at this from another angle. Incredibly many operations within JavaScript don't produce a meaningful value. How would you represent that lack of a value? That's the question! You guessed it, with ```null``` or ```undefined```. You will see in the coming chapters of this series what makes the two different. For now, you can view them as equals.

How does this relate to comparisons? Well, only if both ```undefined``` and ```null``` occur on both sides of an equality operator does the expression hold ```true```.

```
null == undefined
// → true
```

###

In **any** other situation, when either ```null``` or ```undefined``` is compared to any other value the equality will hold ```false```.

```
null == 0
// → false
undefined == '13'
// → false
```

Now we've come to an important fact. This technique is widely in use to check whether a value actually holds a real value instead of ```null``` or ```undefined```. You compare it to ```null``` with the not equals to (```!=```) operator.

```
myValue != null
// → true only if myValue has a real value
```

## Automatic type conversion
There's one really weird thing about JavaScript I want to share with you before moving on to the more hands-on things of today's lesson. What do you think will happen here? Try to deduce what the expressions below will produce:

```
8 * null

'5' - 1

'5' + 1

false == 0
```

No peeking, the correct answers are below.

```
8 * null
// → 0

'5' - 1
// → 4

'5' + 1
// → 51

false == 0
// → true
```

But, how? Why? This is madness!

###

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-4/2-U5drQiQY9MnYGA4evb1sm5bi8nXkmX9_1680x8400.png)

When an operator is applied to the *wrong* type of value, JavaScript will quietly convert that value to the type it wants. In the first example, ```null``` will be converted to ```0```. The second will convert ```'5'``` to the number ```5```. While in the third, the same string value ```'5'``` will remain a string while the number ```1``` will be concatenated onto it. The fourth example converts the value ```0``` into the Boolean value ```false```. A quick heads up, keep in mind, often are the Boolean values of ```true``` and ```false``` represented as the number values of ```0``` and ```1```. This strange behavior of converting data types is called **type coercion**. It's actually meant to be a way of helping the developer. Where the language itself tries to give you a hand in coercing different values to change their type in order to help you out. Sadly, it only creates more issues than it does good. Luckily, this is why we have something called precise type comparisons.

## Precise type comparisons
As you have seen in the examples above, ```0 == false``` and ```'' == false``` evaluate to ```true``` because of automatic type conversion. How does one disable this then? Well, you don't really have a way of disabling it. The way you solve this issue is with two extra operators available in JavaScript by default. They are:

- ===
- !==

These beautiful, awesome, incredible, lovely babies are what make it possible to disable type coercion. Making the expression ```'5' === 5``` evaluate to ```false```. Whenever JavaScript sees one of these precise comparison operators it knows not to implicitly convert any of the values in an expression. This expression needs both the data type and value of the two values to be exactly the same. Keep this in mind. It will be a huge help when you advance your career as a software developer.

![puzzle piece](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-4/3-U5duJ9j47ujF9RtFASVJLipeGYeCZPD_1680x8400.jpg)

## Let's put it all together
I'll give you a set of exercises to solve including all the different topics we went through in the past few lessons. Don't worry, nothing will be hard, and of course, I'll add the solutions and explanations below.

Evaluate the expressions:

```
true === 13 - 12 >= 1 && 3 * 3 < 10
false === 0
true == 1
typeof 13 === 'number' ? '13 is a number': '13 is not a number'
```

###

Take your time, when you think you have evaluated the expressions correctly, take a peek below.

```
true === 13 - 12 >= 1 && 3 * 3 < 10 
// true

false === 0 
// false

true == 1 
// true

typeof 13 === 'number' ? '13 is a number': '13 is not a number' 
// '13 is a number'
```

###

Explanation time! Take a closer look at the first expression. We see the left side of the precise comparison is the value ```true```. Meaning the whole right side of the expression must evaluate to ```true``` in order for the whole expression to hold true. Let's get going. By order of precedence we must first evaluate the arithmetic operators, giving us something like this:

```
true === 1 >= 1 && 9 < 10 
```

###

Then we evaluate the comparison operators:

```
true === true && true 
```

###

Lastly, we evaluate the logical operators:

```
true === true
```

###

Coming to the end we see that indeed this precise comparison holds true, as both sides of the precise equality operator are true.

The second problem is easy. We see that the precise comparison requires the same data type, but the right side doesn't match the left, so without even evaluating anything we know this precise equality can never be true.

The third problem is a bit tricky. The regular equality operator will coerce the data type of the right side of the operator. Making the Boolean ```true``` equal to the number ```1```.

The last problem is a bit more complex. Here we see a common use case for the ternary operator. Everything on the left side of the question mark (?) is an expression. The whole thing has to be viewed as an expression. ```typeof 13 === 'number'``` when evaluated actually is ```true```. The ```typeof``` operator is a unary operator that returns a string value of the type of the value it was called upon. That was a bunch of complicated words. Breaking it down. ```typeof 13``` evaluates to ```'number'```, so the expression:

```
typeof 13 === 'number'
```

###

can be viewed as:

```
'number' === 'number'
```

###

which is, of course, ```true```!

Moving on, with the left side of the question mark being true, the whole ternary operator will evaluate to the first value to the right of the question mark. Which is ```'13 is a number'```. Otherwise, if the expression would have been false, the ternary operator would evaluate to the value to the right of the colon (:).

## Summary
Awesome stuff! Today's lesson was a bit more demanding than the ones before. We went through more complex concepts of the language such as ```null``` values and type coercion. Finally, we learned how to disable implicit type conversion with the use of ```===``` and ```!==```, the so called precise comparison operators. Great job. Hope you had fun with the exercises!

---

## Check out previous lessons
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)
- [Lesson 3 - Logical Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators)

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*
*It means a lot to me.*

*Feel free to ask any questions you have in the comments below.*