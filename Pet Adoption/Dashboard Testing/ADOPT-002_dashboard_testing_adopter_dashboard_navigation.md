## **ADOPT-002:** Dashboard testing - Adopter Dashboard Navigation  

> **Summary:** Verify that adopter dashboard navigation correctly directs user to intended features  <br>

**Preconditions:**
- User is logged in as an adopter

Scenario 1: Navigation between main sections

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap on "Swiped Pets" in bottom navigation | App navigates to Swiped Pets page showing previously liked pets |
 | 2 | Tap on "Home" in bottom navigation | App returns to the main dashboard |
 | 3 | Tap on "Your Adoptions" in bottom navigation | App navigates to adoption requests page showing status of all requests |
 | 4 | Tap on message icon in top bar | App navigates to the inbox showing message threads |
 | 5 | Tap on profile icon in top bar | App navigates to profile settings page |

Scenario 2: Pet discovery navigation

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap on the pet card in dashboard | App navigates to PetSwiperPage for continuous pet discovery |
 | 2 | Navigate back from pet swiper | App returns to the dashboard |

**Post-conditions:**
 - All navigation elements direct user to correct pages
 - Navigation state is preserved when using back buttons
 - Current section is highlighted in bottom navigation