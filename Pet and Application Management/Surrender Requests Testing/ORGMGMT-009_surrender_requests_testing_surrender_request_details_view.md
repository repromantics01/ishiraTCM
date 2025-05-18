## **ORGMGMT-009:** Surrender Requests testing - Surrender Request Details View  

> **Summary:** Verify that surrender request details view shows complete surrenderer and pet information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one surrender request
- User has navigated to the Surrender Requests page

Scenario 1: View surrender request details

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click on a surrender request in the list | Request details modal should open | 
 | 2 | View surrenderer information | Modal should display surrenderer's name, contact info, and address correctly |
 | 3 | View pet information section | Modal should display pet's name, species, breed, age, medical information, and photos if available | 
 | 4 | View surrender reason and details | Modal should display reason for surrender and any additional information provided by surrenderer |
 | 5 | Click "Close" button | Modal should close and return to the surrender requests list |

**Post-conditions:**
- Surrender request details are displayed accurately
- All information sections are properly populated with correct data
- Photos are displayed correctly if available
- Modal opens and closes without errors