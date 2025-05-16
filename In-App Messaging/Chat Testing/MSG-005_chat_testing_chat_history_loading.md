## **MSG-005:** Chat testing - Chat History Loading  

> **Summary:** Verify that chat history loads correctly with proper pagination and historical messages  <br>

**Preconditions:**
- User is logged in
- User has a conversation thread with at least 30 messages

Scenario 1: Load chat history

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open a conversation with extensive history | Initial batch of messages loads (most recent ones) |
 | 2 | Scroll up in the conversation | More historical messages load as user scrolls |
 | 3 | Continue scrolling to the beginning | All historical messages eventually load |
 | 4 | Check message ordering | Messages are displayed in chronological order |
 | 5 | Check for date separators | Date separators appear between messages from different days |

Scenario 2: Conversation reloading

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Close and reopen the same conversation | Conversation position should be maintained at the latest message |
 | 2 | Check message content | All previously loaded messages should still be visible |

**Post-conditions:**
 - Chat history loads correctly with pagination
 - Message ordering is preserved
 - Date separators appear correctly
