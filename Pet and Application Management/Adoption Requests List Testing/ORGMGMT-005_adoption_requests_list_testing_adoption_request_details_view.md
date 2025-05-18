## **ORGMGMT-005:** Adoption Requests List testing - Adoption Request Details View  

> **Summary:** Verify that adoption request details view shows complete applicant and request information  <br>

**Preconditions:**
- User is logged in as an organization account
- Organization has at least one adoption request
- User has navigated to the Adoption Requests page

Scenario 1: View adoption request details

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Click on an adoption request in the list | Request details modal should open | 
 | 2 | View applicant information section | Modal should display applicant's name, contact info, and address correctly |
 | 3 | View pet information section | Modal should display pet's name, species, breed, age, and photo correctly | 
 | 4 | View application details section | Modal should display application date, status, and any applicant comments |
 | 5 | Click "Close" button | Modal should close and return to the adoption requests list |

**Post-conditions:**
- Adoption request details are displayed accurately
- All information sections are properly populated with correct data
- Modal opens and closes without errors