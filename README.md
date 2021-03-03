# JavaCWstyleExample
A simple example of a course work like task. 


This is a task that i created to give those who may struggle to set up an easy to learn enviroment, another task to practice their java skills. (Or Rust or whatever)
It is structured in a similar way to the UoG prog AE2, with similar difficulty of tasks, however it is much much shorter time wise. This is to give people a familiar set up for the task. 

The task is to recreate the logic from a fighting game loading screen, namely street fighter 2. This is based off of this codewars example here: https://www.codewars.com/kata/street-fighter-2-character-selection-part-2/python

The fighters names and info will all be supplied in a CSV file in the repo. There is also meant to be an ANSCII representation of the selection screen so as to test out the movement and selection fo the screen. 

**Key things**
  -Loading in information via CSV file, this is going to require learning about loading files specifically CSV files, very easy to find out just google java csv file read.
  -The display screen can be formatted in the same way as was done for AE2.
  -Try not to use String += string, if we are already using strings we should use string.append() or string.concat(string) instead.

**Task one:**
  To create a simple fighter class that holds 3 variables, name, from/location, style of fighting.
  There should also be methods toString which jsut returns a name formatted for the display table. 
  getInfo() Which should return all the info on a fighter however you see fit. 
  A bonus would be to be able to visually see which fighter is selected by highlighting the name eg *name*
  If a player can be selected, then it stands they must be deselected.
  
 **Task two:**
  Create a display/board/screen class, that holds an array of fighters but omits the top left and top right square of the selection screen.

  See https://www.codewars.com/kata/street-fighter-2-character-selection-part-2/python for more info on this.
  e.g. 
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
             |   Balrog||   Blanka|           
  |    Cammy||  Chun-Li||  Dee-Jay||  Dhalsim|
  |  E.Honda||  FeiLong||    Guile||  M.Bison|
  |   T.Hawk||     Vega||   Ken M.||*Zangief*|
  
  *Zangief* is from: Russian with a fighting style: Pro-Wreslting
  ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

  This class should have an init() method that loads all of the fighters into an array or representation that you prefer.
  It should also have move and select methods, think oldschool arcade machines, you get left, right, up, down and select.
  These should tie back to the select/deselect methods in the fighter class to show the movement of selection visually.
  The movement of selection needs to wrap around the screen vertically but not horizontally, eg if i was on balrog and 
  i went up i should reach vega, however if i was on Dhalsim and went right i should stay on Dhalsim.
  
 **Task 3:**
  Legit just make a test class with a main method and test the program.
  this was my input in test for the output example above:
  		
    	DisplaySelect ds = new DisplaySelect();
  	ds.right();
	System.out.println(ds);
    
    
    
   
   
   
Disclaimer: I have no idea what im doing and any advice or input is greatly appreciated. 
