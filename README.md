# write-good-code
> "Clean code always looks like it was written by someone who cares." — Robert C. Martin

## 1. Start with a plan

Please think about what you'd like your code to do. Do not jump into writing code because you think you know what needs to be done. Take some time to understand the problem at hand.

* What are the inputs and outputs?
* What are the expected results?
* What are the steps involved in getting from one to the other?
* What data structures will you need?
* Are there any edge cases that need to be considered?

Answering these questions before coding can help you avoid getting lost in rabbit holes for hours or days. It also allows you to solidify your mental conceptualization of how the project will work, validate it against any clear leaps of magical thinking, and develop a set of test cases to check your work against as you go.

> [!TIP]
> Tips for developing a high-level plan

Develop a clear **understanding of the problem** you are trying to solve.

Before you start coding, take some time to **think about what you want your code to do** to solve that problem.

**Write pseudocode** before you start coding. Presudocode is code that has yet to be quite real. It helps sketch out the structure of your code without getting bogged down in the details.

**Draw a diagram**

Visualizing the problem can help you better understand what needs to be done and how the different pieces fit together.

**Check your work**

Once you have a plan, check it against any clear leaps of magical thinking to ensure it's feasible.

**Use inline comments** to explain your thought process

Once you write your code, include inline comments explaining your actions and why. These comments can be constructive when you or someone else returns to the code later.

## 2. Write meaningful variable and function name
* Use descriptive names; the name of a variable or function should describe its purpose.
* Avoid single-letter names unless the meaning is very clear from the context. For example, using i as an index in a for loop is usually okay because that's a standard convention.
* Avoid magic numbers: Magic numbers are numeric literals used in code without explaining their meaning.
* Decide on a naming convention: Then stick to it.
* Comment your code: When an explicit name is insufficient, and you need to review the original function or variable, you can quickly refresh your memory.

When you are picking names for things, ask yourself the following questions:
* What is this variable or function for?
* Does its name describe its purpose?
* Is it easy to remember when I pronounce it?
* Is it consistent with the other names in the code?

## 3. Write small, modular functions
Functions are among the most powerful tools in a programmer's toolbox. They allow you to break down a significant problem into smaller, more manageable pieces.

Small functions are easier to test, more accessible to debug, and easier to reuse. They also make your code more readable because the purpose of each function is straightforward.

> [!TIP]
> Tips for writing modular functions

* Keep function small by giving them a single responsibility
  When you write a function, please think about what it's supposed to do and only have it do that.
* Name your function descriptively
  The function name should be clear and descriptive so you can easily understand what they do when reading the code.
* Avoid side effects
  The function that has a side effect if it modifies something outside of its scope. For example, a function that takes an array as an argument and sorts the array would be considered to have a side effect. It can be challenging to avoid side effects all the time, but it's something to keep in mind when writing functions.
* Use arguments wisely
  When including arguments into a function, think about whether they are vital. Arguments are often used to make functions more flexible, but too many arguments can make them challenging to understand.

## 4. Use data structures appropriately
Data structures are ways of organizing data to be used efficiently. There are many types of data structures, but some of the most common are arrays and objects.

Arrays are lists of data. They can store any data type, but each item must have the same type. Arrays are declared using square brackets.

Objects are collections of data organized using key-value pairs. The keys access the values, which can be any data type. Objects are declared using curly braces.

## 5. Comment your code liberally
Comments are a great way to improve the readability of your code. You can use comments to explain what your code is doing and why you are doing it.

One standard convention is to use TODO comments to leave notes for yourself about things that need to be done:

```
// TODO: Implement login functionality
```

Another standard convention is to use FIXME comments to leave notes for yourself about things that need to be fixed:

```
// FIXME: This code is not working properly
```

It's important to remember that comments should improve the readability of your code, not make it more difficult to understand. If you find yourself writing a comment longer than the code it is commenting on, that is a sign that your code needs to be readable and should be refactored.

> [!TIP]
> Tips for commenting code
* Use comments to explain what your code is doing and why you are doing it
* Use comments to leave notes for yourself about things that need to be done or fixed.
* Use comments to explain complex or non-obvious code.
* Use comments to enhance readable code, not as a crutch.
* Comment on your code as you write it, and don't wait until later.
* Don't over-comment your code. Only comment on the parts that need explanation.
* Use clear and concise language in your comments
* Avoid using acronyms
* Keep your comments up-to-date with your code. If you change your code, change your comments.
* Delete obsolete comments 
  
Credit: https://www.sitepoint.com/how-to-write-good-code/#4usedatastructuresappropriately

