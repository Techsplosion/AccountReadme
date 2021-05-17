# Introduction
Hello guys! I am Techboy v1050. You can access my youtube channel at [here](https://www.youtube.com/channel/UCzbYYyFvd5lXhEK_EdnPkTw). I have 40 or so (as of now) subcribers.
If you subscribe to me, that would mean a lot. But you don't have to!
# Python
## Basic
### Hello World Program
```py
print("Hello world!")
```
### Simple Modulus with User Input (is done with dividing by 2 and the % icon for moddulus):
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
Output:
```
Started.
Hi!
Ended.
```
