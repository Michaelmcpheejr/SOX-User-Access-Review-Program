# SOP: User Access Review Control (ITGC_UAR01)

## 1. Control Name and ID

- Control Name: User Access Review for SOX Relevant Applications  
- Control ID: ITGC_UAR01  

## 2. Purpose and Control Objective

Purpose:  
Ensure user and privileged access is reviewed on a recurring basis and documented to support SOX ITGC audit expectations.

Control objective:  
Confirm that access to financial and SOX impacting systems is restricted to authorized users based on job responsibilities and that privileged access is formally reviewed and adjusted where inappropriate.

## 3. Scope and Frequency

Scope:

- Azure Entra ID
- M365 admin roles
- SSO integrated SOX relevant applications
- Privileged groups and elevated access pathways
- Application owners certify access for their applications

Frequency:

- Privileged access reviews: monthly
- General user access reviews: quarterly

## 4. Roles and Responsibilities

IT Compliance:

- Coordinate the review calendar and collect exports
- Maintain the Access Review Tracker
- Ensure completeness and follow up on missing responses
- Validate remediation tickets are opened and closed
- Finalize the evidence binder for each period

Application owners:

- Review and certify user access for their application
- Update Status, Action Required, and Business Justification or Notes
- Confirm completion of required removals or modifications

IAM or IT Operations:

- Implement access changes based on review decisions
- Close remediation tickets and provide proof where needed

Internal or External Audit:

- May request samples and re perform the control using the tracker and evidence

## 5. Inputs and Data Sources

- Access exports from in scope applications and identity platforms
- Access Review Tracker template
- Ticketing system for remediation tracking
- Evidence repository location for the SOX ITGC binder

## 6. Detailed Procedure

1. Identify in scope applications and owners  
   - Maintain an inventory of SOX relevant applications and identity platforms.  
   - Confirm the application owner or business owner for each system.  

2. Extract user access from in scope applications  
   - Generate access reports that list users and roles for each in scope system.  
   - Validate that the reports are complete for the period and environment.  

3. Load data into the Access Review Tracker  
   - Normalize exports into the tracker format:  
     - User  
     - Application Needed  
     - Role  
     - Privileged (Y or N)  
     - Risk Rating  
   - Pre populate Privileged and initial Risk Rating where possible.  

4. Send tracker to application owners for review  
   - Filter or segment the tracker by Application Needed.  
   - Provide each owner with their portion of the data plus instructions and due dates.  

5. Application owners review access and update tracker  
   - For each user, the owner updates:  
     - Status (Certified, Removed, Modified, Pending)  
     - Action Required (None, Remove, Modify, Investigate)  
     - Business Justification or Notes  
   - Owners identify access that should be removed or reduced.  

6. IT creates tickets for any Action Required  
   - IT Compliance or IAM reviews rows where Action Required is not None.  
   - Open remediation tickets in the ticketing system.  
   - Record each ticket number in the Ticket Number or Remediation Ticket column.  

7. Close tickets and update the tracker  
   - IAM or IT Operations implement the changes and close tickets.  
   - IT Compliance updates Status to reflect completion (Removed or Modified).  
   - Track any overdue or pending changes for follow up.  

8. Finalize and store evidence  
   - Save the final Access Review Tracker.  
   - Store access listings, tracker, owner certifications, and remediation evidence in the binder structure defined in `Evidence_Binder_Standard.md`.  

## 7. Documentation and Evidence Requirements

- Raw access listings for each in scope system
- Final Access Review Tracker for the period
- Application owner certifications for each system
- Remediation ticket exports and closure evidence
- Exception approvals where access is kept despite risk

## 8. Exceptions and Escalation

- Define what qualifies as an exception (example, access kept with acknowledged risk).  
- Exceptions require approval from security leadership or governance.  
- Overdue reviews or open high risk remediation items are escalated to management.

## 9. Record Retention

- Retain all evidence per the SOX retention policy, for example 7 years.  
- Ensure evidence remains accessible for future audits covering the review period.

