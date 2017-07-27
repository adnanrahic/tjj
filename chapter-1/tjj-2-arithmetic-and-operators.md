# The JavaScript Journey #2 - Arithmetic and Operators

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-2/1-U5dtyp4yUq6it5gS57bTa8VjxZZhE4J_1680x8400.jpg)

## Intro
Last lesson you gained the understanding of how computers work, what bits are, and how to use the binary numbering system. You learned what basic data types are, their characteristics and how they behave. We only touched the definitions and basic use cases of Numbers.

If you missed lesson #1, you can take a look at it [here](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values).

## Now you'll see why math is important.
This time you will see how to make numbers interact with each other. The main thing you can do with numbers is arithmetic.

```
99 + 6 * 12
```

###

The ```+``` and ```*``` symbols are called **operators**. What do you think happens first in the expression above? Have in mind the first operator stands for addition while the second stands for multiplication. Putting an operator between two values will cause it to produce a new value. Remember math class in primary school? Do you realize now how important that was?

The result of the expression above is ```171```. First, ```6``` and ```12``` are multiplied, then the result is added.

What about now?

```
(99 + 6) * 12
22 - 5 / 7
7 / (27 + 3) * 99
```

### 

When operators appear together without parentheses, the order in which they are applied is determined by the precedence of the operators. First multiplication and division are calculated, then addition and subtraction. Same as when using operators in math!

The four main arithmetic operators are, like in math: ```+, -, *, /```. However, we have one more special operator in JavaScript. The ```%``` symbol is used to represent the remainder operator. ```X % Y``` is the remainder of dividing ```X``` and ```Y```.

```
314 % 100 = 14
```

###

This operation is often called modulo or modulus. However remainder is a but more accurate.

## What about strings?
Good question. Strings cannot be manipulated with arithmetic operators. They cannot be divided, multiplied nor subtracted. Now comes the funny bit. The ```+``` operator can be used on strings. But this process does not add strings. It only glues them together in a process called **concatenation**.

This expression will form the string value *concatenate*.

```
'con' + 'ca' + 'te' + 'nate'
```

###

## Unary operators
Enough about arithmetic, let's talk about something more interesting. Operators don't need to be symbols, there are many different types of operator, one of which stands out.

```
typeof
```

###

This operator is unary, which means it operates on a single value.

```
typeof 12.7
```

###

This expression will return a single string value naming the type of the value to the right of the operator. In this case, ```typeof 12.7``` would be equal to ```'number'```. What do you think would be the value of the expression below?

```
typeof 'x'
```

###

If you guessed ```'string'```, then you deserve a gold star! Good job, you're getting the hang of this.

All arithmetic operators are **binary** which means they operate on **two** values. The operator ```typeof``` is not, as it only operates on **one**. In all general cases, you will only ever come across the fact that ```typeof``` is the only unary operator in JavaScript. However, JavaScript is a bit freaky, so it has its exceptions. The minus operator (```-```) can also be a unary operator.

```
- (16 - 5)
```

###

The expression above equals ```-11```. The minus operator changes the sign of the number value, making it, in turn, a unary operator.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-2/2-U5dtsqwgGioyMcYDY4DFXet7exkLVhx_1680x8400.jpg)

## Binary operators
To understand the concept of binary operators you first need to get acquainted with **Boolean** values. A Boolean value is simply a value that has the possibility of being either ```true```, or ```false```. Just like a light switch. It's either on, or off. A value is present, or it is not. The values of ```true``` and ```false``` are actual values stored in the computer's memory.

So, what's a binary operator now? It compares two values. It **operates** on two values.

```
3 > 2
7 < 4
```

###

These are examples of binary operators, the less than sign (```<```), and the greater than sign (```>```). Applying these operators to two numbers, as in this case, has the result in the shape of a Boolean value that indicates whether the expression holds true. Remember primary school math? How many more operators like these two are there?

- ```>=``` is greater than or equal to
- ```<=``` is less than or equal to
- ```==``` is equal to
- ```!=``` is not equal to

Which of these expressions hold true?
Don't look at the solutions below before trying it yourself!

```
1. 9 / 3 + 1 <= 4 * 2 - 4
2. 2 + 5 * 2 > 3 - 4 / 2
3. 1 * 54 == 25 / 5 * 20
```

###

___

Solutions:
```
1. true
2. true
3. false
```

###

## Summary
Great work! You've brushed up on your math skills and applied them in the field of programming. Arithmetic and operators are the core building blocks of any program. These expressions are used to check the validity in many parts of our programs. The ```true``` or ```false``` value dictates whether the program will continue executing or follow a totally opposite flow of control. These concepts will all be crystal clear to you in a few lessons when we get into them in more detail. Join me in the next lesson when I'll be writing about **logical operators**.

You can read the next lesson [here](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators).

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*
*It means a lot to me.*

*Feel free to ask any questions you have in the comments below.*