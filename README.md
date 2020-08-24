# Python
This repo contains my Python notes from core to expert.

## Basics of Python

### Types of Interpreters:
- We have 2 Methods to run a program or do tasks:
- (a): By writing the code offline like notepad and other softwares like anaconda,etc and running the code
- (b): By IDE that is Integrated development environment.
- The good thing about IDE is whatever code you write,it will save and same time you can run it like a live interpreter. and some more facilities like create and manage the files.
- There were lots of IDE's available like: Spyder,eclipse,pycharm,Jupyter.
- We were gonna use Jupyter.
#### Setting up IDE
- To install : `pip install jupyter`. in your cmd.
- To launch : `jupyter  notebook`. ; this will open your jupyter notebook in your browser where we can write and run and save the code.
- Click on `new` and then `python3` to open your new notebook.
- This will run like a live interpreter same as REPL.
- The box there where you write your code is known as `cell` and we can run one cell at a time.
- To run your code use `shift+enter`, this will run your code and automatic go to next cell.
- To delete the cell use: `Esc+dd` to delete.
- If we do `Alt + Enter` Then it will run the current cell and at the same time execute new cell.
- Similarly for more keyboard shortcuts use `H`.

- (c): Or we can do this by online interpreters present such as CMD But they can directly run the o/p.  Eg: like if do x=5 and enter then the value is assigned to x there in online interpreters.
- Online interpreters are also called as Live interpreters.
- Examples are in CMD if we run python and can do anything there then that thing is done live(hand to hand).

- ` Question: How to read the Entire data of RAM/Memory ?`
- ` Answer: `
 

- Note: If you create any file with .py extension in the text editor like Notepad in windows then do save in " " (Double quotes) bcz if you save any file with doublequotes then it didn't add any .txt extension with it.

### Variables and Datatypes
- In python you don't need to define a datatype just like you define in other languages eg. in C you define like int x=5; ,but here we don't need to define datatypes because python is smart and it automatically assign datatype at runtime.
- To assign a variable in python: `x=5` ,Here x is assigned by 5 and datatype is int.
- To know or print the data of x: `print(x)` or simply `run x`.
- To know datatype of x: `type(x)` ,here type is a function which defines the datatype of variable.
- This dynamically concept is known as Intellegence or Type inferrence, it means you don't have to define a datatype;on the runtime it will automatically define it.
- If you store anything in a variable inside `" "` or `' '` then the datatype is always a `string`.
- There is no difference in python in " " or ' ' .
- If you want anything in Boolean datatype then do `x= True` or `x=False` where T and F should be in caps and if you do `type(x)` then this will give you as datatype `bool`.
- `Limitation of variable`:Variable is just like a box and we can only store one thing at a time of initializing it.

### Print function and REPL
- To print any variable use `print(x)` or we can do print without using print function, by simply running the variable lets say `x` .
#### `>>>` Symbol is known as REPL which means Read Evaluate Print Loop
- Where `Print` uses print function thats why we can use any variable name direcly or eg. "hii" directly to cmd and get the output as hii.
- Where `Evaluate` means if you write any expression to cmd then it will automatically evaluate that expression we don't need to write any function with it.
- Eg.: 5-2+4-2 in cmd this will automatically give output as 5.
- REPL is the facility of Live interpreter.
- For Live interpreter there is a website available which use REPL tech.
- Link: https://repl.it/languages/python3 

### Variables and Lists
- List means just like you want to store some name or anything, then we need to create a list for it.
- To define a List in python: `x = [ "Manan", "Krish" , "Alok" , "Jay" , "Kick" ]` .
- Where the names were called as Elements or items in python which were stored in variable `x`.
- And if you do `type(x)`  then this will give you as datatype `List`.
- Here in List, Elements starts from index 0 then 1 then 2 and continue.
- If you do `x=[1]` or `x[1]` then this will give the o/p `'krish'` as it is in 1st index.
- To find the total number of items/elements in a variable : `len(x)` ,where len stands for length which gives the total length of the variable.
- Since, we know that every thing is dependent on a function same as this `x=[1]` or `x[1]` is also dependent on a function, when we run this, it calls a function named `__getitem__()` and that function gives the item required.
- Similarly, if we do `x.__getitem__(1)` then this will give o/p as `'krish'`.
#### Slicing in a List
- If we dont want to print the entire list we can do slicing by giving the range to print.
- Eg.: `x[2:4]` then o/p `['Alok' , 'Jay' ]` ,here it will starts from position 2 and goes up to 3, last number will always be excluded same as in example, 4 is excluded.
- Similarly we can do as `x[:3]` ,This will starts from 0 ; `x[2:]` ,This will starts from 2 and print till last ; `x[:]` will print all the items.
- Similarly we can also do `x[-1]` to print the last item ; same as `x[-2:]` will print last 2nd option till last.
- If we do like make a list let say `n= [1,2,3,4,5,6,7,8,9]` and if we do slicing as `n=[2:6]` then it will give o/p as `[3,4,5,6]` so this means bydefault it will jump by 1 because bydefault if we write or not but they have colon 1 as there syntax as `n=[2:6:1]`
- And we can change its bydefaut nature as `n=[2:6:2]`, this will give o/p as `[3,5,7]` means jumped  by 2 positions.

#### Use of List
- If we want to store multiple data in a box, we need a List.
- We can create a list inside a list to store multiple data lets say, we want to store id,name,roll no. in a list we can do as :
` x = [ [1 , "Manan" , 1111] , [2, "Krish" ,2222] , [3 , "Lalki" ,3333] , [4 , "Opal" ,4444] ] ` .
- Similarly if we do `len(x)`, will give output as `4`.
- Similarly `x[0]`  o/p is `[1 , "Manan" , 1111]` .
- Similarly `x[0][1] o/p is `['Manan']` .

- `Question: How to retrieve coloumn wise data from List for eg. 2nd coloumn from x`.
   ` x = [ [1 , "Manan" , 1111] , [2, "Krish" ,2222] , [3 , "Lalki" ,3333] , [4 , "Opal" ,4444] ] ` .
- `Answer : It is impossible because List does'nt support coloumn wise data, list only fetches row wise data. For fetching the column data we have Arrays datatype and for using arrays we have to use numpy libraries. `

#### `in` operator in  list
- We can use `in` operator to find anything from a list.
- Syntax: `"Manan" in x` , will find Manan in list x and if present give o/p as `True`.
- If we use as `and` operator and `or` operator to find multiple word in a List.
### Array , Modules & Functions(Builtin,3rd Party)
- Array function is not a builtin Function, we have to ask to load some third party `program file` and that program file typically known in programming world as `Modules` and for Array fuunction we have to load `numpy` as a Module.
- `import numpy` where import is a function which loads 3rd party Modules and numpy is a Module which have functions like array.
- Module contains 100's of Functions.
- To know the functions of Module's run `dir(numpy)` dir will list all the functions inside numpy modules.
- Similarly if you want to see all the functions which are `Builtin` eg.: print(),type(). Builtin means we don't have to go for third party programs/modules, it is bydefault present inside the python.
- Run `dir(__builtins__)` will list all the builtin functions inside python.
#### Basics of Modules
- Module is just like a program file and every module comes from a library.
- To install that library or module use : `pip install `module_name``.
- To list all library of modules in your os use: `pip list`.

#### To create an Array
- `import numpy` because array is a function of numpy module.
-  Then create a list eg.: ` x = [ [1 , "Manan" , 1111] , [2, "Krish" ,2222] , [3 , "Lalki" ,3333] , [4 , "Opal" ,4444] ] ` .
- Then convert that list into array  by `a = numpy.array(x)` ,where we have stored our array in a.
- and if you see the datatype of a `type(a)` it is numpy array.
- Now we can do same operations as `a[1:]`.
- Now to print Coloumn wise date do `a[0:4 , 1]` will give you the 1st column data. 
- Here also indexing starts from 0.
- For printing all data of 2nd column use :`a[: , 1]`
- If we want to print 2 columns : `a[: , 0:2]`

##### NOTE: For practicing in the live interpreter is good, but if once you terminate the interpreter by `exit()`,and then again opening `python` in terminal and searching for the data you created before; you doesn't get the same data you have created before. So the best practice is to do in offline way by creating a file and saving it or by using different softwares.

### Taking input from the user.
- If we want to take input from the user we have a function called `input()`, Lets say i want to take input from the user and store in x?
- Do `x = input()` , this will asks user to give input and stored in x.

#### Creating a program that will ask user to give input that eg. a user want to open chrome using python.
- We create this file in Notepad, Open `notepad` .
- `import os` will import the os module which contains functions like system() .
- `x = input()` , this will take input from the user.
- `os.system(x)`, system is a function, which calls the os to run the input givrn by the user.
- Save the program by "input.py" ,using doublequotes will not save your file by .txt and make sure that saving the file to the same LOC where your terminal is
##### Output 
- Run as `python input.py` in cmd.
- and give input as `chrome`.
- This will open your chrome browser.

#### Running a program that will convert your voice into speech.
- We have a Module called `pyttsx3` for converting your text into speech, where tts is text to speech.
- Firstly install pyttsx3 module in your os as: `pip install pyttsx3`.
- In this module we have different functions just like `speak` is a function that converts your text to speech.
- Then open your python interpreter as `python` in cmd.
- Then import your module: `import pyttsx3`
- Then do print what you want to convert: `pyttsx3.speak("Hello World, Wellcome to our Python World.")`
- Where speak is a function which will convert your text into speech.

### Working on Jupyter
- To launch : `jupyter  notebook`. ; this will open your jupyter notebook in your browser where we can write and run and save the code.
- Click on `new` and then `python3` to open your new notebook.
- `import os` will import all functions of os.
- `dir (os)` will give you all the functions available in the os module.
- We were going to use `system` module to open chrome,notepad,etc.
- `os.system("Chrome")` will open your chrome browser.
- `os.system("notepad")` will open your notepad.

### Special characters
#### Escape sequence keywords
- Newline sequence -> `\n`
- Tab sequence -> `\t`

### Comments in Python
- 1.) Line Comment: If we start a line with `#` , this will mark it as line comment.

###### NOTE: In python there is no difference in double quotes and single quotes, you can run any special characters in any form.
### Some Tips & Tricks
- 1.  If you put r in starting just like `print(r'Helloo \n Peoples')` then it gives output as in the same line as `O/P: Helloo \n Peoples`. Here r means consider it as row and       it doesn't process the special operation inside double quotes.           
- 2.  `print()` function in python internally have a newline char and will always give new line.
- 3.  If we want to know detail of any function, use `help(function_name)` .
- 4.  If we don't want that print function would give newline, use `print("Hellooo" , end='')` .But this syntax only works in Python3.
- 5.  In python, we don't use {} here in if else, we use spaces here and that is called as indentation. And Indentation must be same.
- 6.  In python, we don't have a support of switch cases, because if,else & elif works as switch cases. 
                   
## Some Programs
#### Creating a program that will speak "Welcome to my tools" and ask your choice to open any program.
- Open `notepad` and do save your file as " " to avoid .txt extension.
- write the following code in your file:
- `import pyttsx3`
- `import os`
- `pyttsx3.speak("Welcome to my tools")`
- `p = input("Enter your choice of program")`
- `os.system(p)`
- Do save this file in the loc of cmd or set your cmd to the file loc as per convinience.
- Open CMD.
- Run your file as `python mysoftware.py` ,here mysoftware.py is the name of the file.
- Give input to the file as which software you like to open lets say `wmplayer`
- O/P: your OS will open wmplayer.

## 16 Aug 2020 | Day 3

#### String
- According to python, string is basically a sequence of the char means every char is independent.

