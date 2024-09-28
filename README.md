# RandMegan
### Version: 0.0.4.1
Before you read this, we suggest that you read the "LICENSE" file first.

## What is RandMegan?
RandMegan is a Python Random Package, that is a MêgaTron Random Generator. RandMegan is purposed to be
lightweight, and RandMegan is purposed for random functionalities, independent of Python's built-in Secrets Module.

## Notice:
We would like to inform you that RandMegan is new; Even though RandMegan is outside its Early Access phase,
RandMegan may sometimes contain bugs (some of the bugs can be awkward) and glitches. If you encounter any bugs and
glitches, you can contact Foxy CS (Anonymous) via Email: "foxrobinleela@gmail.com" for inquiries about RandMegan.

## How Much Storage do you require for RandMegan?
Now some people may ponder of how much storage, RandMegan requires, and you might be surprised, for it does not require
much storage. Storage Requirements are as follows, but not limited to:
- (Binary Format) Approximately 42.83 MB
- (Decimal Format) 46.5 MB

## What version of Python is required at minimum for RandMegan?
Now some people may or may not ponder on what Python Version does RandMegan require, which is understandable,
for some companies sticks to one version, and other companies keep their versions up-to-date. In this case
RandMegan requires a Python Version of, but not limited to:
- Python 3.12+

## What is a MêgaTron Random Generator?
MêgaTron Random Generator (MTRNG) is a Random Generator that its primary return strategy is based on Natural Phenomena,
which is the same return strategy as a Cryptographically Secure Random Generator (CSPRNG), which is unpredictable. If a
MêgaTron Random Generator noticed the Cryptography is exhausted, its second layer take over, and that goes towards a
backup Random Generator; The Operating System Entropy Random Generator (URNG or TRNG) is dependent on the Operating
System and hardware for true randomness. If the device got exhausted with its Entropy, then the third layer is its
last attempt before it is truly exhausted, and that is the Pseudo Random Generator (Either the Mersene Twister, or
Uniformly Distributed Random Generator) This makes MegaTron Random Generator have three (3) plans, to make sure that
it is highly stable from being exhausted.

Is MêgaTron Random Generator Stable? Yes, its process of randomness is just a bit slower.
Is MêgaTron Random Generator Cryptographically secure? Yes, it is.
Is MêgaTron Random Generator a True Random Generator? As long as the Cryptographic seeding does not have a mechanical
breakdown, then yes.
Why is MêgaTron Random Generator advised to use if performance is not your problem? Say for example its first layer gives
problems, then the second layer onwards is where the issues can escalate. The OS Entropy for Randomness relies on
hardware and Complex Entropies for True Randomness. However, it is rare for it to bring the backup plan.
Due to MTRNG being a very recent Random Generator, the information about it is still very recent, and the
cryptographers do not know much about it.
What Purposes are MêgaTron Random Generator useful for? There are a few it can be quite useful for:
- Game Development
- Cryptographic Random Generations
- Dice Rolls
- Low to Medium Security Required Development
- Crypto Mining (Even though, I would not recommend it, because Crypto Mining can be risky)
- Cryptographic Algorithms for Game Development purposes
- Chess Engines that works on random openings (For example, Leela Chess Zero)
- Disco Displays
- Card Games

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
# Returns a random integer between 0 to 10. No errors would occur

x = RandMegan.intRandom()
# Uses the Default Max Value to return a random integer of between 1 to 256.

y = RandMegan.intRandom(-128)
# Uses the Default Max Value to return a random integer of between -128 to 256.
```
```
import RandMegan
print(RandMegan.intRandomPlus(0, [1, 2, 3, 4, 5, 6]))
# Also returns a random integer, just a bit more complex than the other one. It uses the length of the List
# if you are a person who likes to be complicated with your code, you at least have the option to do so.

X = RandMegan.intRandomPlus()
# Uses the Default Max Value to return a random integer of between 1 to 256.
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
List = ["Ace_Of_Diamonds", "King_Of_Diamonds", "Joker", "Ace_Of_Spades", "King_of_Clubs", "Seven_Of_Diamonds", "Two_Of_Clubs"]
List = RandMegan.Shuffle(List)
# Cards are shuffled randomly.
# Just do note: The more bigger the list, the bigger the deck is to shuffle. If you have a whole shoebox to shuffle,
# then do expect for MTRNG's Randomness to be much more potent, than four decks of cards.

List2 = RandMegan.Shuffle()
# Uses the Default Entropy to create a list of 128 integer values, and then returns a shuffled version of it
print(List)
```
In addition to the Choose Random functionality:
```
import RandMegan #Assuming you already did that.
List = ["Pac-Man", "Tetris", "Blackjack", "Space Invaders"]
print(RandMegan.chooseRandom(List)
# Select a Random index, to get the random value.
# The Choose Random functionality can work with any variable values in the list. However, using the non-plusified 
# variant is still possible to find the index, during the debugging method, for it does not shuffle the list,
# before selecting one.
```
The Plusified variant of the Choose Random:
```
...
List = [_ for _ in range(50000)]
# This is where an interesting part will start. If you have a big list, it can go to the next level, because it
# can cryptographically be less limited in shuffling and choosing. Let's take it to its powerful randomness,
# shall we?
Lima = RandMegan.choosePlusified(List)
# First shuffles the index, then chooses a random selection from the list. This can be beneficial if 
# you are looking for more of a complex selection at random. Since it is like 200 decks, it might take about a second.
print(Lima)
```
and the Random Bytes method:
```
...
print(RandMegan.RandomBytes(10))
# Returns 10 random byte (Machine Code) values and prints it out

x = RandMegan.RandomBytes()
# uses the Default Max Value to return 256 random bytes
```
In addition, we have the Integer Random Below functionality in one perspective:
```
from RandMegan import *
print(intRandomBelow(10))
# returns and prints a random integer on a range from 0 to 9

x = intRandomBelow()
# uses the Default Entropy to return a random integer on a range from 0 to 127.
```
and the Random Hex in the other:
```
from RandMegan import *
print(RandomHex(10))
# returns and prints a random hex value of 20 digits.

x = RandomHex()
# Uses the Default Entropy to return 256 digits of a random hex value.
```
We also have a Random URL Generator:
```
from RandMegan import *
print(RandUrlsafe(10))
# returns and prints a randomly generated URL of 10 bytes.

x = RandUrlsafe()
# Uses the Default Entropy to generate a random URL of 128 bytes.
```
or if you want to use the plusified version, which returns between 1, and maximum amount of bytes,
in a Random URL Generator:
```
from RandMegan import *
print(RandUrlsafePlus(10))
# returns and prints a randomly generated URL of a random integer between 1 and 10 bytes.

x = RandUrlsafePlus()
# Uses the Default Max Value to return a range, of randomly between 1 and 256 bytes of a randomly generated URL
```
In addition, we also have the randBitArray function:
```
from RandMegan import *
x = randBitArray(10)
# Creates a bit Array of 10 Bits at random values.

xx = randBitArray()
# Uses the Default Max Value to return an array of 256 Bits at random values.
```
and the randBits function:
```
from RandMegan import *
x = randBits(10)
# Creates a string, containing 10 Bits at random values.

xx = randBits()
# Uses the Default Max Value to return a String, containing 256 Bits at random values.

y = randBytesPlus(12)
# Returns 12 random bytes (Ranging from 0 bit to 8 bits), into machine code, by encoding the bit string into a buffed 
# string, and then converting it into bytes.
# This also has a possibility for smaller sized bytes, making it variable on the MTRNG method.

y = randBytesPlus()
# Uses the Default Max Value (256) amount of bytes, and turn it into machine code, as how we stated with the previous 
# variable.
```
The four functionalities mentioned can possibly be useful, depending on what you need it for.

In addition, we also have the method to generate a random password for you:
```
from RandMegan import *
x = TokenPassword(16)
# Generates a 16 Character password, using cryptographic algorithms.

XXX = TokenPassword(ExcludeSpecialCharacters=False)
# Uses the Default Max Value to generate a 256 Character Password, while excluding special characters.

XX = TokenPassword()
# Uses the Default Max Value to generate a 256 Character Password.

print(x)
print(XX)
print(XXX)
```

Now, some people may or may not ponder, "What about the people who play Roleplaying Games that use Dice, and they
do not have Dice in stock?" We do have a few functions for that to make it easier for them, especially in such a
situation, so you're in luck here. Here is an example of how to use them:
```
from RandMegan import *

Player1_Dice = RandDice4()
# Rolls the Dice value, randomly between 1 and 4
Player1_Dice = RandDice4(4)
# Rolls the Dice value, randomly between 4 and 16. This is if you have multiple dices to roll

Player2_Dice = RandDice6()
# Rolls the Dice value, randomly between 1 and 6
Player2_Dice = RandDice6(4)
# Rolls the Dice value, randomly between 4 and 24. This is if you have multiple dices to roll

Player3_Dice = RandDice8()
# Rolls the Dice value, randomly between 1 and 8
Player3_Dice = RandDice8(5)
# Rolls the Dice value, randomly between 5 and 40.

Player4_Dice = RandDice10()
# Rolls the Dice value, randomly between 1 and 10
Player4_Dice = RandDice10(10)
# Rolls the Dice value, randomly between 10 and 100.

Player5_Dice = RandDice12()
# Rolls the Dice value, randomly between 1 and 12
Player5_Dice = RandDice12(10)
# Rolls the Dice value, randomly between 10 and 144.

Player6_Dice = RandDice16()
# Rolls the Dice value, randomly between 1 and 16
Player6_Dice = RandDice16(20)
# Rolls the Dice value, randomly between 20 and 320.

Player7_Dice = RandDice20()
# Rolls the Dice value, randomly between 1 and 20
Player7_Dice = RandDice20(100)
# Rolls the Dice value, randomly between 100 and 2000. (Do you have big hands?)

Player8_Dice = RandDice24()
# Rolls the Dice value, randomly between 1 and 24

Player9_Dice = RandDice28()
# Rolls the Dice value, randomly between 1 and 28

Player10_Dice = RandDice32()
# Rolls the Dice value, randomly between 1 and 32

Player11_Dice = RandDice36()
# Rolls the Dice value, randomly between 1 and 36

# Take note that those are functions, not classes
```

As with Pygame Developers, if you want a completely random colour, there is a function to use, and that can
generate a tuple of 3 colour values, in a Red-Green-Blue (RGB) format. Here is an example to use it:
```
from RandMegan import *

x = RandColour()
# Generates a random colour tuple of each value randomly between 0 to 255.

X = RandColour(25, 99)
# Generates a random colour tuple of each value randomly between 25 to 99.
```

Looking for a Random Colour for TKinter to use? We also have that added in. Here is an example of how it works:
```
from RandMegan import *

x = RandTKColour()
# Generates a random hex of a colour for TKinter to be able to use.

```

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

There is another thing to note: Let's say for example, you make a mistake in your code, by generating a random number. For example:
```
...
C = intRandom(20, 10)
# This causes an exception
```
The error message would occur as follows:
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
In addition, there is a function called "Panic" if you want to raise either an error or a warning, if something went
wrong. Here are two examples of how to use it:
```
from RandMegan import *
C = Negativify(-1)
if C > 1:
    Panic(ValueError(f"{C} is more than one. This should not happen."))
# Fortunately, with this example, the Panic function is not called.
```
```
C = Negativify(-1)
if C == 1:
    Panic(ValueError(f"{C} is equal to one."))
# With this example, on the other hand, the Panic function is called.
```
Even though there is a lot added in RandMegan, we will continue adding or rebalancing as we progress with the
development of RandMegan. Please note that RandMegan creates the Entropy,
every time it randomly generates something, which can be a bit slower than other Random Generators regarding performance.

We wish you all the best, and please, stay secure.
