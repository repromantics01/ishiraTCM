## **ACCESS-006:** Pet testing - Pet Health Information Display  

> **Summary:** Verify that pet health information displays correctly with appropriate formatting and details  <br>

**Preconditions:** User is logged in; Pet with health data exists  

Scenario 1: View pet health information

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to pet profile | Pet profile loads with health information section |
 | 2 | Check spayed/neutered status | Status displays correctly as "Yes" or "No" |
 | 3 | Verify vaccination status | Vaccination status shows as "Full", "Partial", or "None" with appropriate styling |
 | 4 | Test different vaccination statuses | Visit profiles of pets with different vaccination statuses to verify proper display |
 | 5 | Check medical information title | "Medical Information" title appears above the health details section |

**Post-conditions:**  
 - Health information displays accurately
 - Different health statuses are visually distinguishable
 - Information is formatted clearly and consistently