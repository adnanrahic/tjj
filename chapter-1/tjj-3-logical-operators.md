# The JavaScript Journey #3 - Logical Operators

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-3/1-U5dt6BgXtFvsV5rRuUp76c1LDHNrpZ9_1680x8400.jpg)

## Intro
Today's lesson will cover the concept of logical operators, what they are and how to use them. The logic behind them is very simple. No pun intended they are called logical operators after all. View them as simple electrical circuits. There are three possible outcomes based on which current will flow through the hypothetical wires.

## Again with the operators...
[Last lesson](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators) we covered what operators and expressions are. Operators, just as their names state, *operate* on one or two values. These values must eventually be equal to a Boolean value, a simple ```true``` or ```false```. Logical operators are, in turn, very similar to the arithmetic operators we learned about last lesson. The way they behave is at the logical level almost the same. The key exception being on what types of values the operators can be applied to.

Logical operators can be applied to Boolean values themselves. Meaning, they are used to *reason with Booleans*. Let's say you want to make sure both ```5``` is greater than ```4``` **and** ```7``` is less than ```9```. Only if both of these expressions hold ```true``` will the logical operation hold ```true```. In another case, let's say you want to check whether ```1``` is equal to ```2``` **or** ```7``` is equal to ```7```. It's perfectly fine if only one of the two arithmetic expressions holds ```true```, the logical operation will hold ```true```.

Let's break it down. JavaScript supports three main logical operators.

- AND
- OR
- NOT

## AND
In JavaScript, there are special characters which represent certain operators, in this case, logical operators. The ```&&``` operator represents logical **AND**. This is a binary operator, and its result is ```true``` only if both the values given to it are ```true```. By being a binary operator it takes two values.

```
true && false // → false

true && true // → true
```

###

## OR
This logical operator is denoted by the special symbol called pipe. The pipe symbol is written like this ```||```. Logical **OR**  will produce ```true``` if either of the values given to it is ```true```.

```
false || true // → true

false || false // → false
```

###

## NOT
**NOT** is very interesting. All it does is switching the value it is given. It's denoted by an exclamation mark, like this ```!```.

```
!true // → false

!false // → true
```

###

This may seem funny at first, but the power of this operator is incredibly useful. You can negate whole values and expressions, and even validate their existence. This comes in handy a lot.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-3/2-U5dryqSHPaWHAghV8HkcAEcBVcabKcF_1680x8400.jpg)

## Mixing operators
When you mix operators, how do you know which will be executed first? Well, with arithmetic it's easy, you just follow the logic of math you learned in primary school. Multiplication and division first, then addition and subtraction. But what now? Logical operators don't exist in arithmetic. The use of operators boils down to something called **precedence**. Operator precedence determines which operator will be evaluated first, meaning the ones with **higher** precedence are the ones to be evaluated first.

Logical **OR** (```||```) has the lowest precedence, then comes logical **AND** (```&&```), then the comparison operators (```>, ==, <, !=, ...```), then the rest.

Here's an exercise for you to solve:

```
1 + 1 == 2 && 10 * 10 > 50
// what is the value of this expression?
```

###

## Ternary operator
All binary operators interact with only two values, hence the name, *binary*. However, there is one operator in JavaScript which is *ternary*, and it operates on three values.

```
true ? 1 : 2 // → 1

false ? 1 : 2 // → 2
```

###

This is the only ternary operator in JavaScript. Often called the conditional operator, as it defines a condition to be met, based on which a result will be picked. The value on the left of the question mark *picks* which of the other two values will come out. 

When it is ```true```, the middle value is chosen, and when it is ```false```, the value on the right comes out.

## Summary
Great work! Logical operators are the core building blocks of any program. These expressions are used to check the validity in many parts of our programs. The ```true``` or ```false``` value dictates whether the program will continue executing or follow a totally opposite flow of control. These concepts will all be crystal clear to you in a few lessons when we get into them in more detail. Join me in the next lesson when I'll be writing about **special values**, and **precise type comparisons**.

You can read the next lesson [here](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons).

## Check out previous lessons
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*
*It means a lot to me.*

*Feel free to ask any questions you have in the comments below.*