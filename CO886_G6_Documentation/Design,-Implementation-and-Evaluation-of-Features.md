**Font Visibility**

Font size and type specification within the program is distributed and implemented using several methods. The font specifications needed to be amended in the SettingsManager, WindowManager, MainMenu and OptionsWindow classes. The object of the amendment was to either change existing code, adapt code or add code.The implemention of existing fonts was frahgmented and distributed in a haphazard manner. When writing the ode the original coders were unaware thayt subsequently a team would be changing the font type and sizes.

In the SettingsManager class two lines of code were amended to increase the font size to 20. In the WindowManager class one line of code was added using setFont from the java.awt.Font API, changing the font size. In theMainMenu class numerous lines of code were amended to the new font. It was also necessary to amend the code for the undo and redo options (Using JFrame) in order to change the font (JMenuItem). 

  



**Design** 
**Implementation**   
[Branches](https://git.cs.kent.ac.uk/co886/g6/branches)   
[Commits](https://git.cs.kent.ac.uk/co886/g6/commits/master)   
[Contribution](https://git.cs.kent.ac.uk/co886/g6/graphs/master)   

**Evaluation**   