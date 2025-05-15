## **AUTH-004:** Forgot Password testing - Password Reset Flow  

> **Summary:** Verify that password reset flow works correctly from request to confirmation  <br>  

**Preconditions:** User account exists in the system

Scenario 1: Password reset request for existing email

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Tap on "Forgot Password?" link | A password reset dialog appears | 
 |  3 | Enter a registered email address | Input field accepts the email | 
 |  4 | Tap "Send Reset Link" button | The dialog closes and a success message "Password reset email sent. Check your inbox." appears | 

Scenario 2: Password reset request for non-existent email

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Tap on "Forgot Password?" link | A password reset dialog appears | 
 |  3 | Enter an email address that is not registered | Input field accepts the email | 
 |  4 | Tap "Send Reset Link" button | An error message is displayed indicating the email is not registered | 

**Post-conditions:**  

 - For existing email: Password reset email is sent to the user
 - For non-existent email: Error message is displayed, no email is sent