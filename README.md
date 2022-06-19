# Introduction
Hello guys! I am Techsplosion.
<details>
<summary>Do</summary>
<details>
<summary>Not</summary>
<details>
<summary>Open</summary>
<details>
<summary>This</summary>
<details>
<summary>I</summary>
<details>
<summary>Swear</summary>
<details>
<summary>There</summary>
<details>
<summary>Is</summary>
<details>
<summary>Nothing</summary>
<details>
<summary>Here</summary>
<details>
<summary>S</summary>
<details>
<summary>t</summary>
<details>
<summary>o</summary>
<details>
<summary>p</summary>
<details>
<summary>I</summary>
<details>
<summary>t</summary>
<details>
<summary>A</summary>
<details>
<summary>l</summary>
<details>
<summary>r</summary>
<details>
<summary>e</summary>
<details>
<summary>a</summary>
<details>
<summary>d</summary>
<details>
<summary>y</summary>
You can access my YouTube channel at [here](https://www.youtube.com/channel/UCzbYYyFvd5lXhEK_EdnPkTw). I have 200 or so (as of now) subscribers.
If you subscribe to me, that would mean a lot. But you don't have to!
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
</details>
All the repositories: [html](https://github.com/Techsplosion/html), [python](https://github.com/Techsplosion/python), [Unity](https://github.com/Techsplosion/Unity) and [CSharp](https://github.com/Techsplosion/CSharp).
***
# Python
## Basic
### Hello World Program
#### File `helloworld.py`
```py
print("Hello world!")
```
### Simple Modulo with User Input (is done with dividing by 2 and the % icon for modulo, the remainder can be `0` or `1` and is outputted)
#### File `modulo.py`
```py
i = int(input("Enter a whole number to see the remainder: "))
print(i % 2)
```
## Complicated
### Decorators
#### File `decorators.py`
```py
def start_end(func):
	def wrapper_se(*args, **kwargs):
		print("Started.")
		func(*args, **kwargs)
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
	inputu = input(inprefix)
	print(f"Hi, {inputu}!")
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

botclient = commands.Bot(command_prefix="mb!")
botclient.remove_command('help')

TOKEN = 'YOUR-TOKEN-HERE'


@botclient.event
async def on_ready():
	print(f"{botclient.user.name} is ready.")


@botclient.command(aliases=["add"])
async def addition(ctx, num1: float, num2: float):
	await ctx.send(str(num1-num2))


@botclient.command(aliases=["subtract"])
async def subtraction(ctx, num1: float, num2: float):
	await ctx.send(str(num1-num2))


@botclient.command(aliases=["multiply"])
async def multiplication(ctx, num1: float, num2: float):
	await ctx.send(str(num1*num2))


@botclient.command(aliases=["divide"])
async def division(ctx, num1: float, num2: float):
	await ctx.send(str(num1/num2))


@botclient.command(aliases=["sqrt"])
async def squareroot(ctx, number: float):
	await ctx.send(str(sqrt(number))


@botclient.command(aliases=["cbrt"])
async def cuberoot(ctx, number: float):
	await ctx.send(str(sqrt(number / 3)))
botclient.run(TOKEN)
```
# C++
DISCLAIMER: I have (pretty much) no idea about C++.
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
### Simple Modulo with User Input (is done with dividing by 2 and the % icon for modulo, the remainder can be `0` or `1` and is outputted)
#### File `modulo.cpp`
```cpp
include <iostream>
include <string>
using namespace std;
int main() {
	int modulo;
	string prompt = "";
	cout << prompt << endl;
	cin >> modulo;
	cout << modulo % 2 << endl; 
}
```
