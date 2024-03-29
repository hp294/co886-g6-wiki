**ACCEPTANCE CRITERIA**

| **User Story ID** | **Acceptance Criteria** | **Implemented** | **Pass/Fail** |
| ------ | ------ | ------ | ------ |
| 1 | Given I am unable to read the text <br>When I enable the screen-reader <br>Then the screen-reader will  narrate what I have highlighted | N | |
| 2 | Given I am not able to navigate the application with a mouse <br>When using keyboard shortcuts prescribed in the application manual <br>Then I can access the menu options I require | N | |
| 3 | Given I want to view the application as a visually impaired user <br>When I use the accessibility extension <br>Then the text and icons are clearly readable in all areas of the application | Y | |
| 4 | Given I find it difficult to locate the cursor as a visually impaired user <br>When I use the accessibility extension <br>Then I am able to locate the cursor with no difficulties no matter what document is displayed | Y | |
| 5 | Given I am unable to see certain colours as a colour-blind user <br>When I use the accessibility extension <br>Then problem colours (red) are removed and colour contrast is heightened. | Y | |
| 6 | Given I am used to working with the Microsoft Windows operating system <br>When using the HEAT application <br>Then I am easily able to use the functions due to my experience with Windows | Y | |
| 7 | Given I am a visually impaired user that finds it difficult to read the icon annotations <br>When I hover the cursor over icons in the HEAT app <br>Then I am able to clearly read the annotation and have ample time (10-15 seconds) to read it | N | |
| 8 | Given I am using the HEAT application for the first time <br>When attempting to link to a Haskell interpreter <br>Then I am able to navigate the files and connect with the interpreter with no difficulties | N | |
| 9 | Given I am working in the HEAT application as a visually-impaired user <br>When I attempt to run a command or compile a program <br>Then I am aware of whether it was successful or encountered an error based on the respective sound effects | Y | |
| 10 | Given I am severely visually impaired and wish to work with the HEAT application <br>When I use the voice control extension <br>Then I am able to control all aspects of HEAT as intended | N | |


**USER STORIES**

*Estimate*: 1-easy, 5-difficult  
*Priority*: M-must have, S-should have, C-could have, W-won't have

| **ID** | **User Stories** | **Estimate (Dev Effort)** | **Priority (MoSCoW analysis)** |
| ------ | ------ | ------ | ------ |
| 1 | Story: I want the device to read out words from the screen to me. <br>Details: Exploit Window Narrator by incorporating compatibility in the software. <br>Tests: Provide a number of scenarios for a user to use the screen reader on different parts of the window (menu, icon navigator, content,...). | 4 | W |
| 2 | Story: I want efficient keyboard shortcuts that will replace using mouse. <br>Details: Provide keyboard shortcuts for all menu and icon functions. <br>Tests: Provide a number of scenarios for a user to use a combination of shortcuts. | 2 | W |
| 3 | Story: I want to be able to read and see text clearer. <br>Details: Change font type and increase font size above existing max value. <br>Tests: Test a range of font sizes & type | 1 | M |
| 4 | Story: I want to be able to locate cursor easily. <br>Details: Increase cursor size/colour/reflection. <br>Tests: Find the cursor in a big text document.| 1 | M |
| 5 | Story: Story: I want to enhance/exclude certain colour. <br>Details: Change background of all windows and text colour. <br>Tests: Create and run some codes to see which colour combination works best. | 1 | M |
| 6 | Story: I want the menu to be consistent with MS Window. <br>Details: Change menu text to the standard ‘file’ rather than ‘program’. <br>Tests: Load, Amend and Save a file.| 1 | C |
| 7 | Story: I want read the icon annotation easily. <br>Details: Annotation font is small, and not on the screen long enough (6-7 sec). <br>Test: Hover on all icons to see if annotation is large and stay on the screen for long enough. | 3 | W |
| 8 | Story: I want to easily link HEAT to Haskell interpreter. <br>Details: Access to the interpreter in the menu. <br>Tests: Setup HEAT with the interpreter. | 5 | W |
| 9 | Story: I want to know when a programme runs correctly or not via sound. <br>Details: Access/failure sound effect if the programme runs correctly/incorrectly. <br>Tests: Run several valid/invalid programs.| 1 | S |
| 10 | Story: I want to use the software with my voice only. <br>Details: Implement voice control for all functions, input and output. <br>Tests: Input a program via voice and command it to run via voice. | 5 | C |
