**USE CASES**  
<details><summary><b>User Case Diagram</b></summary>
![HEAT_user_case](uploads/2bea741c67418d3bf300a8089d0b1b4f/HEAT_user_case.jpg)</details>
[User Stories](url)<br>  
[Acceptance Criteria](url)<br>
  
<br>**CLASS AND ACTIVITY DIAGRAM**
<details><summary><b>Activity Diagram</b></summary><br>
![HEAT_action_process](uploads/1d07110fc77a5fa4b1f37edd45a8aca2/HEAT_action_process.jpg)</details>
<details><summary><b>Class Diagram</b></summary>
![HEAT_class_diagram](uploads/3097e9933fe380a5150d54e3325da0b7/HEAT_class_diagram.jpg)</details><br>  

**IMPLEMENTATION** Describe what have been done/ would have done/how it was done.   

<details><summary><b>Font Visibility</b></summary><br>

Font size and type specification within the program is distributed and implemented using several methods. The font specifications that needed to be amended in the SettingsManager, WindowManager, MainMenu and OptionsWindow classes. The object of the amendment was to either change existing code, adapt code or add code.The implementation of existing fonts was fragmented and distributed in an appararently haphazard manner. This may be explained because when writing the original code the coders were unaware that subsequently a team would be changing the font type and sizes.<br>

In the SettingsManager class two lines of code were amended to increase the font size to 20. In the WindowManager class one line of code was added using setFont from the java.awt.Font API, changing the font size. In the MainMenu class numerous lines of code were amended to the new font. It was also necessary to amend the code for the undo and redo options (Using JFrame) in order to change the font (JMenuItem). In the OptionsWindow class numerous lines of code had to be adapted. The code used the JLabel method of JFrame. The original code did not include font details. This meant that every time text was displayed one line of existing code needed to be replaced by three.<br>

The amended code will result in larger text size and a font type that is easier to read, by visually impaired users. The implementation has been partially successful with most text changed to Arial and a high font size. There are a number of areas where it was not possible to change the font type or size, for example in pre-filled forms, option tab buttons and the font type in the editor and console windows.The implementation of these items would need considerable research to understand how they are implemented in order to amend the font size and type.</details>


<details><summary><b>Colour & Contrast</b></summary><br>



There are three main windows in the UI, the editor, console, and tree views, along with an additional window for the help section, each of which was modified in its respective class. Each of the windows utilised Swing components, the methods of which were called upon to make the required background colour changes. The different Swing components have slightly varying methods for accessing and changing colours; the Eclipse method suggestion feature was utilised here to browse the available methods and find the appropriate call to make the required changes.  <br>

Some areas, such as the line number bar in the editor window, required changes to be made elsewhere in the program, including the text area defaults file and the text area painter file. The text and syntax highlighting colour changes also required changes in the syntax utilities file. During user testing further colour changes to the help screen and highlight bar were suggested, these changes were subsequently implemented. During this process the team used paired programming methods to achieve higher code quality and to allow the each member to understand the changes being made by others.
</details>

<details><summary><b>Sound Effects</b></summary><br>

To implement the requirements of having sound effects played to signify success or failure of a program or command entered into the Haskell Interpreter involved using the ConsoleWindow.java class and writing a new method called playSound() to play each sound based on certain events.
There is a method inside the ConsoleWndow.java class which calls the Haskell Interpreter to retrieve error information. This method contains a variable called ‘error’ that is incremented every time an error is returned. This was used to determine which sound effect should be triggered by calling the playSound() method with the sound effect name as a parameter of type String. If the error is zero then success sound is triggered, otherwise the failure sound is triggered.
To create the playSound() method 2 javax classes were utilised. These were javax.sound.sampled.AudioSystem and javax.sound.sampled.Clip. More specifically AudioSystem.getAudioInputStream() was used to retrieve a handle to the audio system, and Clip.open() and Clip.start() were used respectively to open and play a sound clip.

To retrieve the file path of the audio files independently of the computer that is being used, it was necessary to use the ClassLoader class which is part of the java.lang package. The String parameter that was passed to the playSound() method is for the name of the file to be found.
The audio files were downloaded from freesound.org
For future the improvements the playSound() method could be used to signify other notifications such as when a user hovers over a particular area.

</details>


<details><summary><b>Caret Cursor Visibility</b></summary><br>
To enhance the visiblility of the caret cursor it was necessary to write a new caret class which extends from the defaultCaret class, within the ConsoleWindow.java class. The code written is based on some code from there http://www.java2s.com/Code/Java/Swing-JFC/Acustomcaretclass.htm

The code was adapted to create a block using g.fillRect() method within the Graphics class, which is part of the java.awt package. The blink rate  and colour was also set using the setBlinkRate() of the current instance of the caret. The colour was also changed to white using Graphics.setColour().


</details>

<details><summary><b>Mouse Cursor Visibility</b></summary><br>
There are several classes that needed to be changed to implement the changing of the mouse cursor. These are EditorWindow.java WindowManager.java and ConsoleWindow.java.
In order to change the mouse cursor it was necessary to write a new mouse method that loads in the image to be used for the mouse cursor, and calls several methods to set the cursor to the new one.
The Images were created using logomakr.com website and then editing with Paint3d. The colours were also changed to aid visibility. 

Each window area has a different mouse cursor and so it was necessary to add the create cursor method into all relevant classes. It was not feasible to create one method and then call that from each class, since each window area had different ways of calling the system mouse methods. 

For improvement we would have allowed custom resizing of the cursors and also the ability to change the type of cursors.


</details>

<details><summary><b>Additional Features</b></summary><br>
In addition to the above features, some additional changes were made to improve the UI for visually impaired users. 

The icon size was changed in the resources class of the utils package. A line of code was added to the getIcon method which increases the size of the icons before they are returned.

To improve compatibility with screen readers the main menu items were given name attributes which can be accessed by screen reading software. In addition to this the ‘Program’ menu name was changed to the more conventional ‘File’ to assure consistency for users who rely on screen reading technology for navigation.


</details><br>

**TESTING**  
Test plan: [Quality Assurance - Test Plan](./Quality-Assurance)   
Test performed, Frequency and Outcomes: [Quality Assurance - Evaluation](./Quality-Assurance)  