## **SETTINGS-003:** Edit Account testing - Password Update Functionality  

> **Summary:** Verify that password update functionality works correctly with validation and confirmation  <br>

**Preconditions:** User is logged in  

Scenario 1: Update password

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to account settings | Account settings page loads |
 | 2 | Tap "EDIT ACCOUNT DETAILS" | Account editing interface opens |
 | 3 | Enter new password | Password field accepts input; text is masked |
 | 4 | Enter mismatched confirmation password | Validation error appears when trying to submit |
 | 5 | Enter matching confirmation password | No validation error |
 | 6 | Submit with valid password | Success message appears; returns to settings |
 | 7 | Test password requirements | Too short password shows validation error |

**Post-conditions:**  
 - Password updates successfully with proper validation
 - User can log in with new password
 - Validation errors appear for invalid input