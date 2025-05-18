## **ORGMGMT-006:** Adoption Requests List testing - Adoption Approval Process  

> **Summary:** Verify that adoption approval process works correctly with proper status updates   <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one pending adoption request
- User has navigated to the Adoption Requests page

Scenario 1: Approve an adoption request

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the details modal for a pending adoption request | Request details should be displayed with "Approve" button available | 
 | 2 | Click the "Approve" button | Confirmation dialog should appear asking to confirm approval | 
 | 3 | Click "Confirm" in the dialog | System should update the request status to "Approved" in the database |
 | 4 | View the adoption requests list | The approved request should now show "Approved" status |
 | 5 | Check the dashboard statistics | Pending adoption request count should decrease by one |

**Post-conditions:**
- Adoption request status is updated to "Approved" in the database
- Dashboard statistics reflect the change
- Pet status is updated to "Pending" if it was "Available"