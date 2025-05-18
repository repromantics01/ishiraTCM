## **SURR-001:** Dashboard testing - Surrenderer Dashboard UI Elements  

> **Summary:** Verify that surrenderer dashboard UI elements display correctly and are properly positioned  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User is authenticated in the app
- User has stable internet connection  

Scenario 1: Dashboard Layout Verification

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Log in as a surrenderer user | User is authenticated and redirected to the dashboard | 
 | 2 | Observe the top section of the dashboard | "Hello, [username]" appears at the top of the screen with correct username |
 | 3 | Verify profile card section | Profile card shows user profile image (or fallback), display name, and email address with proper styling |
 | 4 | Check "Start Matching" section | "Start Matching" title and pet card are displayed below profile section |
 | 5 | Verify pet card UI elements | Pet card shows pet image, name, age, species, breed, and action buttons |
 | 6 | Verify bottom navigation | Bottom navigation has 3 buttons: Swiped Pets, Home, Your Adoptions with correct icons |
 | 7 | Check header icons | Message and Profile icons are visible in the header area |

**Post-conditions:**  
- All UI elements are displayed with proper styling
- All elements are correctly positioned on screen
- No layout overflow or rendering issues observed
- UI is responsive to different screen sizes