## **ORGMGMT-014:** Manage Pets testing - Pet Information Editing  

> **Summary:** Verify that pet information editing works correctly and updates pet details in the database  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one pet in the system
- User has navigated to the Manage Pets page

Scenario 1: Edit existing pet information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click "Edit" on an existing pet | Edit pet form should open with current pet information pre-filled | 
 | 2 | Modify pet name, breed, description | Form should accept changes to these fields |
 | 3 | Update vaccination status | Toggle should update to the new selection | 
 | 4 | Upload additional photos | New photos should be previewed and added to existing photos |
 | 5 | Remove an existing photo | Selected photo should be removed from the preview |
 | 6 | Click "Save Changes" button | System should validate and save updated information to database |
 | 7 | View the pet details | All changes should be reflected in the pet details view |

**Post-conditions:**
- Pet information is updated in the database
- Pet details view shows the updated information
- Photo changes (additions/deletions) are properly applied
- No data loss occurs for unmodified fields