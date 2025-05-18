## **SURR-002:** Dashboard testing - Surrenderer Dashboard Navigation  

> **Summary:** Verify that surrenderer dashboard navigation correctly directs user to intended features  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User is authenticated in the app
- User has completed dashboard loading

Scenario 1: Navigation Between Main Sections

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Tap on "Swiped Pets" in bottom navigation | User is navigated to the Swiped Pets page |
 | 2 | Tap on "Home" in bottom navigation | User is navigated back to the Dashboard home page |
 | 3 | Tap on "Your Adoptions" in bottom navigation | User is navigated to the View Adoptions page |
 | 4 | Tap on message icon in header | User is navigated to the Inbox page |
 | 5 | Tap on profile icon in header | User is navigated to the Profile and Account Settings page |
 | 6 | Tap on "Edit Profile Details" in profile card | User is navigated to the Profile and Account Settings page |

**Post-conditions:**  
- Navigation state is preserved when returning to previous screens
- Current selection is visually indicated in bottom navigation
- Navigation transitions are smooth without errors
