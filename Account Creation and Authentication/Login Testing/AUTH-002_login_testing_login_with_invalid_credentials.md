## **AUTH-002:** Login testing - Login with Invalid Credentials  

> **Summary:** Verify that login fails appropriately with invalid credentials and shows proper error messages  <br>

**Preconditions:** App is installed and running on device/emulator

Scenario 1: Login with non-existent email

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Enter an email that doesn't exist in the system and any password | Input fields accept the data | 
 |  3 | Tap the "LOGIN" button | The app attempts to authenticate |
 |  4 | Wait for authentication to fail | Error message "No user found with this email." is displayed | 

Scenario 2: Login with incorrect password

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Enter a valid email but incorrect password | Input fields accept the data | 
 |  3 | Tap the "LOGIN" button | The app attempts to authenticate |
 |  4 | Wait for authentication to fail | Error message "Wrong password provided." is displayed | 

Scenario 3: Login with empty fields

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Leave the email and password fields empty | No data is entered | 
 |  3 | Tap the "LOGIN" button | Form validation errors appear indicating the required fields cannot be empty | 

**Post-conditions:**  

 - User remains on the login screen
 - Appropriate error message is displayed
 - No authentication session is created