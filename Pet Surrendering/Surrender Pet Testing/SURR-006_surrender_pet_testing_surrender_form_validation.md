## **SURR-006:** Surrender Pet testing - Surrender Form Validation  

> **Summary:** Verify that surrender form validation correctly identifies and displays form errors  <br>

**Preconditions:** 
- User has a valid account with the surrenderer role
- User has navigated to the Surrender Pet form
- User has selected an organization to surrender to

Scenario 1: Form Field Validation

 | # | Step | Expected Behavior | 
 |---|------|-------------------| 
 | 1 | Leave pet name field empty and try to proceed | Error message indicates pet name is required |
 | 2 | Enter invalid birthdate (future date) | Error message indicates birthdate cannot be in the future |
 | 3 | Leave species selection empty | Error message indicates species is required |
 | 4 | Leave breed field empty | Error message indicates breed is required |
 | 5 | Leave gender selection empty | Error message indicates gender is required |
 | 6 | Enter invalid weight value (negative or non-numeric) | Error message indicates weight must be a positive number |
 | 7 | Leave vaccination status selection empty | Error message indicates vaccination status is required |
 | 8 | Leave address field empty | Error message indicates address is required |
 | 9 | Enter a very short description (<10 characters) | Error message indicates minimum length requirement for description |

**Post-conditions:**  
- All validation errors are clearly displayed to the user
- Form cannot be submitted until all validation errors are resolved
- Valid inputs are accepted without error messages