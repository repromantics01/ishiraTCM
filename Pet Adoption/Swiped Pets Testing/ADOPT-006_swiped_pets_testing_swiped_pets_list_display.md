## **ADOPT-006:** Swiped Pets testing - Swiped Pets List Display  

> **Summary:** Verify that swiped pets list displays correctly with all liked pets  <br>

**Preconditions:**
- User is logged in as an adopter
- User has liked at least 3 pets

Scenario 1: View swiped pets list

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to Swiped Pets page | Page loads with grid of previously liked pets |
 | 2 | Check pet information on cards | Each card shows pet image, name, breed, and age |
 | 3 | Compare with Firebase data | All pets marked as liked in Firebase appear in the list |
 | 4 | Pull to refresh the list | List refreshes and shows any newly liked pets |

Scenario 2: Empty state handling

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Create a new test user with no liked pets | No swiped pets exist for this user |
 | 2 | Navigate to Swiped Pets page | Empty state UI appears with message and "Find Pets" button |
 | 3 | Tap "Find Pets" button | Navigates to pet discovery interface |

**Post-conditions:**
 - Swiped pets list displays all liked pets correctly
 - Pet information matches Firebase data
 - Empty state is handled gracefully