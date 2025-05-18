## **ORGMGMT-013:** Manage Pets testing - New Pet Addition  

> **Summary:** Verify that new pet addition works correctly and creates a pet record with proper validation  <br>

**Preconditions:**
- User is logged in as an organization account
- User has navigated to the Manage Pets page

Scenario 1: Add a new pet with valid information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click "Add New Pet" button | New pet form modal should open | 
 | 2 | Enter pet name, species, breed, gender, birthdate | Form should accept valid input |
 | 3 | Enter pet description, behavioral information | Text areas should accept multi-line input | 
 | 4 | Set vaccination status and neutered/spayed status | Toggle buttons should update accordingly |
 | 5 | Upload pet photos | Photos should be previewed and upload indicators should show success |
 | 6 | Click "Save" button | System should validate all required fields and save pet to database |
 | 7 | View pets list | Newly added pet should appear in the list with "Available" status |

Scenario 2: Validation error handling

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click "Add New Pet" button | New pet form modal should open | 
 | 2 | Leave required fields empty | Form should not allow submission |
 | 3 | Enter invalid data (e.g., future birthdate) | Form should display validation errors |
 | 4 | Fix all validation errors and click "Save" | Pet should be saved correctly |

**Post-conditions:**
- New pet is added to the database with correct information
- Pet appears in the organization's pets list with "Available" status
- Photos are properly stored and associated with the pet
- Pet is available for adoption by potential adopters