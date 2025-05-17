## **ADOPT-011:** View Adoptions testing - Adoption Status Updates  

> **Summary:** Verify that adoption status updates are reflected correctly on the adoption applications list  <br>

**Preconditions:**
- User is logged in as an adopter with pending adoption requests
- Admin/organization user has ability to update adoption status

Scenario 1: Status update reflection

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Admin updates an adoption request status to "Approved" | Status is updated in Firebase |
 | 2 | User navigates to "Your Adoptions" page | Page loads with updated status |
 | 3 | Check the updated application | Status shows "Approved" with green color |
 | 4 | Open detailed view of approved application | Details show approval date and next steps |

Scenario 2: Approved adoption actions

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open details of an approved adoption | Details page opens with approved status |
 | 2 | Check for "Message Organization" button | Button is visible for approved adoptions |
 | 3 | Tap "Message Organization" button | Navigates to conversation with the organization |
 | 4 | Send a message | Message is delivered to the organization |

**Post-conditions:**
 - Status updates are reflected correctly in the UI
 - Appropriate actions are available based on status
 - Communication channel opens for approved adoptions
