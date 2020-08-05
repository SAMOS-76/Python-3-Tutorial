# Lesson 2    
## Basic built-in functions   
Last lesson we saw 3 of pythons built in functions, print(), input(), and int(). Go back to the last lesson if you can't remember what they do. Now we are going to look at some more of pythons functions to add new stuff to our code.    

### len()   
The **len** function in python is short for length. This basically means it returns the length of whatever you put in the brackets e.g. the length of a string. Copy the code below into the shell window:    
```python
>>> len("hello world!")
```   
This should return:   
```python
12
```   
This is because it counts **every** character in the string, including the space. Now we are going to look at what else we can do with the **len** function. Create a new file called **len.py** and type.   
```python
name = input("What is your name? ")
length = len(name)
print(name, "is", length, "letters long")
```   
Line 1: Here, we ask the user for their name using the **input** function in python. We then save it into a variable called **name**.   
Line 2: We use the **len** function to get the length of the name and save it to a variable called **length**.    
Line 3: We now print the name and it's length to the screen.    

### str()   
The **str** function in python is short for string. We've already looked at strings and if you can't remeber look at the last lesson. 
The **str** function turns intergers, basically just **whole** numbers, into strings. Copy the code below into the shell window:    
```python
>>> str(14)   
```   
This should return:   
```python
'14'   
```   
The number 14 has now been outputed as a string shown by the quote marks around it. You can do everything that you can do to a string to this number now for example:   
```python
>>> string = str(14) + "years old"   
>>> print(str)
```   
This should return:   
```python
'14years old' 
```   
If you tried doing this without converting the interger to a string you would get an error.   
### float()   
Finally we have the **float** function. A float in python is another word for a decimal number like 1.4 or 5.6. This makes them different from intergers whicgh are whole numbers. Copy the code below:   
```python
>>> float("3.14")
```   
This should return:   
```
3.14
```   
You should notice that it no longer has the quotation marks. You can also use it wil intergers.   
```
>>> float(5)
```   
This should return:   
```
5.0
```   
This is because it has converted the interger into a decimal number.    
