## **SETTINGS-002:** Display User testing - Settings Menu Navigation  

> **Summary:** Verify that settings menu navigation works correctly between different settings sections  <br>

**Preconditions:** User is logged in  

Scenario 1: Navigate between settings sections

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open user settings | Settings overview page loads |
 | 2 | Tap "EDIT ACCOUNT DETAILS" | Account editing interface opens |
 | 3 | Tap back button | Returns to main settings page |
 | 4 | Tap "EDIT PROFILE DETAILS" | Profile editing interface opens |
 | 5 | Test back navigation | Back button returns to settings overview |
 | 6 | Test top back button | Back button in header returns to previous screen |

**Post-conditions:**  
 - Navigation between settings sections works smoothly
 - Back buttons function as expected
 - State is preserved when returning to previous screens