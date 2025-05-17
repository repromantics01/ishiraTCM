## **ADOPT-004:** Swipe testing - Pet Filtering Effects  

> **Summary:** Verify that pet filtering affects which pets are shown in the swipe interface  <br>

**Preconditions:**
- User is logged in as an adopter
- User has previously liked some pets
- User has pending adoption requests for some pets

Scenario 1: Automatic filtering

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open the PetSwiperPage | Only pets that haven't been swiped are shown |
 | 2 | Swipe through multiple pets | Previously liked or disliked pets don't reappear |
 | 3 | Check pets with pending adoptions | Pets with active adoption requests don't appear in swipe interface |

Scenario 2: Empty state handling

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Swipe through all available pets | Empty state UI appears with appropriate message |
 | 2 | Close and reopen the app | Empty state persists until new pets are added |

**Post-conditions:**
 - Pet filtering works correctly to avoid showing duplicates
 - Pets with pending adoptions don't appear in swipe interface
 - Empty state is handled gracefully