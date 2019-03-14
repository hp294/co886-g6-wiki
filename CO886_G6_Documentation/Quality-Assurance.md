**Test Plan for the HEAT Accessibility Function**<br>

**1. Objectives**<br>

**1.1 Purpose**<br>

This document details the plan for testing the extended accessibility functions for the HEAT application. The document supports the following objectives:<br>
*  Identify the areas marked for testing.<br>
*  List the recommended test requirements.<br>
*  Recommend and describe the testing strategies to be employed.<br>

**1.2 Test Scope**<br>

This plan assumes that the HEAT application has already undergone extensive testing procedures. Therefore testing will be limited to the components within the system that have been extended for improved accessibility for visually-impaired users.<br>

The system components to be tested are:<br>

1. Colour and contrast within the editor,console and tree window.<br>
2. Sound effects denoting success and failure with regard to command execution and program compilation.<br>
3. Icon size.<br>
4. Font size and font type.<br>
5. Text cursor size and colour in console window.<br>

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
Verify cursor size and colour within console window.

**2.3 Validation Testing**

Validate developments against user requirement documentation.<br>
Validate developments through user testing.<br>

**2.4 Performance Testing**

Verify functionality of developments in combination.<br>

**3. Test Strategy**<br>

This section presents recommended approaches to the testing of the accessibility extensions. It will reiterate the techniques to be used as listed in the previous section and describe the process and completion criteria for each technique.

**3.1 Unit Testing**

Due to the collaborative nature of the project, with different people working on separate accessibility functions, the components listed in 1.2 should initially be tested as individual units before a full system test.

*3.1.1 Colour and contrast testing*

Test objective: Ensure all changes in text colour/contrast and background colour/contrast has 



























   * Tests: 
     * Unit Testing
     * Junit Test
     * Acceptance Criteria Testing
     * User Testing
     * Code Quality Testing(?)

[<b>Acceptance Criteria](https://git.cs.kent.ac.uk/co886/g6/wikis/CO886_G6_Documentation/User-Stories)   
**Definition**   
**Evaluation**       

https://git.cs.kent.ac.uk/help/user/project/merge_requests/sast.md    
https://git.cs.kent.ac.uk/help/ci/README.md   
https://git.cs.kent.ac.uk/help/user/project/merge_requests/dependency_scanning.md   
https://git.cs.kent.ac.uk/help/user/project/merge_requests/dast.md   
https://git.cs.kent.ac.uk/help/user/project/security_dashboard   
https://git.cs.kent.ac.uk/help/ci/junit_test_reports.md   
https://git.cs.kent.ac.uk/help/user/project/merge_requests/code_quality.md   
https://docs.gitlab.com/ee/ci/examples/code_quality.html     
https://docs.gitlab.com/ee/ci/examples/end_to_end_testing_webdriverio/index.html   