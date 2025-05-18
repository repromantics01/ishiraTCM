## **SURR-009:** Surrender History testing - Surrender History List  

> **Summary:** Verify that surrender history list displays correctly with all past surrender requests  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User has submitted at least one surrender request previously

Scenario 1: Surrender History Display

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Navigate to Surrender History | Loading indicator is shown while fetching surrender history |
 | 2 | Wait for history to load | List of previous surrender requests is displayed |
 | 3 | Verify surrender request cards | Each card shows: pet name, photo, surrender date, and status |
 | 4 | Check status indicators | Different statuses (Pending, Accepted, Rejected) have distinct visual indicators |
 | 5 | Verify chronological order | Requests are sorted with most recent at the top |
 | 6 | Pull down to refresh | List refreshes and shows any updates to status |

**Post-conditions:**  
- All surrender history is visible to user
- Status updates are reflected in real-time or after refresh
- List shows empty state if no surrender history exists