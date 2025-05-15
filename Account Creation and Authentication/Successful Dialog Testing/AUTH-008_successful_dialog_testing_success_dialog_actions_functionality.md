## **AUTH-008:** Success Dialog testing - Success Dialog Actions Functionality  

> **Summary:** Verify that success dialog actions (dismiss, continue, etc.) function correctly when interacted with  <br>

**Preconditions:** Success dialog is displayed after an operation

Scenario 1: Continue to login from success dialog

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | View the success dialog after registration | Success dialog is displayed with "Continue to Login" button | 
 |  2 | Tap the "Continue to Login" button | A smooth transition animation plays and user is redirected to the login screen | 

Scenario 2: Testing success dialog on different screen sizes

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Run the app on a small screen device (e.g., iPhone SE) | Success dialog renders correctly with all elements visible and properly sized | 
 |  2 | Run the app on a large screen device (e.g., tablet) | Success dialog renders correctly with proper scaling of elements | 

**Post-conditions:**  

 - User can navigate from success dialog to the appropriate next screen
 - Dialog displays correctly across different device sizes