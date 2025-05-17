## **ADOPT-009:** Swiped Pets testing - Request Adoption  

> **Summary:** Verify that request adoption functionality works correctly from swiped pets list  <br>

**Preconditions:**
- User is logged in as an adopter
- User has opened detailed view of an available swiped pet

Scenario 1: Submit adoption request

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap "Adopt [Pet Name]!" button | Adoption confirmation dialog appears |
 | 2 | Review confirmation dialog | Dialog shows pet information and adoption commitment text |
 | 3 | Tap "NO" | Dialog closes, no request is submitted |
 | 4 | Reopen dialog and tap "YES" | Success dialog appears confirming request submission |
 | 5 | Check Firebase | New adoption record is created in the adopt collection with "Pending" status |
 | 6 | Check swipe record | Swipe record is updated with isActive="false" |

Scenario 2: Verify adoption request in adoption list

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to "Your Adoptions" page | Page loads with list of adoption requests |
 | 2 | Find the newly submitted request | Request appears with "Pending" status |
 | 3 | Tap on request to view details | Detailed adoption request information is displayed |

**Post-conditions:**
 - Adoption request is successfully submitted
 - Adoption record is created in Firebase
 - Swipe record is updated correctly
 - Pet no longer appears in swipe interface