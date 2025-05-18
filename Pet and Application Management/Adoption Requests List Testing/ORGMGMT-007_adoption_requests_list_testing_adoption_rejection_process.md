## **ORGMGMT-007:** Adoption Requests List testing - Adoption Rejection Process  

> **Summary:** Verify that adoption rejection process works correctly with proper status updates  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one pending adoption request
- User has navigated to the Adoption Requests page

Scenario 1: Reject an adoption request

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the details modal for a pending adoption request | Request details should be displayed with "Reject" button available | 
 | 2 | Click the "Reject" button | Dialog should appear asking for rejection reason | 
 | 3 | Enter rejection reason and click "Submit" | System should update the request status to "Rejected" in the database |
 | 4 | View the adoption requests list | The request should now show "Rejected" status |
 | 5 | Check the dashboard statistics | Pending adoption request count should decrease by one |

**Post-conditions:**
- Adoption request status is updated to "Rejected" in the database
- Dashboard statistics reflect the change
- Pet remains available for other adoption requests