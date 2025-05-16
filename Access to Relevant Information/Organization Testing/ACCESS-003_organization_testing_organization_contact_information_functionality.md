## **ACCESS-003:** Organization testing - Organization Contact Information Functionality  

> **Summary:** Verify that organization contact information functions correctly when interacted with (email links, phone links)  <br>

**Preconditions:** User is logged in; Internet connection is available  

Scenario 1: Interact with contact information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to organization profile's contact section | All contact information displays properly |
 | 2 | Tap on email address | Email app opens with pre-filled recipient field |
 | 3 | Tap on phone number | Phone app opens with number pre-filled |
 | 4 | Tap on social media icons | Proper app or browser opens to the social media page |
 | 5 | Test "Send Message" button | Chat interface opens with the organization as recipient |

**Post-conditions:**  
 - All contact links function properly
 - External apps open as expected when contact methods are tapped
 - Message thread is created when "Send Message" is tapped