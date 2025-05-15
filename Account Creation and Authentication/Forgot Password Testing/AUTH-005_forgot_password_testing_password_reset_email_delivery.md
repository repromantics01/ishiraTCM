## **AUTH-005:** Forgot Password testing - Password Reset Email Delivery  

> **Summary:** Verify that password reset email is delivered to the correct email address with valid reset link  <br>

**Preconditions:** User account exists in the system

Scenario 1: Email delivery and content validation

 | \# | Step | Expected Behavior | 
 |----|------|-------------------| 
 |  1 | Request a password reset for a registered email | The system processes the request | 
 |  2 | Check the inbox of the registered email | A password reset email is received | 
 |  3 | Verify the email content | The email contains:<br>- PawsMatch branding<br>- Clear instructions<br>- A password reset link<br>- Security information | 

**Post-conditions:**  

 - Password reset email is delivered to the correct address
 - Email contains valid and secure reset link