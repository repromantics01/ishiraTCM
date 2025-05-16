## **ACCESS-005:** Pet testing - Pet Photo Carousel Functionality  

> **Summary:** Verify that pet photo carousel functions correctly with proper navigation between photos  <br>

**Preconditions:** User is logged in; Pet with multiple photos exists  

Scenario 1: Navigate through pet photos

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Open a pet profile with multiple photos | First photo displays at the top with pagination dots below |
 | 2 | Count pagination dots | Number of dots matches number of available photos |
 | 3 | Swipe left on the photo | Next photo displays with smooth transition |
 | 4 | Check active pagination dot | Second dot is now highlighted |
 | 5 | Swipe through all photos | All photos display correctly with proper transitions |
 | 6 | Test fallback for failed images | Temporarily disable internet and verify placeholder appears instead of broken images |

**Post-conditions:**  
 - Photo carousel navigates smoothly between all pet photos
 - Active photo is correctly indicated by pagination dots
 - Error states are handled gracefully