## **AUTH-003:** Login testing - Login Persistence Across App Restarts  

> **Summary:** Verify that login session persists across app restarts and maintains authentication state  <br>

**Preconditions:** User has successfully logged in to the application

Scenario 1: Session persistence after app restart

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Successfully log in as an Adopter or Surrenderer | User is on the appropriate dashboard | 
 |  2 | Force close the application | The app is terminated | 
 |  3 | Relaunch the application | The app should bypass the login screen and navigate directly to the user's dashboard | 

Scenario 2: Session persistence after device restart

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Successfully log in as a user | User is authenticated and on the dashboard | 
 |  2 | Restart the device | Device powers down and restarts | 
 |  3 | Launch the application after device restart | User should remain logged in and be directed to their dashboard | 

**Post-conditions:**  

 - User remains authenticated after app or device restart
 - Firebase Authentication token is properly stored and retrieved