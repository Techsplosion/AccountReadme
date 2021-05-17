# Introduction
Hello guys! I am Techboy v1050. You can access my youtube channel at [here](https://www.youtube.com/channel/UCzbYYyFvd5lXhEK_EdnPkTw). I have 40 or so (as of now) subcribers.
If you subscribe to me, that would mean a lot. But you don't have to!
# Python
## Basic
### Hello World Program
#### File `helloworld.py`
```py
print("Hello world!")
```
### Simple Modulus with User Input (is done with dividing by 2 and the % icon for modulus, the remainder can be `0` or `1` and is outputted):
#### File `modulus.py`
```py
i = int(input("Enter a whole number to see the remainder: ")
print(i % 2)
```
## Complicated
### Decorators
#### File `decorators.py`
```py
def start_end(func):
	def wrapper_se(*args, **kwargs):
		print("Started.")
		func()
		print("Ended.")
		return
	return wrapper_se


@start_end
def print_hi():
	print("Hi!")


print_hi()
```
#### Output
```
Started.
Hi!
Ended.
```
### Complex Imports
#### Module `somepackage\__init__.py`
```py
def print_hi():
	print("Hi!")
```
#### Module `somepackage\other.py`
```py
def print_hi_in(inprefix: str):
	in = input(inprefix)
	print(f"Hi, {in}!
```
#### File `cimports.py`
```py
import somepackage
from somepackage import other

somepackage.print_hi()
otherprinth_hi_in("Enter your name: ")
```
Test the files and see the output.
# C++
## Basic
### Hello World Program
```cpp
include <iostream>
using namespace std;
int main() {
	cout << "Hello world!" << endl;
}
```
