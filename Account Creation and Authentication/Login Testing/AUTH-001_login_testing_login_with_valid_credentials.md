## **AUTH-001:** Login testing - Login with Valid Credentials  

> **Summary:** Verify that users can log in successfully with valid credentials  <br>

**Preconditions:** User account exists in the system with verified email

Scenario 1: Adopter logs in with valid credentials

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Enter valid email/username and password for an Adopter account | Input fields accept the data | 
 |  3 | Tap the "LOGIN" button | The app shows a loading indicator while authenticating |
 |  4 | Wait for authentication to complete | User is redirected to the Adopter Dashboard | 

Scenario 2: Surrenderer logs in with valid credentials

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the login screen | The login form is displayed | 
 |  2 | Enter valid email/username and password for a Surrenderer account | Input fields accept the data | 
 |  3 | Tap the "LOGIN" button | The app authenticates the user |
 |  4 | Wait for authentication to complete | User is redirected to the Surrenderer Dashboard | 

**Post-conditions:**  

 - User is authenticated in Firebase Authentication
 - User session is created
 - User is directed to the appropriate dashboard based on their account type