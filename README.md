# RandMegan
### Version: 0.0.3.5
Before you read this, we suggest that you read the "LICENSE" file first.

##What is RandMegan? 
RandMegan is a Python Random Package, that uses mostly Cryptography. RandMegan is purposed to be lightweight, and RandMegan is purposed for random functionalities, independent of Python's built-in Random Module.

##In Development Notice: 
We would like to inform you that RandMegan is new, and RandMegan is in the Early Access phase of its development; RandMegan may sometimes contain bugs (some of the bugs can
be awkward) and glitches. If you encounter any bugs and glitches, you can contact Foxy CS (Anonymous) via Email: "foxrobinleela@gmail.com" for inquiries about RandMegan.

##How do you use RandMegan?
There are a few functionalities we would cover for RandMegan, and it may not be limited to just the functionalities mentioned.

The first example we would cover is how to import it. Say, for example, you have the package, and your main Python file through mentioned paths:
```
.\\Project\\RandMegan\\__init__.py
.\\Project\\RandMegan\\randy.py
.\\Project\\Project.py
```
You want RandMegan to be imported through 'Project.py'. It can be as simple as using:
```
import RandMegan
#place your code here
```
It is simple, and you do not need to add some additional code to import RandMegan.

Another example is when you imported it, how can you use its random integer generator? It is also coded in our methods to make the code simple, and easy to use.
Here are two examples of how to do it:
```
import RandMegan
print(RandMegan.intrandom(0, 10))
#Returns a random integer. No errors would occur
```
```
import RandMegan
print(RandMegan.intrandomplus(0, [1, 2, 3, 4, 5, 6]))
#Also returns a random integer, just a bit more complex than the other one. It uses the length of the List
#if you are a person who likes to be complicated with your code, you at least have the option to do so.
```
In retrospect, that is not all you can do with RandMegan; you also have a random boolean function. How you can use it is as follows:
```
import RandMegan
print(RandMegan.boolrandom())
#Returns either "True" or "False" at random.
```
In addition, we also have the Random Character selection for a string:
```
import RandMegan
print(RandMegan.strandom("HI THERE!"))
#Selects a random character from a String.
```
Another addition is the Shuffle functionality, and this is beneficial for gamers who like card games:
```
import RandMegan
List = ["Ace_Of_Diamonds", "King_Of_Diamonds", "Joker"]
List = RandMegan.Shuffle(List)
#Cards are shuffled randomly, and the function uses a specific shuffle name. Can you figure out the name for that type of Shuffle?
print(List)
```
In addition to the Choose Random functionality:
```
import RandMegan #Assuming you already did that.
List = ["Pac-Man", "Tetris", "Blackjack", "Space Invaders"]
print(RandMegan.chooserandom(List)
# Select a Random index, to get the random value.
#The Choose Random functionality can work with any variable values in the list. However, using the non-plusified variant is predictable with its index.
```
The Plusified variant of the Choose Random:
```
...
List = ["Pizza", "Chocolate", "Custard", "Pasta", "Poultry", "Beef", "Oxtail"]
Lima = RandMegan.choose_plusified(List)
#First shuffles the index, then chooses a random selection from the list. This can be beneficial if you also look for an unpredictable index return value.
print(Lima)
```
and the Random Bytes method:
```
...
print(RandMegan.Random_bytes(10))
#Returns 10 random byte (Machine Code) values
```
We know that this is short information, but as mentioned, RandMegan is in the in-development phase, and we will be adding or rebalancing as we progress with the development of RandMegan.

Continue Playing.
