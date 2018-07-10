

## Python Hacks. What every python coder should know

### Debugging
By and far, I have mentored and interacted with many people who code in python yet do not know how to debug.

#### pdb
I use pdb on a daily basis. It is one of the first debugging resources I learned about, and it is particularly useful for situations where you have a complex piece of code that is producing an error that is not readily identifiable. 
You can use pdb 4 ways:
1. Within Your Program
2. From the Command Line
2. Within the Interpreter
4. After a Failure

Below are pretty straight forward examples of each type.

##### Within your program
```
import pdb; 

def find_answer(number1, number2):
    return

pdb.set_trace()
```

[back](./)
