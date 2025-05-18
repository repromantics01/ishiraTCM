## **ORGMGMT-004:** Adoption Requests List testing - Adoption Requests List  

> **Summary:** Verify that adoption requests list displays correctly with proper request information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has multiple adoption requests in different statuses
- User has navigated to the Adoption Requests page

Scenario 1: Adoption request list display and filtering

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | View the adoption requests list | List should display all adoption requests for the organization with pet name, applicant name, date submitted, and status | 
 | 2 | Set filter to "Pending" | List should update to show only adoption requests with "Pending" status | 
 | 3 | Set filter to "Approved" | List should update to show only adoption requests with "Approved" status | 
 | 4 | Set filter to "Rejected" | List should update to show only adoption requests with "Rejected" status | 
 | 5 | Set filter to "All" | List should update to show all adoption requests regardless of status |
 | 6 | Sort list by "Date" | List should reorder with most recent requests first |
 | 7 | Sort list by "Name" | List should reorder alphabetically by pet name |

**Post-conditions:**
- All adoption requests are properly displayed
- Filtering and sorting functions work correctly
- List accurately reflects the current state of adoption requests in the database

## **ORGMGMT-005:** Adoption Requests List testing - Adoption Request Details View  

> **Summary:** Verify that adoption request details view shows complete applicant and request information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one adoption request
- User has navigated to the Adoption Requests page

Scenario 1: View adoption request details

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click on an adoption request in the list | Request details modal should open | 
 | 2 | View applicant information section | Modal should display applicant's name, contact info, and address correctly |
 | 3 | View pet information section | Modal should display pet's name, species, breed, age, and photo correctly | 
 | 4 | View application details section | Modal should display application date, status, and any applicant comments |
 | 5 | Click "Close" button | Modal should close and return to the adoption requests list |

**Post-conditions:**
- Adoption request details are displayed accurately
- All information sections are properly populated with correct data
- Modal opens and closes without errors

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

## **ORGMGMT-009:** Surrender Requests testing - Surrender Request Details View  

> **Summary:** Verify that surrender request details view shows complete surrenderer and pet information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one surrender request
- User has navigated to the Surrender Requests page

Scenario 1: View surrender request details

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click on a surrender request in the list | Request details modal should open | 
 | 2 | View surrenderer information | Modal should display surrenderer's name, contact info, and address correctly |
 | 3 | View pet information section | Modal should display pet's name, species, breed, age, medical information, and photos if available | 
 | 4 | View surrender reason and details | Modal should display reason for surrender and any additional information provided by surrenderer |
 | 5 | Click "Close" button | Modal should close and return to the surrender requests list |

**Post-conditions:**
- Surrender request details are displayed accurately
- All information sections are properly populated with correct data
- Photos are displayed correctly if available
- Modal opens and closes without errors

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

## **ORGMGMT-012:** Manage Pets testing - Pets List with Filtering Options  

> **Summary:** Verify that pets list with filtering options displays correctly with proper pet information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has multiple pets with different statuses
- User has navigated to the Manage Pets page

Scenario 1: Pet list display and filtering

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | View the pets list | List should display all pets with name, breed, age, photo, and status | 
 | 2 | Set filter to "Available" | List should update to show only pets with "Available" status | 
 | 3 | Set filter to "Adopted" | List should update to show only pets with "Adopted" status | 
 | 4 | Set filter to "Pending" | List should update to show only pets with "Pending" status | 
 | 5 | Set filter to "All" | List should update to show all pets regardless of status |
 | 6 | Sort list by "Name" | List should reorder alphabetically by pet name |
 | 7 | Sort list by "Age" | List should reorder by pet age |
 | 8 | Sort list by "Recently Added" | List should reorder with most recently added pets first |
 | 9 | Use search function to find a specific pet | List should filter to show only matching results |

**Post-conditions:**
- All pets are properly displayed
- Filtering, sorting, and search functions work correctly
- List accurately reflects the current state of pets in the database

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