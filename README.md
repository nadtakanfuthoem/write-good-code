# write-good-code
> "Clean code always looks like it was written by someone who cares." — Robert C. Martin

## 1. Start with a plan

Think about what you want your code to do. Don't jump into writing code because you think you know what needs to be done. Take some time to understand the problem at hand.

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

**Write pseudocode** before you start coding. Presudocode is code that is not quite real yet. It helps sketch out the structure of your code without getting bogged down in the details.

**Draw a diagram**

Visualizing the problem can help you better understand what needs to be done and how the different pieces fit together.

**Check your work**

Once you have a plan, check it against any clear leaps of magical thinking to ensure it's feasible.

**Use inline comments** to explain your thought process

Once you write your code, include inline comments explaining your actions and why. These comments can be constructive when you or someone else returns to the code later.

Credit: https://www.sitepoint.com/how-to-write-good-code/#4usedatastructuresappropriately

## 2. Write meaningful variable and function name
* Use descriptive names: The name of a variable or function should describe its purpose.
* Avoid single letter name: Unless the meaning is very clear from the context. For example, it's usually okay to use i as an index in a for loop, because that's a common convention.
* Avoid magic number: A magic number is a numeric literal that's used in the code without clear explaination of its meaning.
* Decide on a naming convention: Then stick to it.
* Comment your code: When a clear name is not enough and you do need to review the original function or variable, you will be able to refresh your memory quickly.