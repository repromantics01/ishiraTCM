## **ORGMGMT-015:** Manage Pets testing - Pet Status Update Functionality  

> **Summary:** Verify that pet status update functionality works correctly with proper status transitions  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has pets in various statuses
- User has navigated to the Manage Pets page

Scenario 1: Update pet status

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open details for an "Available" pet | Pet details should display with status update options | 
 | 2 | Change status to "Adopted" | Confirmation dialog should appear |
 | 3 | Confirm the status change | Pet status should update to "Adopted" in the database | 
 | 4 | View the pets list | Pet should now appear with "Adopted" status |
 | 5 | Open details for a "Pending" pet | Pet details should display with status update options |
 | 6 | Change status to "Available" | Confirmation dialog should ask to confirm cancelling pending adoption |
 | 7 | Confirm the status change | Pet should return to "Available" status and related adoption requests should be updated |

**Post-conditions:**
- Pet status is updated correctly in the database
- Status changes trigger appropriate updates to related adoption requests
- Pets list displays the updated status
- Any dependent processes (adoptions, availability) are updated accordingly