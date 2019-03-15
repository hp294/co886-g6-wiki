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

<details><summary><b>Sound Effect</b></summary><br>

To implement the requirements of having sound effects played to signify success or failure of a program or command entered into the Haskell Interpreter involved using the ConsoleWindow.java class and writing a new method called playSound() to play each sound based on certain events.
There is a method inside the ConsoleWndow.java class which calls the Haskell Interpreter to retrieve error information. This method contains a variable called ‘error’ that is incremented every time an error is returned. This was used to determine which sound effect should be triggered by calling the playSound() method with the sound effect name as a parameter of type String. If the error is zero then success sound is triggered, otherwise the failure sound is triggered.
To create the playSound() method 2 javax classes were utilised. These were javax.sound.sampled.AudioSystem and javax.sound.sampled.Clip. More specifically AudioSystem.getAudioInputStream() was used to retrieve a handle to the audio system, and Clip.open() and Clip.start() were used respectively to open and play a sound clip.

To retrieve the file path of the audio files independently of the computer that is being used, it was necessary to use the ClassLoader class which is part of the java.lang package. The String parameter that was passed to the playSound() method is for the name of the file to be found.
The audio files were downloaded from freesound.org
For future the improvements the playSound() method could be used to signify other notifications such as when a user hovers over a particular area.

</details>


<details><summary><b>Caret Cursor Visibility</b></summary><br>


</details><br>

<details><summary><b>Mouse Cursor Visibility</b></summary><br>


</details><br>



**TESTING**  
Test plan: [Quality Assurance - Test Plan](./Quality-Assurance)   
Test performed, Frequency and Outcomes: [Quality Assurance - Evaluation](./Quality-Assurance)  