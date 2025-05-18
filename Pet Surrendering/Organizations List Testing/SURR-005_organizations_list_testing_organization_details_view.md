## **SURR-005:** Organizations List testing - Organization Details View  

> **Summary:** Verify that organization details view shows complete organization information  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User is on the Organizations Listing page
- At least one organization exists in the system

Scenario 1: View Organization Profile

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Tap on an organization card | User is navigated to the organization's profile page |
 | 2 | Verify organization images | Organization images are displayed in a carousel at the top |
 | 3 | Verify organization name and logo | Organization name and logo are displayed correctly |
 | 4 | Verify address information | Full address is displayed with location icon |
 | 5 | Verify "About Us" section | Organization description is shown in the About Us section |
 | 6 | Verify "Mission" section | Organization mission statement is displayed |
 | 7 | Verify "Services Offered" section | List of services offered by the organization is displayed correctly |
 | 8 | Verify "Operating Hours" section | Weekday and weekend hours are displayed |
 | 9 | Verify "Contact/Visit Us" section | Contact information (email, phone, etc.) is displayed correctly |
 | 10 | Verify "Connect With Us" section | Social media links are displayed if available |
 | 11 | Tap on "SEND MESSAGE" button | User is navigated to conversation page with this organization |

**Post-conditions:**  
- Complete organization details are available to the user
- Links (email, phone, social media) are functional
- User can navigate back to organizations list