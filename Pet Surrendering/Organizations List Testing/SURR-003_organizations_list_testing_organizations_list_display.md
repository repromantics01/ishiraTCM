## **SURR-003:** Organizations List testing - Organizations List Display  

> **Summary:** Verify that organizations list displays correctly with proper organization information  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User is authenticated in the app
- There are multiple organizations registered in the system

Scenario 1: Organizations List Loading and Display

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Navigate to Organizations Listing | Loading indicator is shown while fetching organizations |
 | 2 | Wait for organizations to load | Organizations are displayed in a list format |
 | 3 | Verify organization cards | Each organization card shows: organization logo/image, name, location, and description |
 | 4 | Scroll through the list | List scrolls smoothly, organizations load as they come into view |
 | 5 | Verify empty state | If no organizations exist, appropriate empty state message is shown |

**Post-conditions:**  
- Organization list is displayed with proper information
- Organizations are sorted according to defined criteria
- List updates automatically if changes occur in backend data