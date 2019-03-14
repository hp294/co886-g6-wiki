**Font Visibility**

Font size and type specification within the program is distributed and implemented using several methods. The font specifications needed to be amended in the SettingsManager, WindowManager, MainMenu and OptionsWindow classes. The object of the amendment was to either change existing code, adapt code or add code.The implementation of existing fonts was fragmented and distributed in an appararently haphazard manner. This may be explained because when writing the original code the coders were unaware that subsequently a team would be changing the font type and sizes.

In the SettingsManager class two lines of code were amended to increase the font size to 20. In the WindowManager class one line of code was added using setFont from the java.awt.Font API, changing the font size. In the MainMenu class numerous lines of code were amended to the new font. It was also necessary to amend the code for the undo and redo options (Using JFrame) in order to change the font (JMenuItem). In the OptionsWindow class numerous lines of code had to be adapted. The code used the JLabel method of JFrame. The original code did not include font details. This meant that every time text was displayed one line of existing code needed to be replaced by three.

The amended code will result in larger text size and a font type that is easier to read, by visually impaired users. The implementation has been partially successful with most text changed to Arial and a high font size. There are a number of areas where it was not possible to change the font type or size, for example in pre-filled forms, option tab buttons and the font type in the editor and console windows.The implementation of these items would need considerable research to understand how they are implemented in order to amend the font size and type.

  



**Design** 
**Implementation**   
[Branches](https://git.cs.kent.ac.uk/co886/g6/branches)   
[Commits](https://git.cs.kent.ac.uk/co886/g6/commits/master)   
[Contribution](https://git.cs.kent.ac.uk/co886/g6/graphs/master)   

**Evaluation**   