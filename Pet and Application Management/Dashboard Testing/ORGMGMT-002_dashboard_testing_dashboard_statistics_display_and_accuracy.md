## **ORGMGMT-002:** Dashboard testing - Dashboard Statistics Display and Accuracy  

> **Summary:** Verify that dashboard statistics display correctly with accurate data from the database  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has existing adoption and surrender requests in the system
- User has navigated to the organization dashboard

Scenario 1: Verify statistics accuracy

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | View the total adoption requests counter | Value should match the actual total number of adoption requests for this organization in the database | 
 | 2 | View the pending adoption requests counter | Value should match the number of adoption requests with 'Pending' status for this organization | 
 | 3 | View the total surrender requests counter | Value should match the actual total number of surrender requests for this organization in the database | 
 | 4 | View the pending surrender requests counter | Value should match the number of surrender requests with 'Pending' status for this organization |
 | 5 | Create a new adoption request in another session | Dashboard should update to reflect the new request count (may require page refresh) |

**Post-conditions:**
- All statistics are verified to be accurate
- Dashboard properly reflects the current state of the database
- Statistics update correctly when data changes