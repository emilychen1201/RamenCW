# How to Launch the Software? 

The software is developed with Eclipse IDE, with JDK 1.8. 

The software project name is ***Ramen***, with 4 packages (data, GUI, receiver, process).It is in the same directory as this .md file, with name *Ramen*. 

There are two entrance of the software, corresponding to two major function block: customer and manager. 

### Step 1

To install the software, copy the *Ramen* folder to your computer. Let's assume the path is *'C:\Ramen'*. 

### Step 2

Type *'cd C:\Ramen\bin\'* to enter the 'bin' folder where the .class files are stored. 

### Step 3

##### Customer-side Entrance

Compile and launch *Menu.java*. To do this, type: 

`java -cp .;..lib\jcommon-1.0.14.jar;..\lib\jfreechart-1.0.13.jar GUI.Menu` 

in the command line. 

The menu page will appear for user to directly choose dishes. 

##### Manager-side Entrance

Compile and launch *MngEtr.java*. To do this, type: 

`java -cp .;..lib\jcommon-1.0.14.jar;..\lib\jfreechart-1.0.13.jar;..\lib\log4j-1.2.13.jar GUI.MngEtr`

in the command line. 

two manager functions are available as buttons. 

### Notes

Because the directory of program execution when entering from CMD is './bin',

We changed the file path in the program accordingly.

So Junit tests that can pass in the eclipse environment will FAIL NOW!

To get the JUnit test success, file path must be changed, from "*../inFile/xxxxxx*" to "*./inFile/xxxxxxxxx*". 

(JUnit tests are in the package "test".)