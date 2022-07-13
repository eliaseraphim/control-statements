#Control Statements  
Author: Elia Deppe  
Editor: <name here>  

## Section 1

### Algorithms

### Pseudocode

### Control Statements

Python provides three selection statements that execute code based on a condition that evaluates to either True and False.  
- The `if` statement performs an action if a condition is True or skips the actions if the conditon is false.
- The `if...else` statement ...
- The `if...elif...else` statement ...

Anywhere a single action can be placed, a group of actions can be placed. Python provides two **iteration statements** - `while` and `for`:
- The `while` statement ...
- The `for` statement ...

#### Keywords
The words above, `if`, `elif`, `else`, etc. are all keywords. Keywords are special commands, conditions, or values that are used in program execution.

| Python Keywords |       |          |       |          |
|-----------------|-------|----------|-------|----------|
| and             | as    | assert   | async | await    |
| break           | class | continue | def   | del      |
| elif            | else  | except   | False | finally  |
| for             | from  | global   | if    | import   |
| in              | is    | lambda   | None  | nonlocal |
| not             | or    | pass     | raise | return   |
| True            | try   | while    | with  | yield    |

#### if_else Statements

`if...else` Statements allow us to make ______ decisions based on the result of the _________.

Let's take a look:

```python
>>> name = 'elia'
>>> if name == 'elia':
...   print('hello elia')
... else:
...   print('user not recognized')
...
hello elia
```

We as people often rely on utilizing binary decision-making in order to accomplish a goal. Three examples of this:
1. First example...
2. Second example...
3. Third example...

##### Questions
Examine the following code segments and answer questions related to them.

###### Segment 1
```python
number = (45 - 15) / 2

if number % 2 == 0:
    print(number, 'is an even number')
else:
    print(number, 'is an odd number')
```

1. Which print statement will execute?
2. If `number` were a random integer, what would be the chances to get an even or odd number?

##### Coding
Complete the following code segments with notes.py according to the specifications.
1. Accept input in the form of a number from the user.
2. Determine if that number is divisible by 5 or not.
   1. If divisible print: x is divisible by 5
   2. Else: x is not divisible by 5

Question(s):
1. What is the probabilty the user will enter a number divisible by 5?

#### if_elif_else Statements

```python
>>> if x == 3:
...   print(x, 'is a single digit prime number')
... elif x == 5:
...   print(x, 'is a single digit prime number')
... elif x == 7:
...   print(x, 'is a single digit prime number')
... else:
...   print(x, 'is not a single digit prime number')
...
5 is a single digit prime number
```

##### Questions
1. How many elif statements can you use?
2. Do elif Statements require a condition?
3. When using if_elif_else, do you need an else Statement?

##### Coding
Complete the following code segments with notes.py according to the specifications.
1. Accept input from the user in the form of a string, requesting they enter the current weather.
   1. If the weather is sunny, inform the user to put on sunscreen.
   2. If the weather is cloudy, inform the user to keep an umbrella with them.
   3. If the weather is rainy, inform the user to keep an umbrella with them and use a raincoat.
   4. If the weather is cold, inform the user to wear a coat.

## Section 2

### while Loops

The **while statement** allows you to repeate one or more actions while a condition remains True.

```python
>>> x = 5
>>> while x < 15:
...   x = x + 3
...   print(x)
...
8
11
14
17
```

#### Questions
1. What might you use a while loop for?
   1. ...
2. What happens if you never modify x in the example above?
   1. ...

#### Coding
Complete the following code segments with notes.py according to the specifications.
1. Create a program that continually prompts the user to enter a word, and then prints it out to the user capitalized.
2. Is the user types `'quit'`, then after that word is outputted, exit the loop, and end the program.

### for Loops

The **for statement** allows you to repeat an action or several actions for each item in a sequence of items. This can be done using a sequence like a string.

```python
>>> for letter in 'cats':
...   print(letter)
...
c
a
t
s
```

Order of Operations (for above code segment):
1. ...
2. ...
3. ...
4. ...

Often times when using for Loops, we utilize the `range` function to run the for loop a set number of times.

```python
>>> for i in range(5):
...   print('i =', i)
...
i = 0
i = 1
i = 2
i = 3
i = 4
```

#### Questions
1. What does the function `range` return? It is a sequence?
   1. ...
2. Why might you use a `for` loop?
   1. ...
3. Give an example of where you might use a `for` loop instead of a `while` loop, and why.
   1. ...
4. Give an example of where you might use a `while` loop instead of a `for` loop, and why.
   1. ...

#### Coding
Complete the following code segments with notes1.py according to the specifications. 
- Create a program that calculates the average of a set number of numbers.
  - You should prompt the user to enter the number of numbers that you will be calculating.
  - Within a loop, capture those numbers inputted by the number.
  - At the end of the loop, output the average of the numbers entered by the user.

### Augmented Assignments

**Augmented assignments** abbreviate expressions in which the same variable name appears on the left and right of the assignment's =.

An expression like `x = x + 5` can be shortened by using a matching expression `x += 5`.

Assuming c = 3, d= 5, e = 4, f = 2, g = 9, h = 12

| Augmented Assignment | Sample Expression | Explanation | Assigns  |
|----------------------|-------------------|-------------|----------|
| +=                   | c += 7            | c = c + 7   | 10 to c  |
| -=                   | d -= 4            | d = d - 4   | 1 to d   |
| *=                   | e *= 5            | e = e * 5   | 20 to e  |
| **=                  | f **= 3           | f = f ** 3  | 8 to f   |
| /=                   | g /= 2            | g = g / 2   | 4.5 to g |
| //=                  | g // = 2          | g = g // 2  | 4 to g   |
| %=                   | h %= 9            | h = h % 9   | 3 to h   |

#### Questions
1. Why might you use augmented assignments?
   1. ...
2. Do you find augmented assignments easier to understand?
   1. ...

#### Coding
Complete the following code segments with notes.py according to the specifications.
- Develop a program that continually accepts input from the user in the form of a number, and exits once the sum of those numbers is greater than 300.
  - Use augmented assignments to capture the sum of each number entered by the user, while within a while loop.

### Sentinel-Controlled Iteration

Sentinel-Controlled Iteration is a form of iteration in which you use what is known as a _sentinel_, a special variable that holds a value important to the continuation of the iteration. If the sentinel variable hols a certain value, then iteration should stop or continue based on that value. Typically sentinel-controlled iteration is used with `while` Loops.

Problem: Develop a class-averaging program that process an arbitrary number of grades each time the program executes.  

```python
"""Class average program with sentinel-controller iteration."""

# initialization
total = 0  # sum of grades
grade_counter = 0  # number of grades

# processing
grade = int(input('Enter grade, -1 to end: '))

while grade != -1:
   total += grade
   grade_counter += 1
   grade = int(input('Enter grade, 1 to end: '))

# termination
if grade_counter != 0:
   average = total / grade_counter
   print('Class average is', average)
else:
    print('No grades entered')
```

#### Questions
1. Why might you use sentinel-controlled iteration?
   1. ...
2. Can you use sentinel-controlled iteration with for Loops? Why or why not?
   1. ...

#### Coding
Complete the following code segments with notes.py according to the specifications.
- Develop a program that continually accepts input from the user in the form of a string, and exits the program upon a '.' being entered.
  - For every string entered, connect said string with all other previous strings, and output the result at the end.
  - See below for an example:

```
>> hello 
>> my friend! 
>> where do we go now
>> .

hello my friend! where do we go now.
```

### Built-In Function `range` - A Deeper Look

The range function can be modified to run from a different starting point or utilize a different step. The variations of range are as follows:
1. `range(stop)`
2. `...`
3. `...`

#### start, stop
```python
>>> for i in range(-5, 5):
...   print('i =', i)
...
i = -5
i = -4
i = -3
i = -2
i = -1
i = 0
i = 1
i = 2
i = 3
i = 4
```

#### start, stop, step
```python
>>> for i in range(-5, 5, 2):
...   print('i =', i)
...
i = -5
i = -3
i = -1
i = 1
i = 3
```

##### Questions
1. Why might you use the (start, stop) variation of `range`?
2. Why might you use the (start, stop, step) variation of `range`?

##### Coding
Complete the following code segments with notes.py according to the specifications.
1. Create a for loop that prints the numbers -10 through 20 with a step of 1.
2. Create a for loop that prints the numbers -100 through -50 with a step of 5.
3. Create a for loop that prints the numbers -10 through -20 with a step of -2.

### Boolean Operators `and`, `or`, and `not`

Currently, we can only test one condition at a time in conditional expressions. However, we are allowed to chain conditionals together using the following boolean operators. These boolean operators will modify the expression based on the following logic.

#### `and`
| expression 1 | expression 2 | expression 1 and expression 2 |
|--------------|--------------|-------------------------------|
| False        | False        | False                         |
| False        | True         | False                         |
| True         | False        | False                         |
| True         | True         | True                          |

`and` ensures both conditions on either side are True.

#### `or`
| expression 1 | expression 2 | expression 1 or expression 2 |
|--------------|--------------|------------------------------|
| False        | False        | False                        |
| False        | True         | True                         |
| True         | False        | True                         |
| True         | True         | True                         |

`or` ensures at least one conditions on either side are True.

#### `not`
| expression | not expression |
|------------|----------------|
| False      | True           |
| True       | False          |

`not` is utilized with one conditional expression, and negates that expressions value.

#### Questions
1. Why might you use these relational operators?
2. Can you think of a real life situation in which you use these operators?
   1. and ->
   2. or ->
   3. not ->

#### Coding
Complete the following code segments with notes.py according to the specifications.
- Develop a program that continually accepts input from the user in the form of a number, and exits the program upon a 0 being entered.
  - For every number entered make a decision to do one of the following:
    - If the number is odd and greater than 25, then output "High Odd"
    - If the number is even and less than 45, then output "Low Even"
    - If the number is not divisible by, then output "Indivisible by 5"

