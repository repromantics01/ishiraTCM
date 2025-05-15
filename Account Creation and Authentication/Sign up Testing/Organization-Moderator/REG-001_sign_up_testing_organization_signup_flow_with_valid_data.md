# PawsMatch Application Test Cases

## **REG-001:** Sign up testing - Organization Signup Flow with Valid Data  

> **Summary:** Verify that organization signup flow completes successfully with valid data  

**Preconditions:** 
- User has a valid email address
- User is on the web organization signup page

**Scenario 1: Complete 3-step organization registration flow**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Navigate to organization signup page | Page loads correctly displaying step 1 of signup | 
 | 2 | Enter valid username, email, password, and confirm password | Form accepts input without validation errors | 
 | 3 | Click "NEXT" button | User is directed to step 2 (Organization details) | 
 | 4 | Enter valid organization name | Field accepts input | 
 | 5 | Upload PDF file as proof of validation | File is successfully attached to form | 
 | 6 | Click "NEXT" button | User is directed to step 3 (Additional details) | 
 | 7 | Fill in location, address, about, contact number fields | Fields accept input | 
 | 8 | Add mission statement, operating hours | Fields accept input | 
 | 9 | Upload organization logo | Logo is displayed in preview | 
 | 10 | Click "SUBMIT" button | Success dialog appears with message that verification will take 8-12 hours |

**Post-conditions:**  
- User account is created in Firebase Authentication
- Organization details are stored in Firestore
- Uploaded documents are stored in storage
- Organization status is set to "pending verification"

