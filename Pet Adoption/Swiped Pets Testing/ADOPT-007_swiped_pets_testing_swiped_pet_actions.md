## **ADOPT-007:** Swiped Pets testing - Swiped Pet Actions  

> **Summary:** Verify that swiped pet actions function correctly (view details, request adoption)  <br>

**Preconditions:**
- User is logged in as an adopter
- User has at least one pet in their swiped pets list

Scenario 1: View pet details from swiped list

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap on a pet in the swiped pets list | Detailed SwipedPetProfile view opens |
 | 2 | Check detailed information | All pet details are displayed correctly |
 | 3 | Navigate back to swiped pets list | Returns to grid view of swiped pets |

Scenario 2: View organization profile

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open a pet's detailed view | Swiped Pet Profile view opens |
 | 2 | Tap on the organization section | Adopter's Organization Profile view opens |
 | 3 | Check organization details | Organization information displays correctly |
 | 4 | Navigate back to pet profile | Returns to pet profile view |

**Post-conditions:**
 - Pet detail view functions correctly
 - Organization profile view functions correctly
 - Navigation between views works smoothly