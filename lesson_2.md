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

##Making Decisions in python    
To make a python script that allows you to choose what happens in it we need to use something called conditions. A condition is a bit of code that compares two pieces of information using the comparitive operators below:    
  * **==** means **is equal to**  
  * **!=** means **is not equal to**  
  * **<** means **is less than**
  * **>** means **is greater than**
  * **<=** means **is less than or equal to** 
Another word for condition is a **Boolean expression**. This just means **True** or **False**. Let's go to the shell window and type the following code:  
```python
>>> age = 10
>>> age == 12
```  
Line 1: This creates a variable called age and gives it the number 10.  
Line 2: This line uses the comparitive operator **==** meaning **is equal to**. This line basically justs asks if age **is equal to** 10 and should return:  
```python
False 
```  
This returns **False** because 10 does not equal to 12. How about if we change the value of age:  
```python
>>> age = 12
>>> age == 12
```  
This returns:  
```python 
True 
```  
Note that **True** and **False** are capital letters to tell python that we are using conditions.  
We can replace the **==** sign with any other comparitive operator and see the different results.  

## What are conditionals?  
To use a condition in your save code we need to use a python command called a **conditional**. Conditionals use conditions to test if something is **True** or **False** then they decide what path in the cide we should take. 

### The IF statement  
The most important conditional is called the **if statement** which tests if a condition is True. **if** it is True, the computer will carry out the code inside of the if statement. **if not**, the computer will just skip it. In python, **if** is a keyword so you can't use it as variable names. Create a new file in a code window and type in the following:  
```python
reply = input("Do you like animals? (Type yes or no)")
if reply == "yes":
    print("Animals like you too"
```  
Line 1: We create a variable called reply and put the value from the input inside of it.  
Line 2: **if** reply **is equal to** yes, then... (note that after the if we have a colon)  
Line 3: print, animals like you too.  
You should notice that there is a space from where the print() starts called an indent. Python uses this the group lines of code together so the computer knows what to do next. Where a line is indented means that it belongs to the line above.  
Save and run the program. If you type **yes** (make sure it's lowercase) it will print out the statement. If you say anything else, then it won't do anything because the condition isn't True.  

### The ELSE statement  
The **else** statement tells the computer what to do if the **if statement** isn't true. Go back to our previous code and add to the bottom:  
```python
else: 
    print("Well animals don't like you either")
```  
The completed code should be this:  
```python
reply = input("Do you like animals? (Type yes or no)")
if reply == "yes":
    print("Animals like you too"
else: 
    print("Well animals don't like you either")
```  
Save and run the program. If you type **yes** (make sure it's lowercase) it will print out the statement. If you say anything else, for example, no, then it will print the statement in the else command.  

### The ELF statement  
The **elif** statement is short for **else-if**. **elif** ALWAYS comes after an **if statement** and carries out it's code if the **if** is False. Go back to our previous code and change it to:  
```python
reply = input("Do you like animals? (Type yes or no)")
if reply == "yes":
    print("Animals like you too"
elif reply == "no": 
    print("Well animals don't like you either")
else:
    print("Please answer with yes or no")
```  

## Random numbers and the while loop   
### The Random Module
To generate random numbers in python, we need a new function  called **randint**. However, all the random number functions are stored seperately in something called a module. To get to them you need a keyword called **import**. Make a new file and type in:  
```python
import random
number = random.randint(1, 20)
print(number)
```
Line 1: Here we import the random module.  
Line 2: We create a variable called number and we give it the value of random.randint(1, 20). This created a random number from 1 to 20.  
Line 3: We print this random number.  

### Adding Loops  
A **loop** is a bit of code that repeats. Loops save time because tou don't have to keep typing the same thing over and over. We are going to look at the **while loop**. A **while loop** repeats as long as a certain condition is true. Add the following to our previous code:  
```python
import random
number = random.randint(1, 20)
guess = int(input("I'm thinking of a number what is it? "))
while guess != number:
  if guess < number:
    print("Your number was too low...")
  else:
    print("Your number was too high")
  guess = int(input("Please try again "))
print("Congrats!! That is correct" )
```  
