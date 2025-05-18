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