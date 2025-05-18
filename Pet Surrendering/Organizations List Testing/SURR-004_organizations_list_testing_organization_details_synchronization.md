## **SURR-004:** Organizations List testing - Organization Details Synchronization  

> **Summary:** Verify that organization search functionality returns correct results based on search criteria  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User is on the Organizations Listing page
- Multiple organizations with varied names/locations exist in system

Scenario 1: Search by Organization Name

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Locate the search input field | Search field is visible at the top of organizations list |
 | 2 | Enter partial organization name | Search results update in real-time as user types |
 | 3 | Enter a name that should match multiple organizations | Multiple matching organizations are displayed |
 | 4 | Enter a name that should match exactly one organization | Only that specific organization is displayed |
 | 5 | Enter a name that shouldn't match any organization | "No results found" message is displayed |
 | 6 | Clear the search field | All organizations are displayed again |

Scenario 2: Search by Location

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Enter a location name in search field | Organizations in that location are displayed |
 | 2 | Enter partial location name | Organizations in locations containing that text are displayed |

**Post-conditions:**  
- Search results are accurate and match the search criteria
- Search functionality performs with acceptable response time
- Search is case-insensitive and handles partial matches