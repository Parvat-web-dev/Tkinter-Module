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
    Python 3.7.4 or Greater, available at [Official Python](https://www.python.org)
    Tkinter installed,
        if not installed and python and pip are istalled, visit [Wiki How](https://www.wikihow.com/Install-Tkinter)
    
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
            ```python
            from TkinterModule import *

            #Creating a variable for Tkinter screen
            window = Tk()

            #Changing The size of the Tkinter Screen
            size(window, 700, 700)
            #Now the size of the Tkinter screen
            # will be 700 px wide and 700 px height
            
            ```
            
    2. title(Surface, title_name):
        Gives a title to the screen.
        
        Parameters:
            1. Surface: <class 'tkinter.Tk'>
                The variable of Tk()
                
            2. title_name: <class 'str'>:
                Sets the title as the given string.
                
        Ex:
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
       
    3. button(Surface, TEXT, position, **optional_arguments):
        Parameters:
            1. Surface: <class 'tkinter.Tk'>
                The variable of Tk()
    
    `More Will Be Added Tomorrow!`
    
    
    
    
</pre>        
