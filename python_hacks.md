

## Python Hacks 01. What every python coder should know ...

### Debugging
By and far, I have mentored and interacted with many people who code in python yet do not know how to debug. Below I discuss my best approaches to debugging code I have written, I would love to hear about different approaches you use!

#### pdb
I use pdb on a daily basis. It is one of the first debugging resources I learned about, and it is particularly useful for situations where you have a complex piece of code that is producing an error that is not readily identifiable. 

You can use pdb 4 ways:
1. After a failure
2. Within your program
3. From the command line
4. Within the interpreter
 

Below are pretty straight forward examples of each type with the example script myscript.py as follows:

```
import pdb
def divide(a, b):
    pdb.set_trace()
    return a / b
    
if __name__ == '__main__':
    divide(3,0)
```


##### After a failure
```
jessica$ ipython
Python 3.5.3 | packaged by conda-forge | (default, May 12 2017, 15:35:12)
Type 'copyright', 'credits' or 'license' for more information
IPython 6.1.0 -- An enhanced Interactive Python. Type '?' for help.

In [1]: import pdb

In [2]: def divide(a, b):
   ...:   return a / b
   ...:

In [3]: divide(3,0)
---------------------------------------------------------------------------
ZeroDivisionError                         Traceback (most recent call last)
<ipython-input-3-24bf8d716600> in <module>()
----> 1 divide(3,0)

<ipython-input-2-25fda7045bd1> in divide(a, b)
      1 def divide(a, b):
----> 2   return a / b

ZeroDivisionError: division by zero

In [4]: pdb.pm()
> <ipython-input-2-25fda7045bd1>(2)divide()
-> return a / b
```

##### From command line
```
jessica$ python -m pdb -c continue myscript.py
```

##### Within the interpreter
```
Jessica$ python
Python 3.5.3 | packaged by conda-forge | (default, May 12 2017, 15:35:12)
[GCC 4.2.1 Compatible Apple LLVM 6.1.0 (clang-602.0.53)] on darwin
Type "help", "copyright", "credits" or "license" for more information.

>>> import pdb
>>> import myscript
>>> pdb.run('divide(3,0)')
(Pdb)

```
##### Within your program

```
jessica$ python my_script.py
```

I hope these quick and easy examples give you insight to how to use pdb for your debugging needs. Questions, comments and suggestions are welcome. 

[back](./)
