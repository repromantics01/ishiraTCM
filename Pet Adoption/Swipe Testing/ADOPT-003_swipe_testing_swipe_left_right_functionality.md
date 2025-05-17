## **ADOPT-003:** Swipe testing - Swipe Left/Right Functionality  

> **Summary:** Verify that swipe left/right functionality works correctly to like or reject pets  <br>

**Preconditions:**
- User is logged in as an adopter
- User is on the PetSwiperPage

Scenario 1: Swipe gestures

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Swipe a pet card to the right | "LIKE" indicator appears, pet card animates off-screen |
 | 2 | Observe next pet card | Next pet in queue appears with animation |
 | 3 | Swipe a pet card to the left | "NOPE" indicator appears, pet card animates off-screen |
 | 4 | Check Firebase | Swipe action (like/dislike) is recorded in the swipes collection |

Scenario 2: Button actions

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap the like button (heart icon) | Same behavior as right swipe, pet is marked as liked |
 | 2 | Tap the dislike button (X icon) | Same behavior as left swipe, pet is marked as disliked |
 | 3 | Check swiped pets list after liking | Liked pet appears in the swiped pets list |

**Post-conditions:**
 - Swipe actions are correctly recorded in Firebase
 - Liked pets appear in the swiped pets list
 - Animation transitions work smoothly