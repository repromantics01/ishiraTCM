## **VERIF-002:** Verification Requests testing - Verification Request Details View  

> **Summary:** Verify that verification request details view shows all necessary information for verification decisions  <br>

**Preconditions:** 
- User has a valid account with moderator role
- User is on the moderator dashboard
- There is at least one pending organization verification request

Scenario 1: View Verification Request Details

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Select a verification request from the list | Request details view opens |
 | 2 | Verify organization details section | Organization name, email, address, and phone are displayed |
 | 3 | Verify documents section | All uploaded documents are displayed with preview options |
 | 4 | Open a document for detailed view | Document opens in full-screen view with zoom capability |
 | 5 | Verify organization description | Organization description, mission, and services are displayed |
 | 6 | Check admin information | Admin names and contact information are displayed |
 | 7 | Check approval/rejection controls | "Verify" and "Reject" buttons are prominently displayed |

**Post-conditions:**  
- Moderator has all necessary information to make verification decision
- All documents can be reviewed in detail
- Actions can be taken directly from the details view