## **SURR-008:** Surrender Pet testing - Pet Photo Upload for Surrenders  

> **Summary:** Verify that pet photo upload for surrenders works correctly and attaches photos to the surrender request  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User has navigated to the Surrender Pet form
- User has filled in required text fields

Scenario 1: Photo Upload Functionality

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Tap on "Add Photo" button | Device's file picker or camera options appear |
 | 2 | Select an image from device gallery | Image is uploaded and preview appears in the form |
 | 3 | Tap on "Add Another Photo" | Device's file picker or camera options appear again |
 | 4 | Select a second image | Second image is uploaded and previewed alongside first image |
 | 5 | Tap on delete icon for first image | Confirmation dialog appears |
 | 6 | Confirm deletion | First image is removed, second image remains |
 | 7 | Try to upload a very large image (>10MB) | Error message indicates file size limit |
 | 8 | Try to upload a file that is not an image | Error message indicates invalid file type |

**Post-conditions:**  
- Uploaded photos are associated with the surrender request
- Photos are stored in the database/storage
- Photos can be viewed after submission in surrender history