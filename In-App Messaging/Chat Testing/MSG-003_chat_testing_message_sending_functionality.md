## **MSG-003:** Chat testing - Message Sending Functionality  

> **Summary:** Verify that message sending functionality works correctly with text appearing in the conversation  <br>

**Preconditions:**
- User is logged in
- User has opened a conversation thread

Scenario 1: Send a new message

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Type a message in the text input field | Text appears in the input field |
 | 2 | Tap the send button | Message sends successfully |
 | 3 | Observe the conversation | New message appears in the conversation with correct formatting |
 | 4 | Check the sender information | Message shows correct sender name and timestamp |

Scenario 2: Handle sending errors

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Put device in airplane mode | Device disconnects from network |
 | 2 | Attempt to send a message | App should indicate failure to send message |
 | 3 | Turn off airplane mode | Device reconnects to network |
 | 4 | Retry sending the message | Message should send successfully |

**Post-conditions:**
 - Messages are sent correctly
 - Messages are displayed correctly in the conversation
 - Messages are saved correctly in Firebase
 - Error handling works as expected