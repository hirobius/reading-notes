# Chapter 10: Error Handling & Debugging

Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too.

---

## Order of Execution

The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

## Execution Contexts

Every Statement in a script lives in one of three execution contexts.

1. Global Context
2. Function Context
3. *Eval Context (Not shown in the book / NA at this time)*

---

Variable Scope

The first two execution contexts correspond with the notion of scope

1. Global Scope
   - if a variable is declared outside a function, it can be used anywhere because it has global scope.
   - when a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

---

## The Stack

The JavaScript Interpreter processes one line of code at a time. When a statement needs data from another function, it **stacks** / piles the new function on top of the current task. 

Once the new task has been performed, the Interpreter can go back to performing the task in hand. Each time a new item is added, it creates a new execution context.

## Execution Context & Hoisting

Each time a script enters a new execution context, there are 2 stages.

1. **Prepare**

- the new scope is created
- Variables, functions, and arguments are created
- The value of the `this` keyword is determined
  
1. **Execute**

- Now it can assign values to variables
- Reference functions and run their code
- Execute statements

*Understanding that these two phases happen helps
with understanding a concept called hoisting. You
may have seen that you can:*

- Call functions before they are declared
- assign a value to a variable that has not yet been declared

This is because any variables and functions within
each execution context are created before they are
executed.

The preparation phase is often described as taking
all of the variables and functions and hoisting them
to the top of the execution context.

Each execution context also creates its own
**variables object**. This object contains details of all
of the variables, functions, and parameters for that
execution context.

---

In the interpreter, each execution context has its own variables object.It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

Functions in JavaScript are said to have **lexical scope**:
*They are linked to the object they were defined within.*

If a variable is not found in the variables object for the current execution context, it can look in the variables object of the parent execution context. But it is worth knowing that looking further up the stack can affect performance, so ideally you create
variables inside the functions that use them.

Each time a function is called, it gets its own execution context and variables object.

---

## Understanding Errors

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. (page 480)

*If you are anticipating that something in your code
may cause an error, you can use a set of statements
to handle the error.*

When an exception is thrown, the interpreter searches through the current execution context and up the chain. So it is going through the stack looking for error-handling code until it gets to the global context. If there is still no error handler, the script stops running and the Error object is created.

## Error Objects

Error objects can help you find where your mistakes are
and browsers have tools to help you read them. They have the following properties: 

- name: Type of Execution
- message: Description
- fileNumber: Name of the JS file
- lineNumber: Line number of error

You can see all of this on the console.

---

### There are 7 types of built-in error objects in JavaScript 

#### SyntaxError

**Syntax is not correct.** This is caused by incorrect use of the rules of the language. It is often the result of a simple typo.

#### ReferenceError

**Variable does not exist.** This is caused by a variable that is not declared or is out of scope.

#### EvalError

**Incorrect use of** `eval()` **function.** Very rare. A Browser often throws other errors when it is supposed to throw this one. 

#### URIError

**Incorrect use of URI Functions.**
If these characters are not escaped in URls, they will
cause an error: / ? & I : ;

#### TypeError

**Value is unexpected data type.**
This is often caused by trying to use an object or
method that does not exist.

#### RangeError

**Number outside of range**
If you call a function using numbers outside of its
accepted range.

#### NaN

**Not an Error** / "Not a Number"

---

## How to deal with Errors

You can either **debug the script** or **handle errors gracefully.**

Sometimes, an error may occur in the script for a
reason beyond your control. In such cases, it is particularly
important to write error-handling code.

## Debugging Workflow

**Debugging is about deduction: eliminating potential causes of an error. Try to narrow down where the problem might be, then look for clues.**

### Where is the Error?

1. Look at the Error Message
2. Check how far the script is running
3. Use Breakpoints (pause execution) where things are going wrong

### What Exactly is the Problem?

Once you think that you might know the rough area
in which your problem is located, you can then try to
find the actual line of code that is causing the error.

When you have set breakpoints, you can see if the
variables around them have the values you would
expect them to. If not, look earlier in the script.

Break out parts of the code to test
smaller pieces of the functionality.

- Write values of variables into the console.
- Calrfunctions from the console to check if they
are returning what you would expect them to.
- Check if objects exist and have the methods I
properties that you think they do.
- Check the number of parameters for a function, or
the number of items in an array.

If the problem is hard to find, it is easy to lose track
of what you have and have not tested. Therefore,
when you start debugging, keep notes of what you
have tested and what the result was. No matter
how stressful the circumstances are, if you can,
stay calm and methodical, the problem will feel less
overwhelming and you will solve it faster.

## The JavaScript Console

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

When you are debugging errors, it can help if you
look at the error in more than one browser as they
can show you different error messages.

Note that **the line number does
not always indicate where the
error is. Rather, it is where the
interpreter noticed there was a
problem with the code.**

If the error stops JavaScript from
executing, the console will show
only one error - there may be
more to troubleshoot once this
error is fixed.

Browsers that have a console have a console object, which has severalmethods that your script can use to display data in the console. The object is documented in the Console API.

---

`console.group('Area calculations');
console.info('Width ', width);
console.info( 'Height ', height);
console.log(area); console.groupEnd();`

`console.table();` logs a table

`console. assert();` tests if a
condition is met, and writes to the
console only if the expression
evaluated to false.

---

## Stepping through Code: breakpoints

If you set multiple breakpoints, you can step
through them one-by-one to see where values
change and a problem might occur.

When you are doing this, if
the debugger comes across a
function, it will move onto the
next line after the function.
(It does not move to where
the function is defined.) This
behavior is sometimes called
stepping over a function.

## Conditional breakpoints

You can indicate that a breakpoint should be
triggered only if a condition that you specify is
met. The condition can use existing variables.

## Handling Exceptions

If you know your code might fail, use `try`, `catch`, and `finally`.
Each one is given its own code block.

You can nest checks inside each other (place another t ry inside a
catch), but be aware that it can affect performance of a script.

(Kind of complex, waiting til lecture to understang)

## Throwing Errors

If you know something might cause a problem for your script, you can
generate your own errors before the interpreter creates them.

To create your own error, you use the following line:
`throw new Error('message');`

Therefore, if you throw an error when the user enters
a value you cannot use, it prevents issues at some
other point in the code. You can create an error that
explains the problem, before the user gets further
into the script.

---

## Other Tips

- Use Another Browser
- Add Numbers
- Strip it Back / remove parts until it works
- Explaining the Code (talk it out to someone else)
- Search (Stack Overflow)
- Code Playgrounds (JSfiddle, Dabblet, JSBin, CSSDeck, CodePen)
- Validation tools!!! - jslint.com + jshint.com + jsonlint.com
- Jquery has a jquery debugger plugin for chrome

- If you know that you may get an error, you can handle
it gracefully using the **try**, **catch**, **finally** statements.
Use them to give your users helpful feedback.