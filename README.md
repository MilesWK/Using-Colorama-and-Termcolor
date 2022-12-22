# Using Colorama and Termcolor
A great guide to learn how to make colored text in Python!!!

Colorama and Termcolor are two python modules that can, when combined, created awesome colored text!\

Colorama project link: https://pypi.org/project/colorama/

Termcolor project link: https://pypi.org/project/termcolor/

**To start**, we need to install the two modules. The best way to do this is using pip. 

In the Command Prompt / shell app, run this to install colorama:
```
pip install colorama
```
Or you can run this in IDLE:
```python
import os

os.system("pip install colorama")
```
After running one of those, pip will install colorama. 

Next, we need to install Termcolor:

In the Command Prompt / shell app, run this to install termcolor:
```
pip install termcolor
```
Or you can run this in IDLE:
```python
import os

os.system("pip install termcolor")
```

Now that we have both of our modules, we can start programming!

In python create a new python file, as the first two lines, we need to import the two modules into our program:
```python
from colorama import init, Fore, Back, Style
from termcolor import colored
```

We also need to import one other module:

```python
from time import sleep
```

Next, we need to use Colorama to make Termcolor work on Windows:
```python
init(autoreset=True) #Makes Termcolor work on Windows devices
```
The "autoreset=True" inside the "init" function makes it so we don't have to reset the color after using it. That only applies if running color through colorama only.

Now, we can print colored text with the colored() function:
```python
print(colored('This is red text on a white background','red','on_white'))
```

Last, we need to make it so the terminal window doesn't automatically close after it prints, because the terminal window closes after completing all the tasks:

```python
sleep(10000) #waits 10000 seconds before ending the program
```
Save and run the program. 

This is the output you would get if you run it in IDLE:

![image](https://user-images.githubusercontent.com/121042782/208771033-b3a1763f-e56a-423a-8960-884ecd34e472.png)

But this is the output you would get if you ran it in the terminal:

![image](https://user-images.githubusercontent.com/121042782/209204410-7a2cfabc-4f77-4006-8d26-594c95117efa.png)

Here is a list of all the available colors (they work with both text colors and background colors):
  - Gray
  - Red
  - Green
  - Yellow
  - Blue
  - Magenta 
  - Cyan
  - White

**Note:**
The color will only show when running the program in the terminal. Otherwise, you will get ASCII around the text.
