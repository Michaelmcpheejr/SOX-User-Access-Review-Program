# Privileged Access Governance Add On

## Definition of Privileged Access

Privileged access is any account that can change system configurations, security settings, or financial data beyond normal business processing.

## Categories of Privileged Access

- Global or tenant administrators
- Security and compliance administrators
- Application configuration administrators
- Integration or service accounts with elevated rights

## Extra Rules for Privileged Accounts

- Named owner required  
  Each privileged account must have a documented owner.  

- Business justification required  
  Each privileged account must have a documented business justification stored in the tracker.  

- Shared accounts restricted  
  Shared privileged accounts are not allowed without a documented exception approved by security leadership.  

- High risk and break glass accounts  
  These accounts remain in scope for monthly review even if unused.  

- Unused privileged accounts disabled  
  Privileged accounts that remain unused for more than 14 days must be disabled.  

- Re enabling privileged accounts  
  Re enabling a disabled privileged account requires:  
  - Fresh business justification  
  - Approval from the next higher level of management above the account owner  

Example escalation model:

- If an IT Helpdesk privileged account is re enabled, approval must come from the Head of Information Security.  
- If a Head of Information Security account is affected, approval must come from the CISO.  
- If a CISO account is affected, approval must come from an appropriate governance authority, such as the Head of Information Security or equivalent committee, depending on the organization.

