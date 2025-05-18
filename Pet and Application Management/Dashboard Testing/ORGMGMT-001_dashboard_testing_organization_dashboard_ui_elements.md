## **ORGMGMT-001:** Dashboard testing - Organization Dashboard UI Elements  

> **Summary:** Verify that organization dashboard UI elements display correctly and are properly positioned  <br>

**Preconditions:** 
- User is logged in as an organization account
- Organization account is verified and active
- User has navigated to the organization dashboard page

Scenario 1: Verify Dashboard UI elements and layout

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | View the organization dashboard | Dashboard should display with sidebar navigation and main content area | 
 | 2 | Observe the sidebar navigation elements | Sidebar should contain: Dashboard, Manage Pets, Surrender Requests, Adoption Requests, Messages, and Organization Profile options | 
 | 3 | Observe the dashboard statistics area | Statistics area should display total adoption requests, pending adoption requests, total surrender requests, and pending surrender requests | 
 | 4 | Check the adoption and surrender table | Table should display monthly data for both adoption and surrender trends over the last 6 months | 

**Post-conditions:**  
- All dashboard UI elements are verified to be displaying correctly
- No visual anomalies or layout issues are detected
- Dashboard statistics are properly loaded from database