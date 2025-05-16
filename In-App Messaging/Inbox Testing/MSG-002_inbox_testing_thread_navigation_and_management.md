## **MSG-002:** Inbox testing - Thread Navigation  

> **Summary:** Verify that thread navigation functions correctly  <br>

**Preconditions:**
- User is logged in
- User has at least 2 message threads

Scenario 1: Navigate to a conversation thread

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the inbox page | All message threads are listed |
 | 2 | Tap on a message thread | The selected conversation opens |
 | 3 | Observe the conversation view | Messages are displayed in chronological order with sender information |
 | 4 | Navigate back to inbox | The thread should be marked as read if it was previously unread |

**Post-conditions:**
 - Thread navigation works smoothly
 - Thread read status updates correctly in Firebase