## **SETTINGS-006:** Edit Profile testing - Personal Information Update  

> **Summary:** Verify that personal information update works correctly and saves changes to the database  <br>

**Preconditions:** User is logged in  

Scenario 1: Update personal information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to profile settings | Settings page loads |
 | 2 | Tap "EDIT PROFILE DETAILS" | Profile editing interface opens |
 | 3 | Update first name, last name fields | Fields accept new input |
 | 4 | Update address information | Address field accepts new input |
 | 5 | Submit changes | Loading indicator appears; success message displays |
 | 6 | Return to profile view | Updated information displays correctly |
 | 7 | Test required field validation | Removing required fields shows validation errors |

**Post-conditions:**  
 - Profile information updates successfully
 - Updated information is visible in profile view
 - Validation works for required fields