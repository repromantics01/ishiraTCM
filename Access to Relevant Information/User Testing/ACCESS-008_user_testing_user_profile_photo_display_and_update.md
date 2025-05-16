## **ACCESS-008:** User testing - User Profile Photo Display and Update  

> **Summary:** Verify that user profile photo displays correctly and can be updated through the interface  <br>

**Preconditions:** User is logged in; Internet connection is available  

Scenario 1: Update profile photo

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to profile editing interface | Profile edit page loads with current photo or placeholder |
 | 2 | Tap the edit icon on profile image | File picker opens to select a new image |
 | 3 | Select a valid image file | Image preview appears, showing selected photo |
 | 4 | Submit the profile update | Loading indicator appears during upload |
 | 5 | Return to profile view | New profile image displays correctly |
 | 6 | Test error handling | Try uploading an invalid file and verify appropriate error message |

**Post-conditions:**  
 - Profile photo updates successfully
 - New photo is visible across the application
 - Error states are handled gracefully