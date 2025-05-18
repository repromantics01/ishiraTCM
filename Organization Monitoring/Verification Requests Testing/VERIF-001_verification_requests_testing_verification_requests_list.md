## **VERIF-001:** Verification Requests testing - Verification Requests List  

> **Summary:** Verify that verification requests list displays correctly with all pending organization verification requests  <br>

**Preconditions:** 
- User has a valid account with moderator role
- User is authenticated in the app
- There are pending organization verification requests in system

Scenario 1: Verification Requests List Display

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Log in as a moderator | User is authenticated and redirected to moderator dashboard |
 | 2 | Select "Verification Requests" filter | List of pending organization verification requests is displayed |
 | 3 | Verify request cards | Each card shows organization name, submission date, and document preview |
 | 4 | Check for action buttons | Each request has "Verify" and "Reject" buttons |
 | 5 | Verify sorting order | Requests are sorted with oldest requests first |
 | 6 | Check empty state | If no pending requests, appropriate empty state message is shown |

**Post-conditions:**  
- Moderator can see all pending verification requests
- UI clearly differentiates between different requests
- List updates when requests are approved or rejected