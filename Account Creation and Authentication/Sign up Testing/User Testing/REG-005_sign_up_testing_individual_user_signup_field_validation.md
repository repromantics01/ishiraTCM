## **REG-005:** Sign up testing - Individual User Signup Field Validation  

> **Summary:** Verify that individual user signup fields validate input correctly and show appropriate error messages  <br>

**Preconditions:** App is installed and running on device/emulator

Scenario 1: Empty field validation

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the signup screen | The signup form is displayed | 
 |  2 | Leave all fields empty and tap the "SIGN UP" button | Error messages appear under each required field indicating they cannot be empty | 

Scenario 2: Email format validation

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Enter a valid username and passwords but an invalid email format (e.g., "testuser") | No immediate validation error is shown | 
 |  2 | Tap the "SIGN UP" button | An error message appears indicating the email is not valid | 

Scenario 3: Password mismatch validation

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Enter a valid username and email | Fields accept the input | 
 |  2 | Enter "password123" in the password field and "password456" in the confirm password field | No immediate validation error is shown | 
 |  3 | Tap the "SIGN UP" button | An error message appears indicating the passwords do not match | 

Scenario 4: Password length validation

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Enter a valid username and email | Fields accept the input | 
 |  2 | Enter "pass" in both password fields (less than 6 characters) | No immediate validation error is shown | 
 |  3 | Tap the "SIGN UP" button | An error message appears indicating the password must be at least 6 characters long | 

**Post-conditions:**  

 - No user account is created when validation fails
 - The user remains on the signup screen with error messages displayed