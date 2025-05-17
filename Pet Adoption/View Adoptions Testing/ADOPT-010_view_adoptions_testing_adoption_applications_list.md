## **ADOPT-010:** View Adoptions testing - Adoption Applications List  

> **Summary:** Verify that adoption applications list displays correctly with status indicators  <br>

**Preconditions:**
- User is logged in as an adopter
- User has submitted at least one adoption request

Scenario 1: View adoption applications list

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Navigate to "Your Adoptions" page | Page loads with list of adoption requests |
 | 2 | Check list information | Each item shows: pet image, name, status, and submission date |
 | 3 | Check different status types | Status indicators show different colors based on status (pending, approved, rejected, etc.) |
 | 4 | Use filter dropdown | List filters to show only selected status type |

Scenario 2: Sort and filter options

 | # | Step | Expected Behavior | 
 |----|------|-------------------| 
 | 1 | Tap on filter dropdown | Filter options appear (All, Pending, Approved, Rejected, etc.) |
 | 2 | Select "Pending" filter | Only pending applications are shown |
 | 3 | Select "All" filter | All applications are shown again |
 | 4 | Check default sorting | Applications are sorted by date (newest first) |

**Post-conditions:**
 - Adoption applications list displays correctly
 - Status indicators show correct colors and text
 - Filter and sort functions work correctly