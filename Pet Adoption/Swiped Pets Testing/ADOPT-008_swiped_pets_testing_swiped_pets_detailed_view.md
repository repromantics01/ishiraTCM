## **ADOPT-008:** Swiped Pets testing - Swiped Pets Detailed View  

> **Summary:** Verify that swiped pets detailed view shows complete pet information  <br>

**Preconditions:**
- User is logged in as an adopter
- User has opened detailed view of a swiped pet

Scenario 1: Verify comprehensive pet information

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Observe pet image section | Main image displays with page indicators if multiple photos exist |
 | 2 | Check basic information | Name, age, gender, and address display correctly |
 | 3 | Verify "About" section | Pet description text displays properly |
 | 4 | Check "Pet Details" section | Species, breed, gender, age appear in formatted table |
 | 5 | Check "Medical Information" section | Vaccination status and neutered/spayed status display correctly |
 | 6 | Verify photo gallery | Multiple photos can be scrolled through if available |

Scenario 2: Test pet status indicators

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Check pet availability status | Status indicator shows "Available for adoption", "Pending", or "Adopted" |
 | 2 | Verify status styling | Status has appropriate color coding (green for available, orange for pending, blue for adopted) |

**Post-conditions:**
 - All pet information displays correctly and completely
 - Multiple photos can be viewed if available
 - Status indicators accurately reflect the pet's current status