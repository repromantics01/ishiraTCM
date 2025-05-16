## **MSG-001:** Inbox testing - Message Threads Display  

> **Summary:** Verify that message threads display correctly with proper sender information and timestamps  <br>

**Preconditions:** 
- User is logged in
- User has existing message threads with at least one organization

Scenario 1: View message threads in inbox

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to the inbox page by tapping the message icon in the dashboard | Inbox page loads with a list of message threads |
 | 2 | Observe the threads displayed in the inbox | Each thread displays: <br> - Organization name <br> - Organization avatar/logo <br> - Preview of last message <br> - Timestamp of last message |
 | 3 | Check threads with unread messages | Threads with unread messages should be visually distinct (bold text or indicator) |
 | 4 | Check thread sorting | Threads should be sorted by most recent message first |

**Post-conditions:**  
 - All message threads are displayed correctly
 - Thread information matches the data in Firebase
 - Recent messages appear at the top of the list