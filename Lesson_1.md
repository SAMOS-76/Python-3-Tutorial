# Lesson 1
## Accesing IDLE
IDLE is a built-in software with python that allows you to write and execute code.  
To find IDLE in Mac OS:  
  * Open your terminal.
  * Simply type **idle** into your terminal.
  * A rocket icon should show up as IDLE loads.

To find IDLE in Windows:  
  * Press the search icon at the bottom left of your screen.
  * Start typing **idle** into it.    

## Using IDLE
Once idle has loaded, you should see a window like the image below called **Python 3.x.x Shell**, where 3.x.x is your version of python.  
![alt text](https://files.realpython.com/media/idle-1.ad05cbe1e2f7.png)   

This window that we are in now is called the **Shell Window**. This windowis useful for testing quick pieces of code. Here code is executed the moment you press enter. Let's try it! Your first line of code! 
Type the code below and press enter
```python
print("Hello World!")
```
Your window should look something like this:  
![alt text](https://files.realpython.com/media/idle-2.c0a65df087ef.png)   
Congrats! You just wrote your first line of code! Here's how it works.  
The **print()** command is a fuction, a pre writtern bit of code, in python that justs print's the thing that's inside the brackets to the screen. Make sure that if you are typing letters into the **print()**, the letters are surrounded by either single('') or double("") quotation marks. 
If it didn't work then you most likely got some red text saying somethng along the lines of:  
```python
SyntaxError: invalid syntax
```  
This is a type of error in python. This paticular error means that you have typed something wrong. Syntax is the combination of spelling and punctuation that a computer can understand. Check and make sure the code you have written matches **exactly** to what I put above.  

## Saving your code
The shell window is good for testing small peices of code but you can't save anything in it. To be able to do this you need something called a **code window**. I will now go through the steps to save your code.  

1. Click on file at the top of the shell window and select **New File**. A code window will now open up.  
2. Click on file at the top of your Code Window select **Save As**. Name the file **Hello World.py**. **.py** tells the computer that the file is a python file. Save the file in a central location you can find easily.  
3. Go back to your code window and type in...  
```python
print("Hello World!")
```  
...just as we did before.  
4. Click on file again and click **save**.  
5. Click on **run** and select **Run module**. In this instance, **module** means python file.  
6. The Shell window should then open up and the words **Hello World!** should appear.  

## Numbers in python  
### Adding in python  
Open/go back to the shell window and type and press enter: 
'''python
4 + 4
'''  
You should see the shell window output:  

### Subtracting in python  
Type and press enter: 
```python
8 - 4
```  
You should see the shell window output: 

### Dividing in python  
Type and press enter: 
```python
8 / 4
```  
You should see the shell window output: 
Notice how we don't use the standard **÷** symbol. In python and computer science in general we don't use the normal divide sign but the **/** sign.

### Multiplying in python  
Type and press enter:  
```python
2 * 2
```   
You should see the shell window output:  
Notice how we don't use the standard **x** symbol. In python and computer science in general we don't use the normal divide sign but the **'*'** sign.  

### Equals sign 
In python, we don't use **=** for maths but for a different purpose that will be answered in a moment.  

## Variables  
Variables are like a named boxes where you can store information. You can change this information but the label stays the same.  
### How to create a variable  
```python
age = 14
```  
You have just created a variable called age. You can call a variable anything you like as long as it doesn't have spaces, certain special characters, and it can't be a python keyword. You will know if it is a keyword as it will be coloured.  
 * hello there = 5 (wrong) 
 * age! = 5 (wrong) 
 * print() = 5 
 * age = 14 (perfect!) 

### Using variables  
1. First go to the shell window and type:  
```python
var1 = 3
var2 = 2
```  
2. Now we are going to do some maths with this. Type the following and press enter:  
```python
>>> var1 - var2
```  
The following should come up:  
```python
1
```  
The variables have numberts assigned to them so you can do arithmatic with them.  
3. Lets assign var1 to something else and do an equation:  
```python
var1 = 5
var1 - var2
```  
You should get:
```python
3
```  
This is because we have changed the "item in the box" from 3 to 5.  

### Strings in python.  
What is a string? Well a string in python is a word or a collection of letters or symbols. You can also put strings in variables.  
```python
var3 = "This is a string"
```  

### Getting user input 
If you wanted the user of your code to decide what a variable is in python then you need to use the **input()** function.  When using the input() function, inside the brackets you put the question you want to ask inside the brackets and assign the input to a variable:  
```python
name = input("What is your name? ")
```  
Press enter and **What is your name?** should come up. Beside this text type in, well any name.  
On the next line type:  
```python
print(name)
```  
Press enter and you should see the name you put in be outputted.  

### Our first project  
We are going to use everything that we have learnt today and create a small project. It will be a script to create our own character.  
1. Click on **file** and select **new file**. Press **save as** and save it as **Character_Code**.
2. Next, we are going to create a title at the top of our script.  
```python
print("Create your own character") 
```  
3. Use the **input()** function to ask the user for their charcters name.  
```python
name = input("What is your character called? ")
```  
4. Then we can do the same for different attributes for example:  
```python
age = input("What is your character's age? ")
place = input("Where is your character from? ")
like = input("What does your character like? ")
dislike = input("What does your character dislike? ")
```  
5. Now we need the computer to print your character description: 
```python
print("Your character's age is ", age)
print("Your character is from ", place)
print("Your character likes ", like)
print("Your character dislikes ", dislike)
```  
6. We have finished our first part of the script. Go to **file** then **save**. Now press run and the code should start working.  
7. We are now going to add some extra code at the end:  
8. Create a new variable called **ageNextYear**:
```python
ageNextYear = int(age) + 1
print("Your character will be", ageNextYear, "next year".)
```  
When you enter anything into a **input()** function it returns a string so the **int()** converts it to a number instead of a string.  

That is all for our first lesson hope you enjoyed. There is however a small amount of homework.  
## Homework
What i want you to do is try and make a diiferent character creator with your own variables and we will go over them together at the beginning of the next lesson.  
