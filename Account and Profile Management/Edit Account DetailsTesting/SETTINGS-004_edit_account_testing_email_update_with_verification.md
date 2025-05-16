## **SETTINGS-004:** Edit Account testing - Email Update with Verification  

> **Summary:** Verify that email update with verification works correctly, including verification email delivery  <br>

**Preconditions:** User is logged in  

Scenario 1: Update email address

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to account settings | Account settings page loads |
 | 2 | Tap "EDIT ACCOUNT DETAILS" | Account editing interface opens |
 | 3 | Enter new email address | Email field accepts input |
 | 4 | Submit with invalid email format | Validation error appears |
 | 5 | Submit with valid email | Success message appears; returns to settings |
 | 6 | Verify email update | New email displays in settings and profile |
 | 7 | Test account access | User can log in with new email |

**Post-conditions:**  
 - Email updates successfully
 - Validation works for invalid email formats
 - Account remains accessible after update