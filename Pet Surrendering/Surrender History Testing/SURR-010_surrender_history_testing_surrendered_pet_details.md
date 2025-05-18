## **SURR-0011:** Surrender History testing - Surrendered Pet Details  

> **Summary:** Verify that surrendered pet details show complete information about the surrender request  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User has at least one surrender request in history

Scenario 1: Viewing Surrender Details

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Navigate to Surrender History | List of previous surrender requests is displayed |
 | 2 | Tap on a specific surrender request | Detailed view of surrender request opens |
 | 3 | Verify pet information | Pet name, species, breed, age, gender, and photos are displayed |
 | 4 | Verify surrender details | Surrender date, reason, organization name, and status are displayed |
 | 5 | Verify organization contact | Organization contact information is available if request is accepted |
 | 6 | Check status history | Status changes and timestamps are displayed in chronological order |
 | 7 | If request is rejected, verify reason | Rejection reason provided by organization is displayed |

**Post-conditions:**  
- Complete surrender request details are visible to user
- User can navigate back to surrender history list
- User can contact organization if request is accepted