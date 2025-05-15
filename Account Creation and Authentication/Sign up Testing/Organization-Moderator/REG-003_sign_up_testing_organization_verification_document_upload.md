## **REG-003:** Sign up testing - Organization Verification Document Upload  

> **Summary:** Verify that organization verification documents can be uploaded and stored correctly

**Preconditions:** User is on step 2 of organization signup

**Scenario 1: Document upload functionality**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Click on upload area for proof of validation | File picker dialog opens | 
 | 2 | Select multiple valid files (.pdf, .jpg, .png) | Files are selected and displayed in the upload area with file names |
 | 3 | Navigate to step 3 and submit the form | Files are uploaded to storage without errors |

**Scenario 2: Document type restrictions**

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Attempt to upload an unsupported file type (e.g., .exe or .zip) | File picker only shows supported file types OR system rejects the upload with appropriate message |
 | 2 | Upload extremely large files (>10MB) | System shows a size limit message |

**Post-conditions:**  
- Documents are successfully uploaded to storage
- Document references are stored with the organization record
- Uploaded files can be retrieved by moderators for verification
