# day_7

###### [day_1](day_1.md)
###### [day_2](day_2.md)
###### [day_3](day_3.md)
###### [day_4](day_4.md)
###### [day_5](day_5.md)
###### [day_6a](day_6a.md)
###### [day_6b](day_6b.md)
###### [day_7](day_7.md)
###### [day_8](day_8.md)

###### [MASTER_NOTES.md](MASTER_NOTES.md)

# Duckett: JavaScript & jQuery

# Intros + Scripts: pg 1-24

1. **Access Content:** You can use JavaScript to select any element, attribute or text from an HTML page.
2. **Modify Content:** You can use javascript to add elements, attributes and text to the page
3. **Program Rules:** You can specify a set of steps for the browser to follow, which allows it to access or change the content of the page.
4. **React to Events:** You can specify that a script should run when a specific event has occured.

JQuery will help you write scripts.
JQuery also helps you deal with cross-browser inconsistencies. 

Scripts can run different sections of the code in response to the situation around them.

>To write a script, you need to first state your goal and then list the tasks that need to be completed in order to achieve it.

A script may seem complicated, but it is simply a series of small steps.

1. Define the goal
2. Design the script
3. Code each step

**Vocabulary**: The words that computers understand
**Syntax**: How you put words together so a computer can follow them

###### Flowchart key

| **Generic step** | **Event** |
| ------ | ------ |
| **Input or output** | **Decision** |


## Expressions + Operators: pg 74-79

An **Expression** evaluates into (results in) a single value. Broadly speaking, there are 2 types of expressions.

1. Expressions that just assign a value to a variable
2. Expressions that use two or more values

"undefined" is a data type just like a number, string or Boolean. 

Expressions rely on **operators**. They allow programmers to create a single value from one or more values.

## Arithmetic operators

**Addition (+)** Adds one value to the other
**Substraction (-)** Subtracts one value from another
**Division (/)** Divides two values
**Multiplication (*)** Multiplies two values
**Increment (++)** Adds one to the current number
**Decrement (--)** Subtracts one from the current number
**Modulus (%)** Divides two values and returns the remainder

Don't forget PEMDAS for the order of operations.

In order to have an operation performed first, you will need to put the operation in parentheses, so: ```total = (2 + 4) * 10;``` 

To combine strings, you use the Addition operator. You cannot perform arithmetic on strings, makes sense.

## Functions: pg 88-94

Functions let you group a series of statements together to perform a specific task. *If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements)

When you ask it to perform its task, it is known as **calling** the funtion. 

The steps are packed into a code block.

Pieces of info passed to a function are known as **parameters**.

When you write a function and you expect it to provide you with an answer, the response is known as a **return value**.

*You can also have anonymous functions.* They do not have a name so they cannot be called, instead, they are executed as soon as the interpreter comes across them. 

To create a function, you give it a name and then write the statements needed to achieve its task inside the curly braces. This is known as **function declaration**.

1. You declare a **function** using the ```function``` keyword

2. You give the function a **name** (sometimes called an **identifier**) followed by parentheses: ```sayHello()```

3. Then the **statements** that perform the task sit in a code block: ```{document.write('Hello!');}```

## Calling a function

You can call the entire code block of a function with just one line of code! This is called **calling the function**.

## Declaring functions that need information

```function getArea(width, height) {return width * height;}```

## Calling functions that need information

When you call a function that has parameters, you specify the values it should use in the parentheses that follow its name. The values are called **arguments**, and they can be provided as values or as variables.

People often use the terms **parameter** and **argument** interchangeably, but they're slightly different...

When you are passing actual information that is needed for the function to calculate something, the values you insert are called **arguments**.

## Getting a single value out of a function

*Note that the interpreter leaves the function when **return** is used. It goes back to the statement that called it. If there had been any subsequent statements in this function, they would not be processed.*

(still kind of fuzzy on some stuff here and there, but onward and upward)