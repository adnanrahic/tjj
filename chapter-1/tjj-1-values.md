# The JavaScript Journey #1 - Values

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-1/U5dtFTSYx3EVKaztL79Sjtbdd1m67Wn_1680x8400.jpg)

## Are you ready to take your first step?
Welcome to a new kind of journey. A path towards making dreams come true. You wouldn't be here if you weren't already hell-bent on learning the ins and outs of programming. Do not let go of that desire. It will push you, be your leading motivation. Okay, let's get down to business, enough of my yapping.

## Intro
First of all, we need to define a bunch of key terms. These are what we will be using in the lectures to come. However, these are also universal things you will need to understand regarding computers and the science around them.

Have you ever thought about how a computer stores memes of cats in its memory? I have. Many times. The technology behind this is equally as mindblowing and putting a man on the moon. No offense NASA, but hey... memes of cats are equally as important, thank you. Anyhow, in the world of computers, there exists only data. What does this even mean? Well, anything that is not data simply doesn't exist. You can read data, modify data, create new data—but anything that isn’t data simply does not exist. All this data is stored as long sequences of **bits**, making it fundamentally alike. Ever seen The Matrix? The green numbers on the screens, remember them? Yeah, that's how Hollywood represents bits. Kind of cool right?

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-1/U5dsLAhoY4uiZdyxaev8ZPtsDCzsQJR_1680x8400.jpg)

But what are they really? They are sequences of numbers only consisting of the digits one (1) and zero (0). If any of you have been in touch with the binary numbering system you'll feel right at home. Everybody else, pay close attention. The binary system **only** consists of these two digits. The zero (0) symbolizes the lack of electrical current in a tiny transistor in the computer's CPU, while the one (1) symbolizes the presence of that same current. But, not to dive too deep into this, that's a story for another lesson.

Let's see what a sequence of bits looks like:
```
Binary  -> 0    0   0   0    1   1   0   1 
Decimal -> 128  64  32  16   8   4   2   1
```

###

This binary number you see is equivalent to 13 in decimal. How? It works on the principle of the power of two. The rightmost digit of the number is evaluated as 2⁰ (two to the power of 0). Which is equal to 1. Additionally, if this digit is 1, the value it holds will be 1 in decimal. Otherwise, it holds the value 0. This principle is the same for every other digit to the left. Here's an assignment, if you want to know more, jump over [here](http://www.electronics-tutorials.ws/binary/bin_2.html) to read more.

## Values
Can you now imagine, that a modern computer has more than 30 billion bits only in its RAM. If you're reading this in Chrome, I guess more than 20 billion of those are used by it. Okay, lame jokes aside. Now, you're wondering how the computer knows what is what in this huge amount of bits. But more important, how we as programmers how to use these bits without getting lost. We do this by chopping them into chunks which represent concrete **pieces of information**. These are called values. To create a value you must call it by its name. When you call for it, it will automagically appear before you, right there for you to use as you wish. Every value you create has to be stored somewhere. But, as soon as you no longer need the value it will dissipate, leaving behind the bits to be recycled. These recycled bits will, in turn, be used as the building material for new values. Remember, data is ever persistent. It cannot be created from nothing, nor destroyed. It only changes shapes, as the bits get re-arranged. Where have I heard this before? Hmm...

![]()

## Numbers
Get acquainted with your first data type. A data type represents the shape of the data the bits will create. The Number data type represents numeric values, written like 13. Using this in a computer program will cause a bit sequence to form a pattern for the number 13 in the computer's memory. JavaScript uses a fixed number of bits, precisely 64, to store a single number value. Imagine what you could do with 64 binary digits. Well, JavaScript can represent 264 different numbers. Could you guess how much that is? Roughly 18 quintillion. Yeah, that's an 18 with 18 zeroes after it. In translation, a lot. But there's a catch. One bit must represent the sign of the number, whether it's positive or negative. Also, non-whole numbers must be represented, they use some bits to store the position of the decimal point. So the actual real world max value in for a whole number is around 9 quadrillion. Care to guess how much that is? Yeah, still a lot.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-1/U5drZUZmRyaJPrBXG5xJ4cUeaFiz5La_1680x8400.jpg)

## Fractional numbers
These numbers are written with a dot. For example 9.81. For scientific calculations, even the e notation can be used. Like this 2.998e8. However, one important thing must be noted about fractional numbers. They are always approximations. Never, ever, can they be exactly precise. Every calculation with fractions, especially numbers with large fractions, must be treated as approximations. This is the main difference. While calculations with whole numbers up until 9 quadrillion are guaranteed to be precise.

## Strings
Enough about numbers and digits. Let's see how to represent text. Voilá, strings. A string is a data type which stores all textual input as a string of characters. These characters can be anything, a number, a letter, symbols, special characters, etc... They are all stored in strings, and strings are visually represented with quotes.

```
"The giraffe has a long neck."
'The cheetah can run fast.'
```

###

But strings have one downside. It's a bit difficult to put some characters in strings. Because a string needs to stay on one line, a newline character is hard to manage. Because of this strings have something called escape characters. They indicate some special function of the escaped character.

```
'First line\nSecond line'
```

###

This string will be visually represented as:

*First line*

*Second line*

When a string contains a backslash (\) it means the first character after the backslash denotes the special function, in the example above, the \n symbols a newline character.

![](https://raw.githubusercontent.com/adnanrahic/cdn/master/tjj-1/U5drka2LE93NQzpurpjWLK3qCW4CeZ3_1680x8400.jpg)

## Summary
You have just scratched the surface of computer science and programming. We covered basic computer memory and bits, and basic values. You now know what numbers and string are. Take a while to let these concepts sink in. Tune in next time, when I'll be writing about arithmetic and operators.

You can read the next lesson [here](https://steemit.com/programming/@adnanrahic/the-javascript-journey-2-arithmetic-and-operators).

___

*Hope you guys and girls had as much fun reading this article as I had writing it!*
*Drop an upvote if you liked it, share if you believe it will be of help to someone.*
*It means a lot to me.*

*Feel free to ask any questions you have in the comments below.*

