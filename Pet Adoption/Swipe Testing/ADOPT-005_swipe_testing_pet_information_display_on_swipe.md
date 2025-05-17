## **ADOPT-005:** Swipe testing - Pet Information Display on Swipe  

> **Summary:** Verify that pet information displays correctly on swipe cards with proper formatting  <br>

**Preconditions:**
- User is logged in as an adopter
- User is on the PetSwiperPage

Scenario 1: Pet card information verification

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Observe an individual pet card | Pet image is visible at the top of the card |
 | 2 | Check pet details section | Displayed details include: name, age, species, breed, gender |
 | 3 | Check pet location | Address/location is displayed with location icon |
 | 4 | Verify organization section | Posted by organization name and logo are visible |
 | 5 | Check multiple pet cards | All cards consistently display information in the same format |

Scenario 2: Detailed pet view

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap on the pet card content (not swipe) | Detailed view of pet opens |
 | 2 | Check detailed information | Additional details appear: description, medical information, etc. |
 | 3 | Verify photo gallery | If multiple photos exist, gallery navigation works |

**Post-conditions:**
 - Pet information displays correctly on swipe cards
 - All required pet details are visible
 - Image loading works correctly