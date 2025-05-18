## **VERIF-004:** Verified Accounts testing - Document Access  

> **Summary:** Verify that organization documents can be accessed and easily viewed  <br>

**Preconditions:** 
- User has a valid account with moderator role
- User is viewing a verified organization's details
- The organization has uploaded documents during verification

Scenario 1: Document Access and Viewing

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Navigate to organization's document section | List of documents is displayed with document types |
 | 2 | Tap on a document thumbnail | System leads the user to a new tab to download the prompt document download |
 | 3 | Download document | Document downloads successfully to device |
 | 4 | Return to document list | User returns to document list view |
 | 5 | Try accessing document from organization history | Previous document versions are available if updates exist |

**Post-conditions:**  
- All documents are accessible and viewable
- Documents can be inspected in detail
- Document history is preserved when updates occur