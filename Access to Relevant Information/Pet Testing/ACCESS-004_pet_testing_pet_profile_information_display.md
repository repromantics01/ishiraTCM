## **ACCESS-004:** Pet testing - Pet Profile Information Display  

> **Summary:** Verify that pet profile information displays correctly and completely on profile page  <br>

**Preconditions:** User is logged in; Pet data exists in database  

Scenario 1: View pet profile

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to a pet's profile page | Pet profile loads with header image |
 | 2 | Check pet name and basic info | Name displays in large font; gender, age and location display correctly |
 | 3 | Verify status badge | Appropriate status badge (Available, Adopted, Pending) displays with correct color |
 | 4 | Check "About Pet" section | Pet description displays in the gray box with proper formatting |
 | 5 | Verify "More About" details | Details section displays species, breed, gender, age, and origin correctly |
 | 6 | Check health information | Spay/neuter status and vaccination information display correctly |
 | 7 | Verify organization posting info | Organization name and logo that posted the pet display correctly |

**Post-conditions:**  
 - All pet information displays correctly
 - Status badge shows the current adoption status with appropriate color
 - Text is properly formatted and readable