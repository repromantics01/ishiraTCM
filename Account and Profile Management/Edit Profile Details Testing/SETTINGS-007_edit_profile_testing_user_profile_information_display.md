## **SETTINGS-007:** Edit Profile testing - User Profile Information Display  

> **Summary:** Verify that user profile information displays correctly after updates are made  <br>

**Preconditions:** User is logged in; Profile has been updated recently  

Scenario 1: View updated profile

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to profile view after update | Profile page loads with updated information |
 | 2 | Check profile image updates | New profile image displays if updated |
 | 3 | Verify name updates | Updated name displays correctly |
 | 4 | Check address updates | Updated address displays correctly |
 | 5 | Test persistence after logout | Log out and back in; verify changes persist |

**Post-conditions:**  
 - All profile updates display correctly
 - Changes persist across app navigation and logout/login
 - Information formatting is consistent
