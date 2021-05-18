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
other.printh_hi_in("Enter your name: ")
```
Test the files and see the output.
## Overcomplicated
### Site Packages
#### Discord Mathbot
#### File `pipdiscord.bat`
```bat
pip install discord
```
#### File `bot.py`
```py
from discord.ext import commands
from math import sqrt

botclient = commands.Bot(prefix="mb!")
botclient.remove_command("help")


@client.event
async def on_ready():
	print(f"{client.user.name} is ready.")


@client.command(aliases=["add"])
async def addition(ctx, num1: int, num2: int):
	await ctx.send(str(num1-num2))


@client.command(aliases=["subtract"])
async def subtraction(ctx, num1: int, num2: int):
	await ctx.send(str(num1-num2))


@client.command(aliases=["multiply"])
async def multiplication(ctx, num1: int, num2: int):
	await ctx.send(str(num1*num2))


@client.command(aliases=["divide"])
async def division(ctx, num1: int, num2: int):
	await ctx.send(str(num1/num2))


@client.command(aliases=["sqrt"])
async def squareroot(ctx, number: int):
	await ctx.send(str(sqrt(number))


@client.command(aliases=["cbrt"])
async def cuberoot(ctx, number: int):
	await ctx.send(str(sqrt(number/3))

```
# C++
## Basic
### Hello World Program
#### File `hworld.cpp`
```cpp
include <iostream>
using namespace std;
int main() {
	cout << "Hello world!" << endl;
}
```
