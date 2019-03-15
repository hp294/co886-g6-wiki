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

Font size and type specification within the program is distributed and implemented using several methods. The font specifications needed to be amended in the SettingsManager, WindowManager, MainMenu and OptionsWindow classes. The object of the amendment was to either change existing code, adapt code or add code.The implementation of existing fonts was fragmented and distributed in an appararently haphazard manner. This may be explained because when writing the original code the coders were unaware that subsequently a team would be changing the font type and sizes.<br>

In the SettingsManager class two lines of code were amended to increase the font size to 20. In the WindowManager class one line of code was added using setFont from the java.awt.Font API, changing the font size. In the MainMenu class numerous lines of code were amended to the new font. It was also necessary to amend the code for the undo and redo options (Using JFrame) in order to change the font (JMenuItem). In the OptionsWindow class numerous lines of code had to be adapted. The code used the JLabel method of JFrame. The original code did not include font details. This meant that every time text was displayed one line of existing code needed to be replaced by three.<br>

The amended code will result in larger text size and a font type that is easier to read, by visually impaired users. The implementation has been partially successful with most text changed to Arial and a high font size. There are a number of areas where it was not possible to change the font type or size, for example in pre-filled forms, option tab buttons and the font type in the editor and console windows.The implementation of these items would need considerable research to understand how they are implemented in order to amend the font size and type.</details>


<details><summary><b>Colour & Contrast</b></summary><br>


</details>


<details><summary><b>Sound Effect</b></summary><br>


</details>


<details><summary><b>Cursor Visibility</b></summary><br>


</details><br>


**TESTING**  
Test plan: [Quality Assurance - Test Plan](./Quality-Assurance)   
Test performed, Frequency and Outcomes: [Quality Assurance - Evaluation](./Quality-Assurance)  