# _Having Trouble With Tkinter Module?_<br/>
## Read This File To Know EveryThing About TkinterModule!
#### Note*: The [Official Tkinter](https://docs.python.org/3/library/tkinter.html) or the [Official Python](https://www.python.org) has *nothind to do with this MODULE*
<br/>
First download the source code form https://github.com/Parvat-web-dev/Tkinter-Module/archive/main.zip and place it in the file where you are to save the create a python program.

Lets start by importing the file,
```python
#We Recommend you to import like this:
from TkinterModule import *

#-----------or-----------

import TkinterModule    #You can Import it this way too, but *not recommended*
```
<pre>

Now, let you know what are the functions available in the TkinerModule !

Module Name:
    TkinterModule
    
The package requires:
    Python 3.7.4 or Greater, available at </pre>[Official Python](https://www.python.org)<pre>
    Tkinter installed,
        if not installed and python and pip are istalled, visit</pre> [Wiki How](https://www.wikihow.com/Install-Tkinter)
<pre>
    
Available Functions:
    
    1. size()
    2. title()
    3. button()
    4. input_area()
    5. value_of()
    6. label()
       
Defenitions:

    1. size(Surface, width, height):
        Adjusts the size os the Tkinter screen.
        % Same as geometry() in tkinter. %
        Parameters:
            1. Surface: <class 'tkinter.Tk'>
                The variable of Tk()
                
            2. width: <class 'int'>
                The width of the screen in pixels.
                
            3. height:  <class 'int'>
                The Height of the screen in pixels 
            
            Ex:
</pre>
```python
from TkinterModule import *

#Creating a variable for Tkinter screen
window = Tk()

#Changing The size of the Tkinter Screen
size(window, 700, 700)
#Now the size of the Tkinter screen
# will be 700 px wide and 700 px height

```
<pre>
    2. title(Surface, title_name):
        Gives a title to the screen.
        
        Parameters:
            1. Surface: <class 'tkinter.Tk'>
                The variable of Tk()
                
            2. title_name: <class 'str'>:
                Sets the title as the given string.
                
        Ex:
</pre>
```python
from TkinterModule import *

#Creating a Tkinter Screen:
window = Tk()

#The title's name can be given in two ways:
name = "This Is The Title"
title(window, name)

#---------or----------#
title(window, 'This Is The Title')

#In both the cases the title is changed
```
<pre>
    3. button(Surface, TEXT, position, command, **optional_arguments):
        Parameters:
            1. Surface: <class 'tkinter.Tk'>
                The variable of Tk()
     
            2. TEXT: <class 'string'>
                The Text You want on the button.
                
            3. position: <class 'list'>
                The X and Y postion of the top left corner of the button.
                Ex:
                button(Surface, 'Button', [100, 100])
                    or
                pos = [100, 100]
                button(Surface, 'Click', pos)
                
            4. command:
                The command to pass when the button is clicked.
                *Note, by default it is none, and it is an optional parameter.
                *You can access it like this:
                Ex:
</pre>
```python
from TkinterModule import *

window = Tk()

def myFunc():
    print('You Pressed The Button!')

myBtn = button(window, 'Click', [10, 10], command = myFunction) #You will have noticed that the call of the function doesnot have any brackets! and will not have!

#looping the tkinter!
window.mainloop()
```
<pre>
            **optional_arguments:
            There are many other parameters that you add if you want them!
            These arguments are called like this:
            
            button(Surface, 'Button', [10, 10], argument1 = 'value1', argument2 = 'value'2, ...)
            
            5. text_color:  <class 'string'>
                The text color on the button!
                *Node By Default It Is Black
                
            6. bg_color:    <class 'string'>
                The background color of the button.
                *Note By Default It Is White.
                
            7. width:   <class 'int'>
                The width of the button.
                *Note By Default It Is 5units wide!
                
            8. height:  <class 'int'>
                The height of the button.
                *Note By Default It Is 1unit height.
                
            9. font:    <class 'string'>
                The font of the text displayed on the button.
                *Note By Default It Is 'Courier'.
                
            10. font_size: <class 'int'>
                The font size in pixels.
                *Note By Default It Is 32px.
                
                
    4. input_area(Surface, position, **optional_arguments):
        This function gets input from the user on the tkinter window.
        *Note: This function is same as 'tkinter.Entry()'!
        
        Parameters:
        1. Surface: <class 'tkinter.Tk'>
            The variable of Tk()
         
        2. position: <class 'list'>, item - <class 'int'>
            The position of the top right corner of the input field.
            *Note it should be in the 'list' type with only 2 items.    
        
        **optional_arguments:
        3. text_color:  <class 'string'>
                The text color on the input area!
                *Node By Default It Is Black
                
        4. bg_color:    <class 'string'>
            The background color of the input area.
            *Note By Default It Is White.

        5. width:   <class 'int'>
            The width of the input_area.
            *Note By Default It Is 190px wide!

        6. height:  <class 'int'>
            The height of the input area.
            *Note By Default It Is 22px height.

        7. font:    <class 'string'>
            The font of the text inputed on the input area.
            *Note By Default It Is 'Courier'.

        8. font_size: <class 'int'>
            The font size in pixels.
            *Note By Default It Is 12px.
        EX:
</pre>
```python
from TkinterModule import *

#Creating a variable for the tkinter's screen
window = Tk()

#Creating a Input Area.
input_field = input_area(window, [10, 10], text_color = 'white', bg_color = 'black', width = 200, height = 25, font='Modern', font_size = 13)

```
<pre>
            
    5. value_of(input_field_name):
        Returns the value of the input_area.
        
        Parameters:
        1. input_field_name:
            The variable assigned to the input_area.
            
        EX:
</pre>
```python
from TkinterModule import *

window = Tk()

#creating a input_field
a = input_area(window, [10, 10])

#Creating a function which should be called when the button is pressed:
def click():
    val = value_of(a)
    print(a)

#creating a button!
b = button(wwindow, [50, 10], command = click)

Explanation_of_the_code = '''
    First the window was created.
    Next We created an input field on the screen
    Then we created a function named 'click' which is called when the button is pressed
    Then we create a button and thats all.
    When the button is pressed, it calls the function and the function
    prints the value of the text inputted in the input_area!
'''

window.mainloop()
```
<pre>
    6. label(Surface, text, position, **optional_argument):   
        Creates a label on the screen.
        *Note same as 'tkinter.Label()'.
        
        Parameters:
        1. Surface:    <class 'tkinter.Tk'>
            The variable of Tk()
        
        2. text:    <class 'string'>
            The text to be displayed on the screen.
            
        3. position:    <class 'list'>, list_item <class 'int'>
            The position of the top left corner of the label
            
        **optional_arguments:
        4. text_color:  <class 'string'>
            The color of the text.
            *Note By Default It Is 'black'.
            
        5. bg_color:    <class 'string'>
            The background color of the label.
            *Note By Default It Is 'white'.
        
        6. anchor:  <class 'string'>
            The anchor of the text.
            *Note By Default It Is CENTER
            
        7. font:    <class 'string'>
            The font of the string.
            *Note By Default It Is 'Courier'
            
        8. font_size:   <class 'string'>
            The font size of the text in pixels.
            *Note By Default It Is 14px
</pre>        
Thanks For Using This Module.<br/>
Credits:<br/>
```Parvat.R and Rohit.S.V```<br/>
More Functions will be added on request!
For More Pygame Module Visit: [myPygameModule](https://github.com/Parvat-web-dev)
For Telegram Bots Visit : [Rohit.S.V](https://github.com/rohithaditya/)
