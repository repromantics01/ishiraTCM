## **AUTH-006:** Forgot Password testing - Setting a New Password After Reset  

> **Summary:** Verify that users can set a new password after clicking the reset link and the new password works for login  <br>

**Preconditions:** User has received a password reset email

Scenario 1: Complete password reset process

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Open the password reset email and click the reset link | A web page opens with password reset form | 
 |  2 | Enter a new password and confirm it | Password fields accept the input | 
 |  3 | Submit the form | A confirmation message appears that the password has been reset | 
 |  4 | Go to the mobile app and try to login with the new password | The login is successful and user is directed to their dashboard | 

Scenario 2: Password validation during reset

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Open the password reset email and click the reset link | A web page opens with password reset form | 
 |  2 | Enter a short password (less than 6 characters) | An error message appears indicating password requirements | 
 |  3 | Enter a valid password but different values in password and confirm password fields | An error message appears indicating the passwords do not match | 

**Post-conditions:**  

 - User's password is successfully updated in Firebase Authentication
 - Previous password no longer works for authentication
 - New password enables successful login