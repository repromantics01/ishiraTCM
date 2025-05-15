## **REG-002:** Sign up testing - Organization Signup Field Validation  

> **Summary:** Verify that organization signup fields validate input correctly and show appropriate error messages

**Preconditions:** User is on the web organization signup page

**Scenario 1: Email validation**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Enter invalid email format in the email field (e.g., "test@") | Validation error displays "Please enter a valid email" |
 | 2 | Enter existing email address | System shows error message after submission "The email address is already in use" |
 | 3 | Enter valid email format | No validation error is shown |

**Scenario 2: Password validation**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Enter short password (less than 6 characters) | Validation error displays "Password must be at least 6 characters" |
 | 2 | Enter mismatched passwords in password and confirm password fields | Validation error displays "Passwords do not match" |
 | 3 | Enter valid matching passwords | No validation error is shown |

**Scenario 3: Required fields validation**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Leave username field empty and attempt to proceed | Validation error displays "Please enter your account username" |
 | 2 | Leave organization name empty in step 2 | Validation error displays "Please enter the organization name" |

**Post-conditions:**  
- Form validation prevents submission until all required fields are correctly completed
- Error messages are clearly displayed to guide the user
