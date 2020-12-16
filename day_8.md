# day_8

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

# Comparison operators: 150-151

These **operators** actually compare 2 values and return a Boolean True of False:

1. ```==``` **"Is equal to" operator** to see if they both are the same.

2. ```!=``` **"Is not equal to"** to see if they are NOT the same.

3. ```===``` **"Strict Equal To"** to see if they are both the same data type and value

4. ```!==``` **"Strict Not Equal To"** to see if both the data type and value are not the same.

5. ```>``` **"Greater Than"** to check if the number on the left is *greater* than the number on the right.

6. ```<``` **"Less Than"** to check if # on the left is less than numer on right

7. ```>=``` **"Greater Than"** for greater than or equal to

8. ```<=``` **"Less Than"** for less than or equal to


When referring to testing / checking of a condition it is called ***evaluating*** a condition.

**Exceptions:**
Every value can be *treated* as true or false even if it is not a Boolean **true** or **false** value. Referred to later...

# Logical Operators: 156 & 157

Comparison operators usually return single values of **true** or **false**. Logical operators let you compare the RESULTS of more than one **comparison** operator.

***Example:*** ```((5 < 2>) && (2 >= 3))``` Which returns *false*.

1. ```&&``` **"Logical And"** to test MORE THAN ONE condition. If both expressions return true, then true if else: false

2. ```||``` **"Logical OR"** this operator tests AT LEAST ONE condition and if either condition ***evaluates*** to true, then true

3. ```!``` **"Logical Not"** this opertor takes a single boolean and inverts it: ```!true``` returns *false* ```!false``` returns *true*

### Short-circuit Evaluation
Basically this concept means that the ***evaluation*** can stop once a condition provides enough information to get the answer... *(If the first expression evaluates to false, then they both can't be true)*


# ```For``` and ```While``` loops: 170-173

Loops check a condition. If it returns **true** then a code block will run and continue to do so until the condition returns **false**

1. ```for``` loops are usually ran on a counter
2. ```while``` loops will continue for as long as the condition ***evaluates*** true
3. ```do while``` loops are similar to the while loop but has one difference: it will always run the statements inside the curly braces at least once, even if the condition evaluates to *false*.

```for``` example: ```for (var i = 0; i < 10; i++) {document.write(i);}``` which will result in "0123456789" being writen to the page

# Using ```while``` loops

***Example:***

``` 
var i = 1;
var msg = '';
while (i < 10) {
    msg += i + ' x 5 = ' + (i * 5) + '<br />';
    i++;
}