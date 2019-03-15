<details><summary><b>Test Plan for the HEAT Accessibility Function</b></summary><br>

**1. Objectives**<br>

**1.1 Purpose**<br>

This document details the plan for testing the extended accessibility functions for the HEAT application. The document supports the following objectives:<br>
*  Identify the areas marked for testing.<br>
*  List the recommended test requirements.<br>
*  Recommend and describe the testing strategies to be employed.<br>

**1.2 Test Scope**<br>

This plan assumes that the HEAT application has already undergone extensive testing procedures. Therefore testing will be limited to the components within the system that have been extended for improved accessibility for visually-impaired users. Note: due to the trivial change in the HEAT task bar (changing the "Program" heading to "File" to be consistent with the Windows task bar), it was deemed unnecessary to test this function formally. <br>

The system components to be tested are:<br>

1. Colour and contrast within the editor,console and tree window.<br>
2. Sound effects denoting success and failure with regard to command execution and program compilation.<br>
3. Icon size.<br>
4. Font size and font type.<br>
5. Cursor size and colour.<br>

The critical performance measures to test are:<br>

1. Functionality of colour and contrast changes within the system.<br>
2. User response to colour and contrast modification.<br>
3. Functionality of implemented sound effects.<br>
4. User response to sound effects.<br>
5. Functionality of increased icon size implementation.<br>
6. User response to modified icon size.<br>
7. Functionality of increased font size and font type implementation.<br>
8. User response to modified font size and type.<br>
9. Functionality of increased cursor size and colour implementation.
10. User response to modified cursor.

**2. Test Requirements**<br>

This section details which testing techniques will be implemented in order to satisfy the testing scope.<br>

**2.1 Unit Testing**

Verify colour and contrast modification.<br>
Verify sound effect inclusion.<br>
Verify icon size modification.<br>
Verify font size and type modification.<br>
Verify cursor size and colour.

**2.3 Validation Testing**

Validate developments against user requirement documentation.<br>
Validate developments through user testing.<br>

**2.4 Performance Testing**

Verify functionality of developments in combination.<br>

**3. Test Strategy**<br>

This section presents recommended approaches to the testing of the accessibility extensions. It will reiterate the techniques to be used as listed in the previous section and describe the process and completion criteria for each technique.

**3.1 Unit Testing**

Due to the collaborative nature of the project, with different people working on separate accessibility functions, the components listed in 1.2 should initially be tested as individual units before a full system test, the testing will be white box and any defects will be recorded before attempts made to fix them.

**3.1.1 Colour and contrast testing**

Test objectives:<br> 

Ensure that...<br>
1. All red text has been removed from the application.
2. Text colour sharpness has been increased for all colours.
3. Background colour has been changed from white to black in all viewing windows.
4. All black text has been changed to white to contrast with the background.
5. The editor window highlight bar has been changed from yellow to grey.
 
Tests:<br>
1. Invoke errors through an incorrect command and a compilation failure to check for red text.
2. Open and compile noughts and crosses program in original HEAT application and extended version. Inspect colour differences between the two.
3. Expand tree window, console window and editor window to check background colour.
4. Inspect original version and extended version, check that no text is missing.
5. Insert code into editor window and use highlight bar to scroll. Check it remains grey.

**3.1.2 Sound effect testing**

Test objectives:<br> 

Ensure that...<br>
1. Success sound plays for successful commands and compilations.
2. Error sound plays for unsuccessful commands and compilations.
3. Success and error sounds are clear and distinct.
 
Tests:<br>
1. The success sound plays for successful commands and compilations.
2. The Error sound plays for unsuccessful commands and compilations.
3. The success and error sounds are clear and distinct.

**3.1.3 Icon size testing**

Test objectives:<br> 

Ensure that...<br>
1. All icons in the application have increased in size 
 
Tests:<br>
1. Inspect icons in the original version of the application and the extended version. Check all icons are larger in the extended version.

**3.1.4 Font size and font type**

Test objectives:<br> 

Ensure that...<br>
1. All font sizes throughout the application have been increased.
2. All font type has been altered to Arial.
 
Tests:<br>
1. Inspect font in the original version of the application and the extended version. Check all fonts are in Arial and that the text is larger in the extended version.

**3.1.5 Cursor size and contrast**

Test objectives:<br> 

Ensure that...<br>
1. The cursor size has increased throughout the application.
2. The cursor colour has changed to maintain high contrast with the application background.
 
Tests:<br>
1. Inspect cursor size in the original version of the application and the extended version. Check cursor is larger in the extended version.
2. Move cursor through each area of the application (console window, tree window, editor window, toolbar) and check cursor maintains size and background contrast.

**Completion Criteria**
1. All planned tests have been executed.
2. All identified defects have been addressed.

**3.2 Validation Testing**

Due to the accessibility extension being highly dependent on user acceptance, extensive testing must be done with the end user in mind. This stage is a combination of final development testing and user testing and will act as a "hand-over" to the user within controlled conditions.

Test Objectives:<br>

Validate the functions implemented for the accessibility extension against the original user requirements created through user stories, customer interviews and use case diagrams.

Tests:

Testing is dependent on the  [<b>Acceptance Criteria](https://git.cs.kent.ac.uk/co886/g6/wikis/CO886_G6_Documentation/User-Stories)   

1. Task a developer with completing the assessment criteria against the accessibility extension version of Heat.
2. Task a user with doing the same.

**Completion Criteria**
The acceptance criteria has passed all tests for both developer and user.

**3.3 Performance Testing**

The performance testing verifies all components of the accessibility function in combination. This is a black box test and is less constrictive than the unit testing and validation testing phases. The testing should be done by a variety of users and feedback should be recorded. Feedback will be evaluated and any modifications will be prioritised dependent on feasibility and time constraints. All modifications must undergo the same testing journey as the other extension components. 

**References**<br>
[1]https://sceweb.uhcl.edu/helm/RUP_course_example/courseregistrationproject/artifacts/test/plans/test_plan_arch.htm
[2]https://git.cs.kent.ac.uk/help/ci/junit_test_reports.md  
</details>




  


</details> 

<details><summary><b>Test Evaluation</b></summary><br>
Some pictures may not load correctly. Please refresh or click on the unloaded image, it should open in a separate window.<br>
<details><summary><b>Unit Testing</b></summary><br>

**Tester: David**<br>
![david_unit_test](uploads/30a349449985f522cfdb6de0c77a1850/david_unit_test.jpg)

**Tester: Wes**<br>
![sound_effects_unit_testing](uploads/75ec71d4af7e82c9a361db6e65babe98/sound_effects_unit_testing.jpg)
![cursor_unit_testing](uploads/8c3e98890b6684836b4c61801232ca4f/cursor_unit_testing.jpg)
</details>

<details><summary><b>Validation Testing</b></summary><br>

**Acceptance Criteria Test**<br>
**User: Tomas**<br>

| **User Story ID**| **Acceptance Criteria** | **Pass/Fail** |
| ------ | ------ | ------ |
| 3 | Given I want to view the application as a visually impaired user<br> When I use the accessibility extension<br> Then the text and icons are clearly readable in all areas of the application | Fail |
| 4 | Given I find it difficult to locate the cursor as a visually impaired user<br> When I use the accessibility extension<br> Then I am able to locate the cursor with no difficulties no matter what document is displayed | Pass |
| 5 | Given I am unable to see certain colours as a colour-blind user<br> When I use the accessibility extension<br> Then problem colours (red) are removed and colour contrast is heightened | Pass |
| 6 | Given I am used to working with the Microsoft Windows operating system<br> When using the HEAT application<br> Then I am easily able to use the functions due to my past experience with the Windows OS | Pass |
| 9 | Given I am working in the application as a visually-impaired user<br> When I attempt to run a command or compile a program<br> Then I am aware of whether it was successful or encountered an error based on the respective sound effects | Pass | 

Test #3 failed due to the user noticing that the "Status" icon in the far right of the application was still at the original font size and therefore inconsistent with the rest of the application. This defect was fixed so that the status icon is now consistent with the font size modifications made throughout the rest of the application.

**User: Terry**<br>

| **User Story ID**| **Acceptance Criteria** | **Pass/Fail** |
| ------ | ------ | ------ |
| 3 | Given I want to view the application as a visually impaired user<br> When I use the accessibility extension<br> Then the text and icons are clearly readable in all areas of the application | Pass |
| 4 | Given I find it difficult to locate the cursor as a visually impaired user<br> When I use the accessibility extension<br> Then I am able to locate the cursor with no difficulties no matter what document is displayed | Pass |
| 5 | Given I am unable to see certain colours as a colour-blind user<br> When I use the accessibility extension<br> Then problem colours (red) are removed and colour contrast is heightened | Pass |
| 6 | Given I am used to working with the Microsoft Windows operating system<br> When using the HEAT application<br> Then I am easily able to use the functions due to my past experience with the Windows OS | Pass |
| 9 | Given I am working in the application as a visually-impaired user<br> When I attempt to run a command or compile a program<br> Then I am aware of whether it was successful or encountered an error based on the respective sound effects | Pass |


</details>
<details><summary><b>Performance Testing</b></summary><br>

**David development test**

![david_dev_test_for_performance](uploads/956ca978bf0fa009994c8e52184de496/david_dev_test_for_performance.jpg)
![Laura_performance_feedback](uploads/37a02b829b4442f7666f71bb5e01d3e8/image.png)
![Tomas_performance_feedback](uploads/0c7fbbbeb5eafe71eaddc87b45ed17a5/Tomas_performance_feedback.jpg)
</details>
</details> 
