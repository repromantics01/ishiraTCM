## **ORGMGMT-008:** Surrender Requests testing - Surrender Requests List  

> **Summary:** Verify that surrender requests list displays correctly with proper request information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has multiple surrender requests in different statuses
- User has navigated to the Surrender Requests page

Scenario 1: Surrender request list display and filtering

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | View the surrender requests list | List should display all surrender requests with pet information, surrenderer name, submission date, and status | 
 | 2 | Set filter to "Pending" | List should update to show only surrender requests with "Pending" status | 
 | 3 | Set filter to "Approved" | List should update to show only surrender requests with "Approved" status | 
 | 4 | Set filter to "Rejected" | List should update to show only surrender requests with "Rejected" status | 
 | 5 | Set filter to "All" | List should update to show all surrender requests regardless of status |
 | 6 | Sort list by "Date" | List should reorder with most recent requests first |
 | 7 | Use search function to find a specific pet | List should filter to show only matching results |

**Post-conditions:**
- All surrender requests are properly displayed
- Filtering, sorting, and search functions work correctly
- List accurately reflects the current state of surrender requests in the database