# SOX User Access Review Program (ITGC_UAR01)

## Overview

This User Access Review Program is an audit ready, reusable SOX ITGC solution for organizations that want to bring security and compliance to identity and application access. It implements a formal User Access Review control (ITGC_UAR01) aligned to SOX ITGC practices and integrates automation to deliver an end to end control that auditors can re perform and security teams can rely on.

At the governance level, the program clearly defines scope, roles, ownership, and operations for reviewing both standard and privileged access across Azure Entra ID, M365 admin roles, and SOX relevant applications. At the process level, it provides a detailed SOP, a reusable Access Review Tracker, and a structured evidence binder that aligns to ITGC control expectations. At the technical layer, it uses a scheduled PowerShell driven export that generates weekly privileged access snapshots from Azure Entra ID, feeding the monthly reviews and giving incident responders an accurate timeline of who had elevated access during specific time periods.

## What is Included

- Program charter for the SOX User Access Review control (ITGC_UAR01)
- SOX ITGC User Access Review SOP
- Access Review Tracker template
- Evidence binder structure and naming standard
- Privileged access governance add on
- Automation concept for weekly privileged access snapshots from Azure Entra ID
- Framework mapping to SOX ITGC, NIST SP 800 53, and ISO 27001

## Tracker Columns

The Access Review Tracker template uses these locked columns:

- User
- Application Needed
- Role
- Privileged (Y or N)
- Risk Rating
- Action Required
- Business Justification or Notes
- Ticket Number or Remediation Ticket
- Reviewer
- Review Date
- Status

Example Status values: Certified, Removed, Modified, Pending.

## How to Use This Repo

1. Start with `docs/Program_Charter_ITGC_UAR01.md` for the program foundation.
2. Review the control operation in `docs/SOP_ITGC_UAR01_User_Access_Review.md`.
3. Use `templates/Access_Review_Tracker_Template.csv` as your base tracker.
4. Follow `docs/Evidence_Binder_Standard.md` to structure your audit evidence.
5. Apply the rules in `docs/Privileged_Access_Governance_AddOn.md` for privileged access.
6. Read `docs/Automation_Weekly_Privileged_Snapshots.md` for the automation concept.
7. See `docs/Framework_Mapping.md` to understand how this aligns with SOX ITGC, NIST, and ISO 27001.

## Important Note

This repository is a portfolio demonstration. Do not upload real company data, credentials, or production access exports.
