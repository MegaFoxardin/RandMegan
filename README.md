# RandMegan
### Version: 0.0.3.11
Before you read this, we suggest that you read the "LICENSE" file first.

## What is RandMegan?
RandMegan is a Python Random Package, that uses Cryptographically Secure Random Generator. RandMegan is purposed to be 
lightweight, and RandMegan is purposed for random functionalities, almost independent of Python's built-in Random Module.

## In Development Notice:
We would like to inform you that RandMegan is new, and RandMegan is in the Early Access phase of its development; 
RandMegan may sometimes contain bugs (some of the bugs can be awkward) and glitches. If you encounter any bugs and 
glitches, you can contact Foxy CS (Anonymous) via Email: "foxrobinleela@gmail.com" for inquiries about RandMegan.

## How do you use RandMegan?
There are a few functionalities we would cover for RandMegan, and it may not be limited to just the functionalities 
mentioned.

The first example we would cover is how to import it. Say, for example, you have the package, and your main Python 
file through mentioned paths:
```
.\\Project\\RandMegan
.\\Project\\Project.py
```
You want RandMegan to be imported through 'Project.py'. It can be as simple as using:
```
import RandMegan
#place your code here
```
It is simple, and you do not need to add some additional code to import RandMegan.

Another example is when you imported it, how can you use its random integer generator? It is also coded in our methods 
to make the code simple, and easy to use. Here are two examples of how to do it:
```
import RandMegan
print(RandMegan.intRandom(0, 10))
#Returns a random integer between 0 to 10. No errors would occur
```
```
import RandMegan
print(RandMegan.intRandomPlus(0, [1, 2, 3, 4, 5, 6]))
# Also returns a random integer, just a bit more complex than the other one. It uses the length of the List
# if you are a person who likes to be complicated with your code, you at least have the option to do so.
```
In retrospect, that is not all you can do with RandMegan; you also have a random boolean function. How you can use it 
is as follows:
```
import RandMegan
print(RandMegan.boolRandom())
# Returns either "True" or "False" at random.
```
In addition, we also have the Random Character selection for a string:
```
import RandMegan
print(RandMegan.stRandom("HI THERE!"))
# Selects a random character from a String.
```
Another addition is the Shuffle functionality, and this is beneficial for gamers who like card games:
```
import RandMegan
List = ["Ace_Of_Diamonds", "King_Of_Diamonds", "Joker"]
List = RandMegan.Shuffle(List)
# Cards are shuffled randomly, and the function uses a specific shuffle name. Can you figure out the name for 
# that type of Shuffle?
print(List)
```
In addition to the Choose Random functionality:
```
import RandMegan #Assuming you already did that.
List = ["Pac-Man", "Tetris", "Blackjack", "Space Invaders"]
print(RandMegan.chooseRandom(List)
# Select a Random index, to get the random value.
# The Choose Random functionality can work with any variable values in the list. However, using the non-plusified 
# variant is still possible to find the index, during the debugging method.
```
The Plusified variant of the Choose Random:
```
...
List = ["Pizza", "Chocolate", "Custard", "Pasta", "Poultry", "Beef", "Oxtail"]
Lima = RandMegan.choosePlusified(List)
#First shuffles the index, then chooses a random selection from the list. This can be beneficial if 
# you are looking for more of a complex selection at random.
print(Lima)
```
and the Random Bytes method:
```
...
print(RandMegan.RandomBytes(10))
#Returns 10 random byte (Machine Code) values and prints it out
```
In addition, we have the Integer Random Below functionality in one perspective:
```
from RandMegan import *
print(intRandomBelow(10))
# returns and prints a random integer on a range from 0 to 10
```
and the Random Hex in the other:
```
from RandMegan import *
print(RandomHex(10))
# returns and prints a random hex value of 20 digits.
```
We also have a Random URL Generator:
```
from RandMegan import *
print(RandUrlsafe(10))
# returns and prints a randomly generated URL of 10 bytes.
```
or if you want to use the plusified version, which returns between 1, and maximum amount of bytes,
in a Random URL Generator:
```
from RandMegan import *
print(RandUrlsafePlus(10))
# returns and prints a randomly generated URL of a random integer between 1 and 10 bytes.
```
In addition, we also have the randBitArray function:
```
from RandMegan import *
x = randBitArray(10)
# Creates a bit Array of 10 Bits at random values.
```
and the randBits function:
```
from RandMegan import *
x = randBits(10)
# Creates a string, containing 10 Bits at random values.
```
The two functionalities mentioned can possibly be useful, if you want to use Quantum Functionalities on the Crypto Side.

Not only do we have random functions in it, we also have the 
Negativify Function:
```
from RandMegan import *
C = Negativify(100)
# This returns -100 as its integer value
```
and the Power of Function:
```
from RandMegan import *
C = Power(2, 10)
# This returns 2 to the power of 10, which is 1024
```
Let's say for example, that you want to use the Negativify Function, with the Warnings and Errors Suppressed.
You can do so, and here is an example of how to do it:
```
from RandMegan import *
C = Negativify(0, True)
# Without the True value on the second parameter, the function will give you a Syntax Warning. In this example,
# The Syntax Warning is Suppressed from raising.
```

There is one thing to note: Let's say for example, you make a mistake in your code, by generating a random number. For example:
```
...
C = intRandom(20, 10)
# This causes an exception
```
The error Message would occur as follows:
```
...
(20 >= 10) The minimum value should not be higher nor equal to maximum value. 
Did you mean to use 'intRandom(10, 20)' instead?
```
Gladly, exceptions are there to guide you, in case you make a Syntax or Value Error. In this case,
you would have to recode the accident mentioned to as follows:
```
...
C = intRandom(10, 20)
# The fixed version of the one that caused an exception
```
In addition, there is a function called "Panic" if you want to raise either an error, or a warning, if something went wrong.
Here are two examples of how to use it:
```
from RandMegan import *
C = Negativify(-1)
if C > 1:
    Panic(ValueError(f"{C} is more than one. This should not happen."))
# Fortunately, with this example, the Panic function is not called.
```
```
from RandMegan import *
C = Negativify(-1)
if C == 1:
    Panic(ValueError(f"{C} is equal to one."))
# With this example, on the other hand, the Panic function is called.
```
We know that this is short information, but as mentioned, RandMegan is in the in-development phase, and we will be adding or rebalancing as we progress with the development of RandMegan.

We wish you all the best, and please, stay secure.
