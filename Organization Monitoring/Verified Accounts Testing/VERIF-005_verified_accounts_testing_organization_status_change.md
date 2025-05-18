## **VERIF-005:** Verified Accounts testing - Organization Modified Details  

> **Summary:** Verify that registered organization's modified details syncs into the moderator view <br>

**Preconditions:** 
- Organization account is verified in the system
- Organization has updated their details 
- Moderator account has access to view organization details

Scenario 1: Verify Data Synchronization After Organization Updates

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Log in as moderator | Moderator dashboard is displayed |
 | 2 | Navigate to verified organizations list | List of verified organizations is displayed |
 | 3 | Select an organization that has recently updated information | Organization details page opens |
 | 4 | Check modification timestamp | Last update time is displayed and matches the time of recent changes |
 | 5 | Verify updated fields | Updated information is displayed correctly in moderator view |
 | 6 | Check history of changes | If implemented, change history shows what was modified and when |
 | 7 | Verify documents section | If documents were updated, new versions are available |

**Post-conditions:**  
- Moderator view reflects the most recent organization details
- Changes are tracked with appropriate timestamps
- Document updates are properly versioned and accessible