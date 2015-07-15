---
tags: cssi, basic python, conditional statements, booleans
level: 1
languages: python
---
#Python Conditional Statements

#Objectives:

+ Understand the syntax of conditional statements
+ Use conditional statements
+ Understand what a boolean is

#Motivation
Sometimes we only want our code to run if certain conditions are in place. If a condition is met, then python should run the code otherwise something else should happen.

#Conditionals
Conditional statements are a type of control flow: They can control which parts of code get executed, and which do not. The basic conditional statement is the if statement:
```
if condition_1:
    run this block of code
```
Here is an example with two variables:
```
yourAnimal = input('What is your favorite animal? ')
myAnimal = "dog"

if yourAnimal == myAnimal:
  print "That's my favorite animal, too!"
```
#Comparison Operator
  + "==" means "are these two things equal?".
  + "=", means assignment - you're setting a variable equal to a value.

#Boolean Values
False and True are special values called **booleans**. Booleans can be assigned to variables.
For example:
```
x = (3 == 5)
print x
```
First, we calculate (3 == 5). This is a question: "Is 3 equal to 5?". The answer to that question is False: 3 is not equal to 5.

So, when we say x = (3==5), this is equivalent to x = False. We're setting X to the boolean value False. Now, when we print x, we just print out False.

Here are some important boolean operators:
<img src= "images/boolean_table.png">

#Else and Elif conditional statements
There are a few other conditional statements that work together with if. For example, you often want to do something if the condition failed:
```
yourAnimal = input('What is your favorite animal? ')
myAnimal = "dog"
if yourAnimal == myAnimal:
  print "That's my favorite animal, too!"
else:
  print "I don't think you understand how cool dogs are."
```
An "else" clause should always follow an "if" clause, because "else" means "otherwise."
You wouldn't ever start a conversation with "Otherwise, do this!", so it doesn't make sense to start with an else, when there's not an if right before it.

There's also "elif".  It's an "else" and "if" glued together - if the first thing works, do that; otherwise, try the second condition; else...
```
if x > 500:
  print "x is really big"
elif x > 50:
  print "x is sort of big"
elif x < 0:
  print "x is negative!"
else:
  print "x is not very interesting"
```
#Student Practice
In your practice.py try writing a conditional statement with an if condition, elsif condition and else condition

 * **Pick a Number:** Write a program that makes the user guess a number 1-10. If their guess is correct, tell them they've won. If their guess is too high or too low, give the user a hint. you will need to use python's `input()` method.
  * `userGuess = input('Guess a number between 1-10')`
