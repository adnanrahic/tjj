# The JavaScript Journey - Chapter 1 Recap

![](https://github.com/adnanrahic/cdn/raw/master/tjj-ch-1-recap/1-U5ds1ja91Yw24kF6zfuFAkexbgZBjvt_1680x8400.jpg)

## Chapter 1 - Recap
Welcome to the end of what has been an awesome first step. You've made it through the introductory leg of *The Journey* . Way to go to! You have come a long way. This first chapter has been a roller-coaster ride of emotions, thrills and new experiences.

## Values
You've learned about the [basics of computers and how they store values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values). A key abstract concept in understanding programming. Furthermore, you now know what different kinds of values we have in JavaScript land. Numbers, Strings, Booleans, Fractions, Null and Undefined. But this is only the first step into the bottomless pit of values. These are only basic representations of values. They are primitive, and cannot be divided into simpler pieces. Imagine atoms! Remember back in primary school physics class, when you learned about the inseparability of atoms! View these basic value types as you would atoms in primary school.

## Arithmetic and Operators
But there's not really that much we can do with values alone. We need something more. [Operators! A way of combining values and performing operations on them](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators). If you hated math in school, now you'll start loving it instead! It finally makes sense, everything you learned in school that seemed so senseless, will now have meaning. Math has now become important! All the basic operators we have in math, are available in JavaScript as well (```+, -, *, /```). With the small addition of a couple of special operators. The remainder (```%```) operator is one of them! However, There's so much more to operators than just maths. We have operators to glue together string values, like so ```con + ca + te + nate```. And operators to check the type of any value: ```typeof 12.7```. Then again, don't forget about binary operators.

- ```>=``` is greater than or equal to
- ```<=``` is less than or equal to
- ```==``` is equal to
- ```!=``` is not equal to

![](https://github.com/adnanrahic/cdn/raw/master/tjj-3/1-U5dt6BgXtFvsV5rRuUp76c1LDHNrpZ9_1680x8400.jpg)

## Logical operators
[Again, more operators... Would you believe all operations performed with a binary operator are called, shockingly, a binary operation](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators). Very surprising, right!? So, what's important to take away from this statement? Any binary operation must eventually be equal to a Boolean value, a true or false. Including logical operators:

- AND, represented with - ```&&```
- OR, represented with - ```||```
- NOT, represented with - ```!```

```
// AND
true && false // → false
true && true // → true

// OR
false || true // → true
false || false // → false

// NOT
!true // → false
!false // → true

```

###

Have in mind, **precedence** is key. It defines in which order a set of operations will be evaluated. Operations with **higher** precedence will be evaluated **first**. Logical **OR** (```||```) has the lowest precedence, then comes logical **AND** (```&&```), then the comparison operators (```>, ==, <, !=, ...```), then the rest.

To finish off the discussion about operators, we only need to mention one more. The ternary operator. The **only** operator in JavaScript which takes **three** values.

```
true ? 1 : 2 // → 1
false ? 1 : 2 // → 2

5 > 4 ? 'buy bread' : 'do not buy bread' // → 'buy bread'
true || false ? 'meatballs' : 'spaghetti' // → 'meatballs'
true && false ? 'meatballs' : 'spaghetti' // → 'spaghetti'
```

###

The leftmost expression will evaluate to either ```true``` or ```false```. If it is ```true```, the middle value will be the result of the operation, otherwise, if the expression is ```false```, the rightmost value will be the result of the operation.

## Special Values
Do you remember which values are special in JavaScript? [Let me give you a hint, they rhyme with full and peace of mind](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons). You got them? Let's continue calling them ```full``` and ```peace of mind``` for the heck of it, in the next couple of paragraphs. These two buddies are for the most part interchangeable. JavaScript will mainly view them as exactly the same. However, they are not! The value of *full*, is indeed **nothing**, ```null```, nada, zip, absolutely empty. The exact opposite of full. It is ```null``` and it has special meaning in JavaScript. However, *peace of mind* is another story altogether. ```Undefined``` represents the absence of a defined value. JavaScript knows a value should exist, but it was not given. This will make much more sense in the coming lessons.

## Type Conversions
Weirdly enough, JavaScript is like a retarded friend, he's so willing to help you out, but whatever he does never really helps you... at all... ever. He's so nice, he tries to convert the types of the values in a comparison operation. Where ```'5' - 1``` is equal to ```4```, and ```'5' + 1``` is equal to ```51```. I know, but why though!? What are you thinking? Beats me, I know it's called **type coercion**. Remember this, please.

<!-- ![](https://github.com/adnanrahic/cdn/raw/master/tjj-ch-1-recap/2-U5dsXdirt5CKLzJbKb47FvH8cPVNS3n.gif) -->

<p>
<center>
<img src='https://github.com/adnanrahic/cdn/raw/master/tjj-ch-1-recap/2-U5dsXdirt5CKLzJbKb47FvH8cPVNS3n.gif'>
</center>
</p>

## Precise Type Comparisons
Thank the flying spaghetti monster, we have a way to stop this! With the precise type comparison. Colloquially called the *triple-qual-to*.

- ```===```
- ```!==```

These awesome operators are what make it possible to disable type coercion. Making the expression ```'5' === 5``` evaluate to false.

## Summary
This has been a brief recap of the first four lessons of *The JavaScript Journey*. With this, Chapter One is complete! You can check out [Lesson 4](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons) if you need to go over some examples again. Hope you guys and girls had fun learning alongside me. Tune in next time when we'll finally start some real coding.

___

## Chapter 1
- [Lesson 1 - Values](https://steemit.com/programming/@adnanrahic/the-javascript-journey-1-values)
- [Lesson 2 - Arithmetic and Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators)
- [Lesson 3 - Logical Operators](https://steemit.com/programming/@adnanrahic/the-javascript-journey-3-logical-operators)
- [Lesson 4 - Special Values and Precise Comparisons](https://steemit.com/programming/@adnanrahic/the-javascript-journey-4-special-values-and-precise-comparisons)

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, so more people will see it here on Steemit.*
*Share if you believe it will be of help to someone.*

*Feel free to ask any questions you have in the comments below.*