## **SETTINGS-005:** Edit Account testing - Account Deletion Process  

> **Summary:** Verify that account deletion process works correctly with proper confirmation and data removal  <br>

**Preconditions:** User is logged in; Test account is available for deletion

Scenario 1: Delete user account

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to account settings | Account settings page loads |
 | 2 | Locate account deletion option | Account deletion button or option is visible |
 | 3 | Initiate account deletion | Confirmation dialog appears with warning |
 | 4 | Cancel deletion | Dialog closes; account remains intact |
 | 5 | Reinitiate and confirm deletion | Success message appears; user is logged out |
 | 6 | Attempt to log in with deleted account | Login fails with appropriate error message |

**Post-conditions:**  
 - Account is successfully removed from the system
 - User is redirected to login or welcome screen
 - Authentication with deleted credentials fails