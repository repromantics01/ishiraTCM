## **REG-004:** Sign up testing - Individual User Signup Flow with Valid Data  

> **Summary:** Verify that individual user signup flow completes successfully with valid data  <br>

**Preconditions:** App is installed and running on device/emulator with network connectivity

Scenario 1: User completes signup as an Adopter with valid information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the signup screen | The signup form is displayed with fields for username, email, password, confirm password, and user type selection | 
 |  2 | Enter a valid username, email address, and matching passwords (at least 6 characters long) | Input fields accept the data without validation errors | 
 |  3 | Select "Adopter" as the user type | User type is set to "Adopter" | 
 |  4 | Tap the "SIGN UP" button | The app shows a loading indicator while processing the request |
 |  5 | Wait for the signup process to complete | User is redirected to the success dialog indicating account creation and verification email is sent |
 |  6 | Check the provided email address | A verification email is received with a valid verification link |

**Post-conditions:**  

 - User account is created in Firebase Authentication
 - Account document is created in the database with correct type (AccountType.User)
 - Profile document is created with UserType.Adopter
 - Verification email is sent to the provided email address

Scenario 2: User completes signup as a Surrenderer with valid information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Launch the application and navigate to the signup screen | The signup form is displayed | 
 |  2 | Enter a valid username, email address, and matching passwords | Input fields accept the data without validation errors | 
 |  3 | Select "Surrenderer" as the user type | User type is set to "Surrenderer" | 
 |  4 | Tap the "SIGN UP" button | The signup process is initiated |
 |  5 | Wait for the signup process to complete | User is redirected to the success dialog with verification instructions |

**Post-conditions:**  

 - User account is created in Firebase Authentication
 - Account document is created in the database with correct type (AccountType.User)
 - Profile document is created with UserType.Surrenderer
 - Verification email is sent to the provided email address