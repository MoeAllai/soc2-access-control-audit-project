# Evidence Request List

## Purpose

This document lists the audit evidence needed to test access management controls for CloudCore Analytics as part of SOC 2 Type II readiness.

The goal is to identify whether access controls are properly documented, approved, reviewed, and retained as evidence.

## Evidence Request Table

| Control ID | Control Area | Evidence Requested | System / Owner | Frequency | Acceptable Evidence | Red Flags |
|---|---|---|---|---|---|---|
| AC-01 | User Access Review | Latest user access review report showing users, roles, reviewer, date completed, and sign-off | Okta / IT Manager | Quarterly | Exported access review report, reviewer approval, remediation notes | No reviewer sign-off, missing dates, incomplete user list |
| AC-02 | Terminated User Removal | List of terminated employees and proof their access was removed from all in-scope systems | HRIS + Okta / HR & IT | Per termination | HR termination report, Okta deactivation logs, ticket closure evidence | User still active after termination date, no removal ticket |
| AC-03 | Privileged Access Review | List of admin users and evidence of management review | Okta, AWS, GitHub / IT Security | Quarterly | Admin user export, approval records, review notes | Unknown admin accounts, excessive privileges, no review evidence |
| AC-04 | MFA Enforcement | Screenshot or report showing MFA enforcement for users and admins | Okta / IT Security | Continuous | MFA policy screenshot, enrolled user report, exception list | MFA disabled for admins, missing exception approval |
| AC-05 | Access Request Approval | Tickets showing access requests were approved before access was granted | Jira / IT Helpdesk | Per request | Jira ticket, manager approval, access grant timestamp | Access granted before approval, missing approver |
| AC-06 | New Hire Access Provisioning | Sample of new hire access requests with approval and role-based access assignment | HRIS + Jira + Okta / HR & IT | Per new hire | New hire ticket, approved role, access provisioning logs | Access does not match job role, no approval |
| AC-07 | Access Removal for Role Changes | Evidence that access was updated when employees changed roles | HRIS + Jira / HR & IT | Per role change | Role change ticket, old access removed, new access approved | Old access retained, no review after transfer |
| AC-08 | Shared Account Review | List of shared/service accounts and evidence they are approved and monitored | Okta, AWS, GitHub / IT Security | Quarterly | Account inventory, owner approval, usage justification | No owner, no business justification, interactive login enabled |
| AC-09 | Evidence Retention | Evidence storage location and proof that audit evidence is retained | Google Drive / Compliance | Annual | Evidence folder, naming convention, retention policy | Missing files, unclear ownership, no version control |
| AC-10 | Exception Management | List of access control exceptions and approval evidence | IT Security / Compliance | Monthly | Exception register, approval, expiration date | Permanent exceptions, no approval, no expiration date |

## Evidence Quality Checklist

Evidence should be:

- Complete
- Dated
- Exported from the source system when possible
- Reviewed and approved by the correct owner
- Clear enough for an auditor to understand
- Stored in a centralized evidence folder
- Connected to the control being tested

## Example Evidence Request Email

Subject: SOC 2 Access Control Evidence Request

Hi Team,

As part of our SOC 2 readiness review, please provide the requested access control evidence for the systems you own.

Please include reports, screenshots, tickets, approvals, and any supporting documentation related to access reviews, user provisioning, offboarding, MFA, and privileged access.

Evidence should include the date, system name, reviewer or approver, and any remediation notes if exceptions were identified.

Thank you,  
Junior GRC Analyst

## Notes

This evidence request list is part of a mock GRC portfolio project. It is designed to demonstrate audit readiness, access control review, evidence collection, and SOC 2 control testing skills.
