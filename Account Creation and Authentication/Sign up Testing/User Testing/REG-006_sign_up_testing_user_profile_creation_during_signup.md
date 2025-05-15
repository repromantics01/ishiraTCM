## **REG-006:** Sign up testing - User Profile Creation During Signup  

> **Summary:** Verify that user profile is created correctly during the signup process with default values  <br>

**Preconditions:** App is installed and running on device/emulator with network connectivity

Scenario 1: Profile creation with default values

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Complete the signup process with valid data as an Adopter | User is redirected to the success dialog | 
 |  2 | Verify the profile document in Firestore database | A profile document is created with the following default values:<br>- account_id matches the user's UID<br>- profile_id matches the user's UID<br>- user_type is set to "Adopter"<br>- first_name, middle_name, last_name, suffix, bio, and address are empty strings<br>- date_created is set to current time | 

Scenario 2: Profile creation for Surrenderer

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Complete the signup process with valid data as a Surrenderer | User is redirected to the success dialog | 
 |  2 | Verify the profile document in Firestore database | A profile document is created with user_type set to "Surrenderer" | 

**Post-conditions:**  

 - Profile document exists in database with correct structure and default values
 - User can later edit their profile to update the empty fields