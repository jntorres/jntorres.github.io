

## Python Hacks 01. What every python coder should know ...

### Debugging
By and far, I have mentored and interacted with many people who code in python yet do not know how to debug. Below I discuss my best approaches to debugging code I have written, I would love to hear about different approaches you use!

#### pdb
I use pdb on a daily basis. It is one of the first debugging resources I learned about, and it is particularly useful for situations where you have a complex piece of code that is producing an error that is not readily identifiable. 

You can use pdb 4 ways:
1. Within your program
2. From the command line
2. Within the interpreter
4. After a failure

Below are pretty straight forward examples of each type.

##### Within your program
```
import pdb; 

def find_answer(number1, number2):
    return

pdb.set_trace()
```
##### From command line
```
import pdb; 

def find_answer(number1, number2):
    return

pdb.set_trace()
```

##### Within the interpreter
```
import pdb; 

def find_answer(number1, number2):
    return

pdb.set_trace()
```
##### After a failure
```
import pdb; 

def find_answer(number1, number2):
    return

pdb.set_trace()
```
[back](./)
