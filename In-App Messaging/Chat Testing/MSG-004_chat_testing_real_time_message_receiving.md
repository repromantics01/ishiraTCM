## **MSG-004:** Chat testing - Real-Time Message Receiving  

> **Summary:** Verify that real-time message receiving works correctly when another user sends a message  <br>

**Preconditions:**
- User A and User B are both logged in
- User A and B have an existing message thread
- User A has the conversation with User B open

Scenario 1: Receive messages in real-time

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | User B sends a message to User A | Message is sent successfully from User B's device |
 | 2 | Observe User A's conversation view | New message appears in real-time without requiring refresh |
 | 3 | Check message formatting and info | Message shows correct sender and timestamp |
 | 4 | Navigate away from the conversation | The message thread updates to show the latest message preview |

**Post-conditions:**
 - Messages are received in real-time
 - Thread previews update correctly