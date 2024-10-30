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

## 4. Indent your code for readability
Indenting your code makes it easier to read and helps you spot errors. When your code is indented correctly, it's easier to see the structure of your code and where each section begins and ends. This can be a helpful way to debug your code and find errors.

In JavaScript, the standard indentation is two spaces. In Python, the standard indentation is four spaces. In a language like Python, where indentation is significant, the wrong indentation can cause your code to break.

```
// Unindented code
function printHello() {
console.log("Hello, world!");
}
printHello();

// Indented code

function printHello() {
  console.log("Hello, world!");
}

printHello();
```
You should indent your code when you start a new block. A block is a section of code that is executed together. For example, a block can be a function, an if statement, or a for loop.

## 6. Use whitespace to improve readability
In addition to indenting your code, you can use whitespace to improve its readability. Adding extra spacing between lines of code will make your code easier to scan and understand. This is especially helpful when you are reviewing large blocks of code.

## 7. Use arrays and loops for efficiency

## 8. Write self-documenting code whenever possible
Self-documenting code is code that is easy to read and understand without the need for comments. This type of code is written in a way that makes its purpose clear.

There are many ways to make your code self-documenting. We've already covered some of them:
* Use clear and descriptive variable and function names
* Write short functions that do one thing and do it well
* Avoid magic numbers(numbers with no apparent meaning) by using named constants.
* Use whitespace to separate code into logical chunks
* Use clear and consistent coding conventions. This makes your code easier to read and understand, even for people unfamiliar with your codebase.

## 9. Don't repeat yourself (DRY)
Remember to avoid duplicating code whenever possible. Duplicated code is more challenging to maintain and more error-prone.

Many tools can be employed to avoid duplication in your code.
* Functions and modules.
  The function allows you to encapsulate code that you want to reuse.
* Data structures.
  Data structures can be used to store information in a way that is easy to access and modify.
* Inheritance.
  A more advanced way to avoid duplication is to use inheritance. Inheritance allows code to be shared between classes by having one class inherit from another.
* Libraries.
  You can avoid duplication by using tools and libraries. There are many open-source libraries that you can use to perform everyday tasks.

> [!TIP]
> Tips for writing DRY code
* Avoid repeating yourself by trying to reuse code where possible. If you know you'll be doing something again elsewhere in your code, you can write that code as a discrete entity the first time and avoid returning to refactor.
* When you reuse code, modularize it. Don't copy the solution to the new location. Instead, move it into the appropriate object or data structure type, then reference it.
* Refactor your code when you see a significant opportunity to benefit from rewriting it as DRY code. That means restructuring your code without changing its functionality. Refactoring can sometimes be a procrastination stop, but if you realize that you will need parts of a significant function again, it's worth doing it.
* Use libraries and frameworks to avoid reinventing the wheel. If you should refrain from repeating yourself, why should you write code to solve a problem that's already been solved?
* Follow the DRY principle when creating documentation - don't duplicate information unnecessarily.
* You can use explicit variable and function names and comment on your code where necessary.
  
Credit: https://www.sitepoint.com/how-to-write-good-code/#4usedatastructuresappropriately

