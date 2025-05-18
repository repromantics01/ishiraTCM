## **VERIF-003:** Verified Accounts testing - Approved Organizations List  

> **Summary:** Verify that approved organizations list displays correctly with all verified organizations  <br>

**Preconditions:** 
- User has a valid account with moderator role
- User is on the moderator dashboard
- There are verified organizations in the system

Scenario 1: Approved Organizations List View

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Select "Verified Organizations" filter | List of verified organizations is displayed |
 | 2 | Verify organization cards | Each card shows organization name, verification date, logo, and location |
 | 3 | Check for status indicators | Organizations show "Verified" status indicator |
 | 4 | Look for action buttons | Each organization has appropriate action buttons (View, Message, etc.) |
 | 5 | Verify sorting functionality | Organizations can be sorted by verification date or alphabetically |
 | 6 | Use search functionality | Organizations can be filtered by name or location |

**Post-conditions:**  
- Moderator can see all verified organizations
- List provides necessary information at a glance
- List can be sorted and filtered as needed