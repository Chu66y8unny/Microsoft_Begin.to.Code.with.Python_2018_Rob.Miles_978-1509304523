# About the authoer

<www.robmiles.com>

**wacky**

# Introduction

<https://aka.ms/BeginCodePython/downloads>

-   Mobile phone or tablet  
    -   Pythonista for iOS
    -   Pyonic Python 3 interpreter for Android
-   Raspberry Pi  
    the Raspbian operating system has Python 3.6 and the IDLE built in

<https://aka.ms/BegintoCodePython/errata>

<https://aka.ms/mspressfree>

# Part 1 Programming fundamentals

# 1 Starting with Python

<www.begintocodewithpython.com/tools/>

<https://github.com/Begintocodewithpython/samples>

```python
>>> import this   # Philosophy of Python
```

**chatty**

# 2 Python and programming

**handoff**

*functional design specification*

*prototyping*

**backer**

**grunts**

**anthem**

**innocuous**

Multiplying a string by zero or negative number gives an empty string.

-   `ord`
-   `chr`
-   `bin`

# 3 Python program structure

-   `print`
-   `input`

**incessant**

To stop IDLE from repeatedly asking you the question to save after each edit:
-   On a Windows PC, click the **Options** and select **Configure IDLE**
-   On a Mac, click **Preferences**
Then move to the **General** tab in the dialog and select the *No Prompt**
option in the **Autosave Preferences**.

If you want to check the syntax of your program without running it, you can use
the **Check Module** option from the **Run** menu in the IDLE editor.

```python
import random
print('You have rolled:', random.randint(1, 6))
```

```python
import time
time.sleep(5)
```

To install `pygame`:
-   In **Windows PowerShell**, run `py -m pip install pygame --user`
-   In a terminal, run `python3 -m pip install pygame --user`

<http://www.pygame.org/wiki/GettingStarted>

# 4 Working with variables

<https://www.python.org/dev/peps/pep-0008/#naming-conventions>

Within Python programs, the end of a line of text is always marked by a single
new line character. The underlying operating system might work differently, for
example the Windows operating system uses the sequence `\r\n` (a return
followed by a new line feed) to mark the end of each line of text in a file.
The Python system performs automatic translation of line endings to match the
computer system being used, so our programs can always use a single new line
character to mark the end of a line.

-   Python 3.6 uses `input`
-   Python 2.7 uses `raw_input`

-   Python 3.6 uses `eval`
-   Python 2.7 uses `input`

-   `int`
-   `float`

The Python print routine “rounds” values when it prints them. In other words,
it says that if the number to be printed is 0.10000000000000000551115 or
thereabouts (which it is), then it will just print 0.1.

-   `1/2` produces `0.5` in Python 3.6
-   `1/2` produces `0` in Python 2.7

You can get a Python 2 program to behave the same way as Python 3 by telling it
to use the updated division routines:
```python
from __future__ import division
```
You could give this command at the start of a program to make Python 2 division
behave the same as Python 3 division.

# 7 Using functions to simplify programs

```python
def print_times_table(times_value):
    if not isinstance(times_value, int):
        raise Exception('print_times_table only works with integers')
    count = 1
    while count < 13:
        result = times_value * count
        print(count, 'times', times_value, 'equals', result)
        count = count + 1

print_times_table('six')
```

```python
import time

def teletype_print(text, delay=0.1):
    for ch in text:
        print(ch, end='')
        time.sleep(delay)
```

```python
cheese = 99

def func():
    global cheese
    cheese = 100
    print('Global cheese is:', cheese)

func()
print('Global cheese is', cheese)
```

# 8 Storing collections of data

**fizzy** drink

```python
import os.path
if os.path.isfile('text.txt'):
    print('The file exists')
```

```python
try:
    output_file = open(file_name, 'w'):
    for sale in sales:
        output_file.write(str(sale) + '\n')
except:
    print('Something went wrong writing the file')
finally:
    output_file.close()
```

**tidy up**

I **dread** getting the message that my program sometimes goes wrong.

```python
try:
    with open(file_name, 'w') as output_file:
        for sale in sales:
            output_file.write(str(sale) + '\n')
except:
    print('Something went wrong writing the file')
```

**splatter**

**ponder**

# Part 2 Advanced programming

# 9 Use classes to store data

the customer might decide that they want the program **there and then**

