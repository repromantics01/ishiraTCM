## **ACCESS-002:** Organization testing - Organization Photos and Logo Display  

> **Summary:** Verify that organization photos and logo display correctly with proper formatting and layout  <br>

**Preconditions:** User is logged in; Internet connection is available  

Scenario 1: View organization profile with multiple photos

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to organization profile | Top image carousel loads with first photo |
 | 2 | Check pagination dots | Number of pagination dots matches number of available photos |
 | 3 | Swipe to next photo | Carousel transitions smoothly to next photo |
 | 4 | Check logo display | Logo appears in circular container at top left |


**Post-conditions:**  
 - All images display correctly
 - Carousel navigation functions properly
 - Placeholder images appear when actual images fail to load

