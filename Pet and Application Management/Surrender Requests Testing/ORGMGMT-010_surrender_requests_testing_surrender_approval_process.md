## **ORGMGMT-010:** Surrender Requests testing - Surrender Approval Process  

> **Summary:** Verify that surrender approval process works correctly with proper status updates <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one pending surrender request
- User has navigated to the Surrender Requests page

Scenario 1: Approve a surrender request

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the details modal for a pending surrender request | Request details should be displayed with "Approve" button available | 
 | 2 | Click the "Approve" button | Confirmation dialog should appear asking to confirm approval | 
 | 3 | Click "Confirm" in the dialog | System should update the request status to "Approved" in the database |
 | 4 | View the surrender requests list | The approved request should now show "Approved" status |
 | 5 | Navigate to Manage Pets page | The surrendered pet should appear in the organization's pet list with "Available" status |

**Post-conditions:**
- Surrender request status is updated to "Approved" in the database
- Pet is added to the organization's available pets list
- Pet is available for adoption by potential adopters