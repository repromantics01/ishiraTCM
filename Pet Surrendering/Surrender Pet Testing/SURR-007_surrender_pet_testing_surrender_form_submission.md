## **SURR-007:** Surrender Pet testing - Surrender Form Submission  

> **Summary:** Verify that surrender form submission works correctly and creates a surrender request  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User has selected an organization to surrender to
- User has filled all required fields with valid data

Scenario 1: Successful Form Submission

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Fill all required fields with valid data | All fields accept input without validation errors |
 | 2 | Upload at least one pet photo | Photo is previewed after upload |
 | 3 | Tap submit button | Loading indicator is shown during submission |
 | 4 | Wait for submission to complete | Success confirmation dialog appears |
 | 5 | Tap "OK" or equivalent on success dialog | User is redirected to surrender history page |
 | 6 | Check surrender history | The new surrender request appears in the surrender history list |

Scenario 2: Network Error During Submission

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Fill all required fields with valid data | All fields accept input without validation errors |
 | 2 | Turn off internet connection | Device disconnects from internet |
 | 3 | Tap submit button | Loading indicator is shown briefly |
 | 4 | Wait for error handling | Error message appears indicating network connectivity issue |
 | 5 | Turn internet connection back on | Device reconnects to internet |
 | 6 | Tap submit button again | Form submits successfully |

**Post-conditions:**  
- Surrender request is stored in the database
- Organization receives notification of new surrender request
- Surrenderer can view the request in their surrender history