# ch. 3 Lists 62-73

### Unordered, Ordered & Definition Lists

Definition lists are made up of a set of terms along with the
definitions for each of those terms.

'''<dt>''' This is used to contain the term being defined
'''<dd>''' This is used to contain the definition


# ch. 13 Boxes 300-329

### Borders


###### Stuff I didn't know

border-top-width
border-right-width
border-bottom-width
border-left-width

thin, medium, thick

border-top-style
border-left-style
border-right-style
border-bottom-style

border: 3px dotted #0088dd;

visibility: hidden;

border-image: url("images/dots.gif")


# JS Review p. 70-73

An Array is a special type of variable that actually stores a list of values.
Each item in an array is assigned a number called an **index**.
Each array has a property called **Length**.
The name of the array is followed by a period symbol, which is then followed by the length keyword.

# Chapter 4 p. 162-182

if ... else statements allow you to provide two sets of code:
1 set if the condition evaluates to true
1 set if the condition evaluates to false


### Switch Statements

A switch statement starts with a variable called the **switch value**. Pretty much, each case indicates a possible value for this variable and code that should run if the variable matches that value:


'''
switch (level) {
  case 'One ':
  title= 'Level 1 ' ;
  break;
case 'Two':
  tit1e = ' Level 2 ' ;
  break;
case 'Three':
  title = 'Level 3' ;
  break ;
default:
  title= 'Test';
  break;
}
'''

###### If else vs. Switch

With a series of If statements, they are all checked even if a solution is found. 
With a Switch, it is more efficient because the **break** statement stops the rest of the switch from executing, making it more efficient than a series of ifs.

### Fun Fact:

"Zero" written as a string is Truthy. The very presence of an object or array can
be considered truthy.

Although NaN is considered falsy, it is not equivalent to anything... not even to itself.

Logical operators are processed left to right.
They short-circuit (stop) as soon as they have a
result - but they return the value that stopped
the processing (not necessarily true or false). So whatever returns true first will proc the interpreter to run the subsequent code in the code block:

'''
var valueA = 0;
var valueB = 1;
var valueC = 2;

if (valueA || valueB || valueC) {
  // do something here
}
'''

Which


### Loops

review your 102 notes, but in summary:

Conditional statements allow your code to make decisions about what to do next.
Comparison Operators are used to compare two operands
Logical Operators allow you to combine more than one set of comparison operators
If...else statements allow you to run one set of code if a condition is true and another if false.
Data Types can be coerced from one type to another.
All values evaluate to either truthy or falsy.
There are three types of loops: For, While and Do...While. Each represents a set of statements.