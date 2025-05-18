## **ORGMGMT-003:** Dashboard testing - Dashboard Sidebar Navigation Flow  

> **Summary:** Verify that dashboard navigation correctly directs user to intended features  <br>

**Preconditions:**
- User is logged in as an organization account
- User is currently on the organization dashboard page

Scenario 1: Sidebar navigation functionality

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click on "Manage Pets" in the sidebar | Application should navigate to the Manage Pets page | 
 | 2 | Click on "Dashboard" in the sidebar | Application should navigate back to the main dashboard | 
 | 3 | Click on "Surrender Requests" in the sidebar | Application should navigate to the Surrender Requests page | 
 | 4 | Click on "Adoption Requests" in the sidebar | Application should navigate to the Adoption Requests page | 
 | 5 | Click on "Messages" in the sidebar | Application should navigate to the Messages page | 
 | 6 | Click on "Organization Profile" in the sidebar | Application should navigate to the Organization Profile page |
 | 7 | Use browser back button | Application should navigate to the previously visited page correctly |

**Post-conditions:**
- All navigation flows function correctly
- Current page is highlighted in the sidebar navigation
- No navigation errors are encountered