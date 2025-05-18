## **ORGMGMT-011:** Surrender Requests testing - Surrender Rejection Process  

> **Summary:** Verify that surrender rejection process works correctly with proper status updates <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one pending surrender request
- User has navigated to the Surrender Requests page

Scenario 1: Reject a surrender request

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the details modal for a pending surrender request | Request details should be displayed with "Reject" button available | 
 | 2 | Click the "Reject" button | Dialog should appear asking for rejection reason | 
 | 3 | Enter rejection reason and click "Submit" | System should update the request status to "Rejected" in the database |
 | 4 | View the surrender requests list | The request should now show "Rejected" status |
 | 5 | Check the dashboard statistics | Pending surrender request count should decrease by one |

**Post-conditions:**
- Surrender request status is updated to "Rejected" in the database
- Dashboard statistics reflect the change
- Pet is not added to the organization's pet inventory